# DeclaGuard

**A declarative security-policy framework for protecting no-code swarms of LLM agents against prompt injection.**

DeclaGuard is an independent proposed standard for swarms built with the AgentFlow no-code agent framework (Lande and Strashnoy). It specifies that the scenario author writes security policies as declarative fields of the same JSON swarm description that defines the agents, without code, and that an unchanged universal conductor enforces them deterministically, with no LLM-based detectors. Under the specification, the conductor blocks tool calls, messages between agents, transition conditions, state writes and answers that the policy does not allow, and records every decision in a journal.

> **Core principle.** Agents process data; the conductor decides what may be done with it.

## Status

**Specification v1.0 (complete).** [`FRAMEWORK/README.md`](FRAMEWORK/README.md) is the full normative standard: all enforcement points, the policy language, general policies, journal and conformance requirements.

## Contents

| Path | What it is |
|---|---|
| [`FRAMEWORK/README.md`](FRAMEWORK/README.md) | The DeclaGuard specification: threat model, formal model, policy language, general policies, enforcement points, journal, conformance requirements, validation protocol, limitations |
| [`EXAMPLES/news-tool/`](EXAMPLES/news-tool/) | Swarm description of the planned practical example (news digest sent with a tool) |

## Implementation status

The reference implementation and the practical example are under development. No results of the protection are reported yet.

## Related work

1. Lande D., Strashnoy L. AgentFlow – No-Code Agent Framework Based on Logical Primitives. SSRN, 2025. DOI: 10.2139/ssrn.5285664.
2. Lande D., Strashnoy L. Orchestration of No-Code Agents in the AgentFlow Framework. SSRN, 2025. DOI: 10.2139/ssrn.5381820.
3. Lande D., Strashnoy L., Kuzminskyi V. Extension of the Universal Conductor for Heterogeneous Execution Environments. SSRN, 2025. DOI: 10.2139/ssrn.5522698.
4. AgentFlowAttack: prompt-injection test on a reproduction of the AgentFlow conductor. GitHub repository, 2026. URL: https://github.com/sunflower3-collab/AgentFlowAttack.

DeclaGuard is an independent research project and is not an official part of AgentFlow.

## License

Apache License 2.0, see [`LICENSE`](LICENSE) and [`NOTICE`](NOTICE).
