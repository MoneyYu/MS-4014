---
image: https://learn.microsoft.com/en-us/training/achievements/generic-badge.svg
tags: MS-4014, Reference
GA: G-DXYJBX6BH8
---

# MS-4014 Reference

> 這份學員版參考頁對應 **Course MS-4014-A: Introduction to building AI agents**，以入門角度整理 AI 代理基礎、Microsoft 平台與工具選擇，以及解決方案規劃的官方學習資源，適合開發者與 app makers 在課前預習、課中對照與課後延伸。

## Course
:::success
Date: 20260810
Course ID: 103820
:::

:::info
Course Survey: [https://aka.ms/ms4014survey](https://aka.ms/ms4014survey)
:::

:::warning
本課程以講解、討論與短活動為主，會透過案例與提問協助你建立 AI 代理的核心概念與規劃思路；目前版本沒有 hands-on lab，建議搭配 Learn 模組與延伸資源安排課後練習。
:::

## Course Materials
### Learning path
[Learning path (EN)](https://learn.microsoft.com/en-us/training/paths/build-foundation-extend-microsoft-365-copilot/)

[Learning path (ZH-CN)](https://learn.microsoft.com/zh-cn/training/paths/build-foundation-extend-microsoft-365-copilot/)

[Learning path (ZH-TW)](https://learn.microsoft.com/zh-tw/training/paths/build-foundation-extend-microsoft-365-copilot/)

### Course page
[Course page (EN)](https://learn.microsoft.com/en-us/training/courses/ms-4014)

[Course page (ZH-CN)](https://learn.microsoft.com/zh-cn/training/courses/ms-4014)

[Course page (ZH-TW)](https://learn.microsoft.com/zh-tw/training/courses/ms-4014)

## Infos
[LxP portal](https://esi.microsoft.com)

[ESI Support](https://esisupport.microsoft.com/en-US/)

## Links
### M01 - Introduction to developing AI agents
[M01 module page](https://learn.microsoft.com/en-us/training/modules/introduction-develop-ai-agents/)

[Agent architecture principles and patterns](https://learn.microsoft.com/en-us/agents/architecture/)

[Agent architecture checklist](https://learn.microsoft.com/en-us/agents/architecture/checklist-agent-architecture)

### M02 - Choose tools and services for your agent on Microsoft's agent platform
[M02 module page](https://learn.microsoft.com/en-us/training/modules/build-solutions-microsoft-agent-platform/)

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
[M03 module page](https://learn.microsoft.com/en-us/training/modules/plan-design-ai-agent-solution/)

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
| 03-02 | Securing AI with Azure AI Foundry \| Built-in protections for Cloud & AI platforms | https://youtu.be/w3O1ZY_9lPg |

## What could be next?
[Follow-on path: Develop AI Agents on Azure](https://learn.microsoft.com/en-us/training/paths/develop-ai-agents-azure/)

[Follow-on path: Create agents in Microsoft Copilot Studio](https://learn.microsoft.com/en-us/training/paths/create-extend-custom-copilots-microsoft-copilot-studio/)

## Mind Map
```markmap
# Introduction to building AI agents (MS-4014)
## M01 - Introduction to developing AI agents
### 定義與價值
- [AI agents](https://learn.microsoft.com/en-us/training/modules/introduction-develop-ai-agents/) 會運用 AI 自動化並執行業務流程，可與人協作，也可代表人採取行動
- 從檢索型、任務型到自主型是一條連續體；是否需要多步驟執行與持續監控，會直接影響設計複雜度
### 使用案例與導入切入點
- 導入時先改善既有流程，把效率瓶頸、知識孤島或積壓工作轉成明確的 business outcome
- 常見場景可跨部門重複出現，例如 IT 支援、onboarding、客服與資料分析
### 架構元件
- [Knowledge / Tools / Autonomy / Model / Orchestrator](https://learn.microsoft.com/en-us/agents/architecture/) 是核心心智模型；Connected agents 用來擴充專長與協作
- 用 [agent architecture checklist](https://learn.microsoft.com/en-us/agents/architecture/checklist-agent-architecture) 先釐清需求、邊界與相依性，再進入平台討論
## M02 - Choose tools and services for your agent on Microsoft's agent platform
### 開發路徑與平台
- [Agent Builder](https://learn.microsoft.com/en-us/training/modules/build-solutions-microsoft-agent-platform/) 偏 no-code、[Copilot Studio](https://learn.microsoft.com/en-us/microsoft-copilot-studio/fundamentals-what-is-copilot-studio) 偏 low-code、[Microsoft Foundry](https://learn.microsoft.com/en-us/azure/foundry/what-is-foundry) 提供更高的自訂與部署控制
- Pro-code 需要把 development platform、orchestration 與 channels 分開規劃；彈性越高，治理責任也越明確
### Grounding 與整合
- [Work IQ](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/work-iq/)、[Foundry IQ](https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/what-is-foundry-iq)、[Fabric IQ](https://learn.microsoft.com/en-us/fabric/iq/overview) 要依資料域選用，而不是用單一服務硬套所有需求
- [MCP](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/model-context-protocol) 統一 agent 連接工具與資料來源；Copilot Studio 可走 connectors / Power Automate / REST，pro-code 則把 Logic Apps、Functions 或 OpenAPI 當成 tools
### 發佈、多代理與治理
- 通路不只是 UI 選擇，還決定發佈流程與預設治理；Copilot Studio 在 Microsoft 365 周邊通常繼承較多控制，Foundry 則需要明確設定 RBAC、logging 與 policies
- [A2A](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/agent-to-agent#host-an-a2a-compatible-agent-endpoint) 適合跨框架或跨組織協作；Microsoft 生態內的複合流程則優先用原生整合與 [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) 編排
## M03 - Plan an AI agent solution
### 成果與成功指標
- 先用 [M03 module page](https://learn.microsoft.com/en-us/training/modules/plan-design-ai-agent-solution/) 定義可衡量的 business outcome 與 scope；成功應該是前後對照，而不是功能清單
- 品質指標與 business value 指標都要先有 baseline；沒有現況數字，就無法證明改善是否成立
### 資料、workflow 與 interaction
- 先盤點 data domains 與 knowledge sources，再決定 grounding strategy；同一個 solution 可以混用多個服務，但要按 agent 與資料域拆開思考
- 用 input → transform → output 描繪 workflow，逐步判斷哪些步驟該用 deterministic、generative 或 hybrid pattern
- Conversational 與 autonomous 是兩種主要 interaction patterns；handoff、escalation 與 channel rules 都要在設計階段先說清楚
### 身分、治理與 Responsible AI
- 依操作模式規劃 [agent identity architecture](https://learn.microsoft.com/en-us/entra/agent-id/how-to-plan-agent-identity-architecture)，把 least privilege、sponsor / owner 與 review cadence 納入 blueprint
- [Guardrails](https://learn.microsoft.com/en-us/azure/foundry/guardrails/guardrails-overview) 要對準暴露面與 failure modes，而 [Responsible AI](https://learn.microsoft.com/en-us/agents/design-guidelines/responsible-ai) 要轉成具體的設計問題與檢核點
```

## Contact
- Money Yu
    - Mail: [Money.Yu@microsoft.com](mailto:Money.Yu@microsoft.com)
    - LinkedIn: [@abc12207](https://www.linkedin.com/in/abc12207/)
