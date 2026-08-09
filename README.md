---
image: https://learn.microsoft.com/en-us/training/achievements/generic-badge.svg
tags: MS-4014, Reference
GA: G-DXYJBX6BH8
---

# MS-4014 Reference
## Course
:::success
Date: 20260810
Course ID: 103820
:::

:::info
Course Survey: [https://aka.ms/ms4014survey](https://aka.ms/ms4014survey)
:::



## Course Materials
[Course MS-4014 English version](https://learn.microsoft.com/en-us/training/courses/ms-4014)

[Course MS-4014 简体中文版本](https://learn.microsoft.com/zh-cn/training/courses/ms-4014)

[Course MS-4014 正體中文版本](https://learn.microsoft.com/zh-tw/training/courses/ms-4014)

## Infos
[LxP portal](https://esi.microsoft.com)

[ESI Support](https://esisupport.microsoft.com/en-US/)

## Links
### M01 - Introduction to developing AI agents
[Agent architecture principles and patterns](https://learn.microsoft.com/en-us/agents/architecture/)

[Agent architecture checklist](https://learn.microsoft.com/en-us/agents/architecture/checklist-agent-architecture)

### M02 - Choose tools and services for your agent on Microsoft's agent platform
[Microsoft Foundry overview](https://learn.microsoft.com/en-us/azure/foundry/what-is-foundry)

[Copilot Studio overview](https://learn.microsoft.com/en-us/microsoft-copilot-studio/fundamentals-what-is-copilot-studio)

[Microsoft 365 Agents Toolkit overview](https://learn.microsoft.com/en-us/microsoftteams/platform/toolkit/agents-toolkit-fundamentals)

[M365 Agents SDK overview](https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/agents-sdk-overview)

[Foundry MCP tool connection](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/model-context-protocol)

[Foundry A2A endpoint guidance](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/agent-to-agent#host-an-a2a-compatible-agent-endpoint)

[Microsoft Agent Framework repo](https://github.com/microsoft/agent-framework)

[Work IQ overview](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/work-iq/)

[Foundry IQ overview](https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/what-is-foundry-iq)

[Fabric IQ overview](https://learn.microsoft.com/en-us/fabric/iq/overview)

[Microsoft Agent 365 overview](https://learn.microsoft.com/en-us/microsoft-agent-365/overview)

### M03 - Plan an AI agent solution
[Plan your agent identity architecture](https://learn.microsoft.com/en-us/entra/agent-id/how-to-plan-agent-identity-architecture)

[Foundry guardrails overview](https://learn.microsoft.com/en-us/azure/foundry/guardrails/guardrails-overview)

[Responsible AI for agent design](https://learn.microsoft.com/en-us/agents/design-guidelines/responsible-ai)

## Videos

### M01 - Introduction to developing AI agents
| No. | Name | Link |
| --- | --- | --- |
| 01-01 | What are AI agents? | https://youtu.be/3zgm60bXmQk |

### M02 - Choose tools and services for your agent on Microsoft's agent platform
| No. | Name | Link |
| --- | --- | --- |
| 02-01 | Foundry Agent Service + Microsoft Agent Framework Explained | https://youtu.be/iR7_57lJOz8 |
| 02-02 | Microsoft 365 Copilot \| Copilot Studio agent builder | https://youtu.be/uo-vCFL96yQ |

### M03 - Plan an AI agent solution
| No. | Name | Link |
| --- | --- | --- |
| 03-01 | How Microsoft Engineers Build AI: Building and Evaluating Agents | https://youtu.be/opAIBSooW9g |

## What could be next?
[Follow-on path: Develop AI Agents on Azure](https://learn.microsoft.com/en-us/training/paths/develop-ai-agents-azure/)

[Follow-on path: Create agents in Microsoft Copilot Studio](https://learn.microsoft.com/en-us/training/paths/create-extend-custom-copilots-microsoft-copilot-studio/)

## Mind Map
```markmap
# Introduction to building AI agents (MS-4014)
## M01 - Introduction to developing AI agents
### Definition and value
- [AI agents](https://learn.microsoft.com/en-us/training/modules/introduction-develop-ai-agents/) use AI to automate and execute business processes, collaborating with people or acting on their behalf.
- Retrieval, task-oriented, and autonomous agents form a continuum; requirements for multistep execution and continuous monitoring directly affect design complexity.
### Use cases and entry points
- Start by improving an existing process and turn efficiency bottlenecks, knowledge silos, or backlogs into a clear business outcome.
- Common scenarios recur across departments, including IT support, onboarding, customer service, and data analysis.
### Architecture components
- [Knowledge / Tools / Autonomy / Model / Orchestrator](https://learn.microsoft.com/en-us/agents/architecture/) form the core mental model; connected agents extend specialization and collaboration.
- Use the [agent architecture checklist](https://learn.microsoft.com/en-us/agents/architecture/checklist-agent-architecture) to clarify requirements, boundaries, and dependencies before discussing platforms.
## M02 - Choose tools and services for your agent on Microsoft's agent platform
### Development paths and platforms
- [Agent Builder](https://learn.microsoft.com/en-us/training/modules/build-solutions-microsoft-agent-platform/) is primarily no-code, [Copilot Studio](https://learn.microsoft.com/en-us/microsoft-copilot-studio/fundamentals-what-is-copilot-studio) is low-code, and [Microsoft Foundry](https://learn.microsoft.com/en-us/azure/foundry/what-is-foundry) provides greater customization and deployment control.
- Pro-code solutions require separate planning for the development platform, orchestration, and channels; greater flexibility brings clearer governance responsibility.
### Grounding and integration
- Select [Work IQ](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/work-iq/), [Foundry IQ](https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/what-is-foundry-iq), and [Fabric IQ](https://learn.microsoft.com/en-us/fabric/iq/overview) by data domain instead of forcing every requirement into one service.
- [MCP](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/model-context-protocol) standardizes agent connections to tools and data sources; Copilot Studio can use connectors, Power Automate, or REST, while pro-code treats Logic Apps, Functions, or OpenAPI as tools.
### Publishing, multi-agent solutions, and governance
- Channels are more than a UI choice: they determine publishing flows and default governance. Copilot Studio often inherits more Microsoft 365 controls, while Foundry requires explicit RBAC, logging, and policies.
- [A2A](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/agent-to-agent#host-an-a2a-compatible-agent-endpoint) supports cross-framework or cross-organization collaboration; composite workflows in the Microsoft ecosystem should prioritize native integration and [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) orchestration.
## M03 - Plan an AI agent solution
### Outcomes and success metrics
- Use the [M03 module page](https://learn.microsoft.com/en-us/training/modules/plan-design-ai-agent-solution/) to define a measurable business outcome and scope; success is a before-and-after comparison, not a feature list.
- Quality and business-value metrics both need baselines; without current-state data, improvement cannot be demonstrated.
### Data, workflows, and interaction
- Inventory data domains and knowledge sources before choosing a grounding strategy. A solution can combine services, but agents and data domains should be considered separately.
- Model the workflow as input → transform → output, then determine which steps use deterministic, generative, or hybrid patterns.
- Conversational and autonomous are the primary interaction patterns; define handoffs, escalations, and channel rules during design.
### Identity, governance, and Responsible AI
- Plan an [agent identity architecture](https://learn.microsoft.com/en-us/entra/agent-id/how-to-plan-agent-identity-architecture) for the operating model, including least privilege, sponsor/owner roles, and review cadence in the blueprint.
- Align [guardrails](https://learn.microsoft.com/en-us/azure/foundry/guardrails/guardrails-overview) to exposure surfaces and failure modes, and translate [Responsible AI](https://learn.microsoft.com/en-us/agents/design-guidelines/responsible-ai) into concrete design questions and checkpoints.
```

## Contact
- Money Yu
    - Mail: [Money.Yu@microsoft.com](mailto:Money.Yu@microsoft.com)
    - LinkedIn: [@abc12207](https://www.linkedin.com/in/abc12207/)
