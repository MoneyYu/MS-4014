# MS-4014 備課指南

> [!WARNING]
> **這份指南只適用於 July 2026 major refresh 版的 MS-4014。**
> 請不要沿用舊版的 Graph connectors、declarative agents、舊 YouTube playlist、舊 labs，也不要把課程講成舊版的 Copilot extensibility / development-path 課。
> 目前正式結構是 **3 個模組**、**3 小時 instructor-led core delivery（含 15 分鐘 break）**，而且互動方式以 Discussion、Activity、Try it 與選擇性 demo 為主。版本差異請對照 [version-change-notes.md](version-change-notes.md)，詳細 legacy 說明與 migration notes 以該文件為準。

> [!IMPORTANT]
> 本文件是 trainer-only 備課內容。學員公開材料請維持在 [../README.md](../README.md)；不要把本文的 facilitation cue、Knowledge Check 解釋與版本風險提醒直接搬到學員版。

## 課程概覽

- **課程定位**：MS-4014 是一門 *planning-first* 的入門課。它先建立 AI agents 的共同語言，再帶學員比較 Microsoft 平台與服務，最後收斂到 solution planning；它不是 hands-on build lab，也不是單一產品操作課。
- **對象**：Trainer Prep Guide 將本課定位給想理解 AI agents、agent development options 與 AI transformation 的 developers 與 makers。
- **學員先備**：建議學員先具備 Microsoft 365 Copilot 基本熟悉度、agents / models / orchestration 等 generative AI 基本概念，以及 Microsoft 365、Power Platform、Azure 等核心 Microsoft Cloud 平台的概念。
- **講師先備**：講師最好已經實際接觸過 AI agents 或 Microsoft 365 Copilot extensibility，並能清楚講解 model、orchestrator、custom agent、plugin、connector、Copilot connectors 等關鍵詞。

| 面向 | 公開 Learn 課程頁 | 講師實際交付依據 |
| --- | --- | --- |
| 對外呈現 | [Course MS-4014-A](https://learn.microsoft.com/en-us/training/courses/ms-4014) 目前仍顯示 **Course Duration = 1 day**，並以 self-directed learning / Achievement Code 的 catalog 方式呈現。 | Trainer Prep Guide 明確寫成 **3-hour instructor-led course including a 15-minute break**。 |
| 你該怎麼用 | 用來說明課程定位、公開描述與 Achievement Code 脈絡。 | 用來決定實際 run-of-show、互動密度、demo 深淺與時間切法。 |
| 備課原則 | 不要因為 Learn 頁面寫 1 day，就把內容展開成全日版或補回舊 labs。 | 一律以當次 issued schedule 規劃交付：先看你拿到的是 3 小時、半日併班、還是內訓壓縮版，再決定互動分享長度。 |

補一句話給自己：**這門課的核心不是把某個 agent 做出來，而是幫學員建立「怎麼選平台、怎麼規劃 solution、怎麼避免一開始就走錯」的判斷框架。**

## 課程地圖：3 個模組

| 模組 | 主軸 | 建議教學格式 | 互動與檢核 |
| --- | --- | --- | --- |
| **M01 - Introduction to developing AI agents** | 平台無關的 agent 基本觀念、business value、use cases、architecture vocabulary | 以講解為主，先讓學員把「agent ≠ 單純 chatbot」這件事講清楚 | **1 個 Discussion（Slide 8）+ 1 個 Activity（Slide 13）+ Knowledge Check（Slide 18）** |
| **M02 - Choose tools and services for your agent on Microsoft's agent platform** | development path、channels、grounding、integrations、governance/identity 的選擇題 | 以 scenario-based comparison 為主，不是 build tutorial | **5 個 Discussions（Slides 29/36/41/47/53）+ Knowledge Check（Slides 54/55）** |
| **M03 - Plan an AI agent solution** | outcomes、workflow、interaction patterns、identity/governance/security/Responsible AI 的 planning discipline | 以 planning-first 設計思考為主，讓學員把 agent blueprint 講完整 | **2 張 Discussion slides（Slides 70/90）+ 1 個 Try it 互動（Slide 78）+ Knowledge Check（Slides 91/92）** |

請特別記住：**deck 只有 8 張標題明確寫成 `Discussion` 的投影片。** Trainer Prep Guide 對 M03 寫的是 3 個 discussion moments，但在 deck 內的實際呈現是 **2 張 `Discussion` + 1 個 `Try it`**；不要把互動總數誤讀成「多出一張同名 `Discussion` 投影片」。

## 建議議程與時間分配

Trainer Prep Guide 同時給了「3-hour course（含 break）」與各段 component time budget。實際備課時，不要把所有高標時間直接相加；**標準 3 小時場次要用低標起跑，並把 Knowledge Check 與 share-out 壓進講解流程。**
另外要先接受一個事實：**就算全部採低標，Intro + M1 + Break + M2 + M3 + Conclusion 合計仍約 224 分鐘，已高於 180 分鐘的表定課長**；因此 issued schedule 若仍是 3 小時，就一定要再裁切互動分享或把部分檢核完全融入講解。

| 區段 | Trainer Prep Guide time budget | 講師場控建議 |
| --- | --- | --- |
| Intro | 10–15 分鐘 | 只做版本警告、課程定位、互動規則與 expectation setting。不要在這裡展開產品史。 |
| M01 presentation | 25–30 分鐘 | 用 1 個學員熟悉的流程案例，把 retrieval → task → autonomous continuum 一次講清楚。 |
| M01 discussion | 5–10 分鐘 | Slide 8 最多抓 2–3 組分享即可，其餘用 chat 蒐集。 |
| M01 activity | 5–10 分鐘 | 時間緊時壓到 5 分鐘；必要時改成講師示範 1 個案例 + 學員口頭回應。 |
| M01 knowledge check | 3–5 分鐘 | 直接口頭快問快答，不要開成獨立測驗段。 |
| Break | 15 分鐘 | 建議固定保留。第二小時開始會進入 platform choice 與 governance，學員精神很重要。 |
| M02 presentation | 55–60 分鐘 | 這是最容易超時的模組，務必用同一個 scenario 貫穿，不要每張 slide 換一個例子。 |
| M02 five discussions | 20–35 分鐘 | 每題 3–5 分鐘即可；若 schedule 緊，保留 verbal share-out 給 Slides 29 與 41，其他題目用 chat waterfall。 |
| M02 knowledge check | 3–5 分鐘 | 只挑最容易混淆的平台 / IQ / governance 題目做口頭檢核。 |
| M03 presentation | 55–60 分鐘 | 這段是整門課的收斂，寧可少 demo，也不要壓縮 outcomes / workflow / identity 的邏輯鏈。 |
| M03 two Discussions + Try it | 15–35 分鐘 | Slide 70 適合 pair-share；Slide 78 Try it 要求畫 workflow；Slide 90 依 speaker notes 只挑 1–2 題即可。 |
| M03 knowledge check | 3–5 分鐘 | 因 Slides 91/92 的 deck notes 沒有 authoritative answer，若你還沒先驗證，就不要現場公布「標準答案」。 |
| Conclusion | 10 分鐘 | 回收三件事：怎麼選平台、怎麼選 grounding / integrations、怎麼先規劃再 build。 |

### 時間風險控制

1. **先鎖低標，不鎖高標**：標準 3 小時班先按每段低標排；有額外時間再放大分享，不要反過來。
2. **Knowledge Check 融入講解**：Trainer Prep Guide 明說可以把 Knowledge Checks 混在授課過程中，而不是每模組都切獨立小考。
3. **M02 是最大超時點**：platform、channels、IQ、integrations、governance 全在同一模組，最容易被 demo 與比較題拉長。
4. **Slide 90 只選 1–2 題**：speaker notes 已經授權依 audience relevance 選題；不要四題全開。
5. **demo 只做「看懂差異」**：這門課不需要 live build。若 demo 讓你離開主線，就砍 demo，不要砍 planning 主軸。
6. **不要把低標當成可直接照抄的 run-of-show**：低標總和仍超出 3 小時，必須主動裁切；否則最常被犧牲的會是 M03，而那正是本課最重要的 planning 收斂段。

## 貫穿全課的核心觀念

1. **Agent continuum 與 architecture 是全課底圖**
   M01 先把 retrieval / task / autonomous 當成連續體，而不是硬分類；再用 Knowledge、Tools、Autonomy、Model、Orchestrator、Connected agents 畫出 agent architecture。後面 M02 的平台選擇、M03 的 solution planning 都是沿著這張底圖展開。

2. **low-code vs pro-code 是「控制權與責任」的選擇，不是高低之分**
   Agent Builder 偏 no-code、Copilot Studio 偏 low-code、Microsoft Foundry 提供更高的 model / orchestration / channel 控制。要讓學員理解：控制權越高，治理責任越明確；不是 Foundry 比 Copilot Studio「更高級」，而是適用條件不同。

3. **Microsoft IQ / grounding 要從 data domain 反推**
   先問資料在哪裡、長什麼樣、授權模型是什麼，再問要用 Work IQ、Foundry IQ、Fabric IQ，或多個服務組合。不要把 grounding 講成「接一個知識庫就好」。

4. **channels、integrations、A2A、MCP 其實是在談 agent 的邊界與互通**
   channel 不只是 UI；它同時決定 publishing path 與 governance defaults。MCP 是 agent 連到 tools / data 的通用方式；A2A 是跨 frameworks / platforms / organizations 的 agent-to-agent 協作；Microsoft 生態內則優先考慮 native integration。

5. **identity、governance、least privilege、Responsible AI 要在 planning 階段進場**
   這不是 build 完再補的工作。interaction pattern、permissions、agent user account、guardrails、sponsor / owner、review cadence，都會反過來改寫 solution design。

6. **術語要全部更新到 current terminology**
   - Graph connectors → **Copilot connectors**
   - Teams Toolkit → **Microsoft 365 Agents Toolkit**
   - Teams AI Library → **Teams SDK**
   - Azure AI Foundry → **Microsoft Foundry**
   - Azure AI Agent Service → **Foundry Agent Service**
   - Semantic Kernel + AutoGen → **Microsoft Agent Framework**
   - Agent Builder 是 **Copilot Studio 的 lite version**，不要把兩者講成完全相同，也不要沿用舊版把 declarative agents 當成這門課的主線。

## 逐模組備課指南

### M01 - Introduction to developing AI agents

#### 學習目標

- Define AI agents
- Explain the business value of AI agents
- Identify common use cases for AI agents
- Define the core components of AI agents

#### 講解重點

- 這一模組 **platform-agnostic**；先建立共同語言，再進入 M02 的 Microsoft 平台地圖。
- Slide 4 要講清楚 agent 的工作定義：agents use AI to **automate and execute** business processes，這是它和單純 generative chat assistant 的分水嶺。
- Slide 5 的 continuum 很重要：retrieval、task、autonomous 是範圍，不是三個互斥盒子。
- Slides 7–12 要把 pain point → business value → use case → process-first 切入一路串起來，避免學員只記住炫技案例。
- Slides 15–17 要用 architecture vocabulary 為 M02 鋪路：Knowledge、Tools、Autonomy、Model、Orchestrator、Connected agents。

#### 互動設計

- **Slide 8 — `Discussion`**
  Prompt: **"which business value or opportunity area could have the greatest impact for your team or organization?"**
  Facilitation:
  - 給 3–5 分鐘先自己想或 pair discussion，再請少數幾位分享。
  - speaker notes 建議把共通答案記在白板或 chat，後面講 use cases 與 platform choice 時再回勾。
  - 常見答案通常會落在「知識不好找、流程卡住、backlog 成長快過 headcount」。

- **Slide 13 — `Activity`**
  Prompt: **"explore real-world use cases"**
  Facilitation:
  - speaker notes 建議讓學員看 Microsoft WorkLab 的案例頁，挑與自己團隊相關的類別再回來分享。
  - 這個活動的真正目的不是「找最炫的案例」，而是把 Slide 8 找到的 pain point，對應到可落地的 agent use case。
  - 因該外部頁面網址不在本 repo 的 approved-current link ledger 中，若你要現場開啟，請在開課前自行重新驗證；本文不列正式 URL。

#### Knowledge Check

- **Slide 18 Q1**：企業導入 AI agents 的關鍵 business benefit 是 **"Enhancing efficiency by automating routine business processes."**
  說明：speaker notes 明確指出這才是 core value proposition；增加 manual data entry 或減少跨部門合作都不是正向答案。

- **Slide 18 Q2**：AI agents 在 business environment 的核心特徵是 **"They use knowledge, perform actions, and follow instructions to achieve business goals."**
  說明：這呼應 architecture slide 的 working definition；它們不是單純 data store，也不是每一步都要靠人手動盯著做。

- **Slide 18 Q3**：marketing team 用 agent 發送活動提醒且遵循團隊指引，需要的元件是 **"Custom knowledge, skills, and actions."**
  說明：情境同時需要團隊指引、可重用能力，以及送信等可執行 actions。

#### 常見誤區與提醒

- 把 agent 當成「會聊天的 chatbot」；M01 要先把 *does things* 這件事講進去。
- 把 retrieval / task / autonomous 當成硬分類；speaker notes 已經提醒這是一條 continuum。
- 一開始就想做最大的 transformation program；Slide 12 明確主張先改善既有流程，不要 boil the ocean。
- 只念 architecture 名詞，不用同一個例子把 request flow 走一次；這會讓 M02 的平台比較失去落點。

#### 重要連結

- [M01 module page](https://learn.microsoft.com/en-us/training/modules/introduction-develop-ai-agents/)
- [Agent architecture principles and patterns](https://learn.microsoft.com/en-us/agents/architecture/)
- [Agent architecture checklist](https://learn.microsoft.com/en-us/agents/architecture/checklist-agent-architecture)

### M02 - Choose tools and services for your agent on Microsoft's agent platform

#### 學習目標

- Identify the appropriate agent development path for a given scenario
- Identify the publishing paths and channel options for delivering agents to users
- Match organizational data categories to the appropriate Microsoft IQ service
- Describe how agents connect to external systems and coordinate with other agents
- Identify the governance and identity services that support agents

#### 講解重點

- 這一模組是 **identify-and-match module**，不是 build tutorial。重點是「看到需求，就知道該往哪個 platform / service / pattern 走」。
- Slides 23–29 請用「layers of agent development」來講清楚 Agent Builder、Copilot Studio、Microsoft Foundry 的差別：差別不在行銷定位，而在 **哪些 layers 由平台代管、哪些 layers 由你自己選**。
- Slides 30–36 要把 **channel = publishing path + governance default** 這件事講明白；不要只講「哪裡可以顯示」。
- Slides 37–41 強調 **Microsoft IQ family** 是 grounding 的 managed layer，而且要從 data domain 反推 Work IQ / Foundry IQ / Fabric IQ。
- Slides 42–47 要把 **MCP、connectors、Power Automate、Logic Apps、Functions、OpenAPI、A2A** 放進同一個「agent 如何獲得 agency」框架裡。
- Slides 48–58 要收斂到 identity / governance：每個 agent 都有身分；Copilot Studio / Microsoft 365 Copilot 有較多 inherited controls，Foundry 則要顯式配置 RBAC、policies、logging。

#### 互動設計

- **Slide 29 — `Discussion`**
  Prompt 1: **"Which development approach fits your team profile and scenario?"**
  Prompt 2: **"If you're on the pro-code path, which options at each layer fit your team's existing skills and your agent's requirements?"**
  Facilitation:
  - 停下來讓學員 3–5 分鐘討論，再請幾位分享。
  - speaker notes 特別提醒：注意學員不要 reflexively pattern-match，而沒有真的看 scenario nuance。

- **Slide 36 — `Discussion`**
  Prompt: **"For the agent you're building or exploring, which channel or channels best fit where your intended users already work?"**
  Facilitation:
  - 引導學員先說 target users 在哪裡工作，再說 channel。
  - 要主動反駁「all channels for maximum reach」這個直覺；speaker notes 已經提醒 governance defaults 與 support burden 會隨 channel 增加而放大。

- **Slide 41 — `Discussion`**
  Prompt: **"Think about the data your agent will need to reason over. Which IQ service or combination of services fits your scenario?"**
  Facilitation:
  - 要求學員把資料講具體，不要說泛泛的「company data」。
  - speaker notes 點名：很多真實案例會是 Foundry IQ + Work IQ 的組合，而不是單一服務。

- **Slide 47 — `Discussion`**
  Prompt: **"What external systems will the agent in your scenario need to act on? And does that scenario involve coordinating with other agents?"**
  Facilitation:
  - 請學員分開列出 read-from 與 write-to systems，因為治理風險不一樣。
  - 再追問：這是 Microsoft 內部 native integration 就能處理，還是真的需要 A2A？

- **Slide 53 — `Discussion`**
  Prompt: **"Based on the development platform you explored, which governance areas require explicit configuration by the development team, and which are inherited by default?"**
  Facilitation:
  - 這題的目的不是背控制項，而是讓學員意識到 governance 是 design input。
  - 講完要收束回：「不是平台比較安全，而是 default inheritance 不同，責任分配不同。」

#### Knowledge Check

- **Slide 54 Q1**：最適合 customer-facing returns agent、multi-step enterprise workflows、custom orchestration、full model control 的平台是 **Microsoft Foundry**。
  說明：speaker notes 明確點出這是 pro-code developer profile。Copilot Studio 偏 low-code，不提供此情境需要的 custom orchestration / model control；Agent Builder 則更不適合。

- **Slide 54 Q2**：集中式 product catalog / technical specifications / policy documents knowledge base 的 grounding 服務是 **Foundry IQ**。
  說明：這是 enterprise content / knowledge base 情境；Work IQ 偏 Microsoft 365 activity signals，Fabric IQ 偏 analytical / operational data。

- **Slide 54 Q3**：Foundry agent 沒有 audit logging 或 access controls、Copilot Studio agent 卻有，原因是 **Foundry 需要顯式設定 Azure RBAC、policies、logging；Copilot Studio 會繼承 Microsoft 365 controls**。
  說明：speaker notes 明確否定「Agent 365 會自動替 Foundry 套上同樣治理」與「只是 SaaS vs PaaS 差異」這兩個說法。

- **Slide 55 Q4**：讓 Copilot Studio agent 進入 Microsoft 365 Copilot 給全員使用的 distribution mechanism 是 **Copilot Control System**。
  說明：這是 admin-governed publishing path。`Agent Application` 是 Foundry 的 publishing resource；Microsoft 365 Agents SDK 是 pro-code channel / transport layer，不是既有 Copilot Studio agent 的 distribution mechanism。

- **Slide 55 Q5**：要讓 third-party / self-hosted agent 被其他 agents 呼叫，應使用 **registering an incoming A2A endpoint**。
  說明：A2A 解的是 multi-agent callability across frameworks / platforms；Microsoft 365 Agents SDK 解的是 agent 觸達 Microsoft 365 channels；Copilot Control System 解的是 user distribution。

#### 常見誤區與提醒

- 以為 **Microsoft Foundry 只代表 pro-code**。speaker notes 明說 Foundry 也支援 configuration-based prompt agents。
- 以為 **channel 只是 UI**。其實 channel 會改變 publishing path 與 governance defaults。
- 以為 **grounding 只要接一個資料源**。真正的重點是 data domain、freshness、permissions 與 multi-IQ 組合。
- 把 **MCP** 與 **A2A** 混為一談：MCP 偏 tools / data access；A2A 偏 agent-to-agent coordination。
- 以為 **Agent 365** 會自動補齊 Foundry 的治理設定；speaker notes 已明確否定。
- 把 **Agent Builder** 與 **Copilot Studio** 畫上等號；正確說法是 Agent Builder 是 Copilot Studio 的 lite version。

#### 重要連結

- [M02 module page](https://learn.microsoft.com/en-us/training/modules/build-solutions-microsoft-agent-platform/)
- [Microsoft Foundry overview](https://learn.microsoft.com/en-us/azure/foundry/what-is-foundry)
- [Copilot Studio overview](https://learn.microsoft.com/en-us/microsoft-copilot-studio/fundamentals-what-is-copilot-studio)
- [Microsoft 365 Agents Toolkit overview](https://learn.microsoft.com/en-us/microsoftteams/platform/toolkit/agents-toolkit-fundamentals)
- [Microsoft 365 Agents SDK overview](https://learn.microsoft.com/en-us/microsoft-365/agents-sdk/agents-sdk-overview)
- [Microsoft Agent Framework repo](https://github.com/microsoft/agent-framework)
- [Work IQ overview](https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/work-iq/)
- [Foundry IQ overview](https://learn.microsoft.com/en-us/azure/foundry/agents/concepts/what-is-foundry-iq)
- [Fabric IQ overview](https://learn.microsoft.com/en-us/fabric/iq/overview)
- [Connect agents to MCP server endpoints](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/model-context-protocol)
- [A2A endpoint guidance](https://learn.microsoft.com/en-us/azure/foundry/agents/how-to/tools/agent-to-agent#host-an-a2a-compatible-agent-endpoint)
- [Microsoft Agent 365 overview](https://learn.microsoft.com/en-us/microsoft-agent-365/overview)

### M03 - Plan an AI agent solution

#### 學習目標

- Plan business outcomes, requirements, and success metrics for an agent
- Plan an agent's data sources, workflows, and dependencies
- Plan an agent's interaction patterns and channels
- Plan an agent's identity, governance, security, and responsible AI posture

#### 講解重點

- 這一模組請明確框成 **planning-first design**，不是 tool training。Slides 60–62 要先讓學員相信：跳過 planning，最後會在 production 用 incident 補課。
- Slides 64–69 要把 **outcome、scope、handoff conditions、acceptance criteria、baseline metrics** 串成一條線。這裡最重要的訊息是：**metrics are design constraints**，不是上線後才補的 dashboard。
- Slides 72–78 要把 **data domain、grounding strategy、input → transform → output、deterministic vs generative vs hybrid、modularity、dependencies** 講成同一件事：如何把 agent 的工作拆對。
- Slides 80–83 要幫學員辨識 **conversational vs autonomous**，並理解 channel 與 cross-agent invocation 是 interaction design，不只是 deployment 細節。
- Slides 84–90 要把 **identity、least privilege、agent user account、guardrails、lifecycle governance、Responsible AI** 放在同一張 blueprint 上看。

#### 互動設計

- **Slide 70 — `Discussion`**
  Prompt: **"What does success look like for your agent in concrete terms? And what data exists today to establish a baseline you could measure against?"**
  Facilitation:
  - 建議 pair-and-share 5–10 分鐘。
  - speaker notes 要求你一直追問具體數字：不是 faster / better，而是「哪個 number、怎麼量、跟哪個 baseline 比」。

- **Slide 78 — `Try it`**
  Prompt 1: **"Sketch a workflow for an agent you’re considering building, using input → transform → output."**
  Prompt 2: **"What triggers the agent?"**
  Prompt 3: **"What does it read, and from which data domain?"**
  Prompt 4: **"What produces the result — a response, handoff, record, or notification?"**
  Prompt 5: **"For each transform step, decide: does it need generative reasoning, or is deterministic logic more reliable and auditable?"**
  Facilitation:
  - 讓學員真的畫，不要只口頭講；speaker notes 認為畫出 input → transform → output 最能暴露 design gaps。
  - 要特別抓「什麼都想用 generative reasoning」這個傾向，主動把 deterministic / auditable step 拉回來。

- **Slide 90 — `Discussion`**
  Prompt 1: **"Which operation pattern does your agent use?"**
  Prompt 2: **"Does it need an agent’s user account?"**
  Prompt 3: **"At which intervention points would you place guardrails, and what failure mode is each protecting against?"**
  Prompt 4: **"Which responsible AI principle presents the highest design risk for this agent, and what decision from this unit addresses it?"**
  Facilitation:
  - speaker notes 明確建議只挑 1–2 題，依 audience relevance 決定。
  - guardrails 這題一定要追問 **named failure mode**，不能接受「這裡加個 guardrail 就好」。
  - agent user account 這題要講清楚：application permissions 處理 background processing；若場景需要 user-shaped presence（例如 shared mailbox 發信），才需要額外的 agent user account。

#### Knowledge Check

- **Slides 91/92 沒有 authoritative answer 可直接引用。**
  deck 的 speaker notes 對 Slides 91/92 明確是 **No speaker-note text present in the deck**；題目本身也沒有附答案或解釋。

- 因此請嚴格遵守這條：
  - **不要臨場猜答案。**
  - **不要把你自己的技術直覺講成官方標準答案。**
  - **講師必須在授課前，對照當前 source material 重新驗證這 5 題。**

- 這 5 題主題分別圍繞：
  - baseline before success metrics
  - deterministic vs agentic routing step
  - autonomous interaction pattern
  - tool response intervention point
  - autonomous permissions + agent user account

#### 常見誤區與提醒

- 把 planning 當成 paperwork；Slides 61–62 明確指出 outcomes / baselines / boundaries 是 build input。
- 沒 baseline 就先定 success metrics；speaker notes 直接說這是最常被跳過、也最難事後補回來的設計步驟。
- 什麼 step 都想用 generative reasoning；Slide 75 明確說 hybrid 往往才是較佳起點。
- 以為 guardrails 越多越安全；Slide 87 明確提醒每個 control 都有 latency cost，要看 actual exposure。
- 先加 agent user account 再說；Slide 85 明確提醒這有 licensing 與 policy complexity 成本，不要 speculative。
- 把 Responsible AI 當 compliance checklist；Slide 89 的正確講法是把原則轉成此 agent 的 design question。

#### 重要連結

- [M03 module page](https://learn.microsoft.com/en-us/training/modules/plan-design-ai-agent-solution/)
- [Plan your agent identity architecture](https://learn.microsoft.com/en-us/entra/agent-id/how-to-plan-agent-identity-architecture)
- [Foundry guardrails overview](https://learn.microsoft.com/en-us/azure/foundry/guardrails/guardrails-overview)
- [Responsible AI for agent design](https://learn.microsoft.com/en-us/agents/design-guidelines/responsible-ai)

## 預期學員問題 Q&A

### 為什麼這門課沒有 lab？

因為這個版本的 delivery model 本來就不是 lab-first。Trainer Prep Guide 明確寫出：這一版沒有 hands-on lab sequence，課程以 presentation、discussion、brief activities、optional demos 與 Learn follow-up 為主；README 也已經對學員說明目前版本沒有 hands-on lab。

### 這門課有 Applied Skills 或 exam 嗎？

依目前公開 Learn 課程頁，MS-4014 顯示的是 **Achievement Code**；在本次 required source set 與公開課程頁中，沒有列出 Applied Skills 或 exam/certification path。對外請只承諾目前可證實的 **Achievement Code**，不要自行延伸成「有考試」或「有技能認證」。

### Copilot Studio、Microsoft Foundry、pro-code 路線怎麼選？

先看你要控制什麼、團隊會什麼、以及 agent 要跑在哪裡：

- **Agent Builder**：no-code，偏個人或小團隊快速起步。
- **Copilot Studio**：low-code，適合 departmental agents、connectors / workflows、多數 Microsoft 365 周邊情境。
- **Microsoft Foundry**：當你需要 full model control、custom orchestration、production-grade architecture、direct API path 或 multi-agent backend specialization。
- **pro-code** 並不只是一個產品；它通常是 Microsoft Foundry + orchestration framework + channel SDK 的組合。

### 舊版材料、舊 playlist、舊 labs 和現在的關係是什麼？

它們是 **legacy evidence**，不是 current teaching baseline。July 2026 refresh 已經把課程改成 3 模組、3 小時、discussion-oriented 的新結構；舊 playlist 與舊 labs 都不是這版的核心材料。若你真的要用舊 demo videos，只能把它們當成「歷史補充」，而且要先下載、先驗證、現場清楚標註 **old / not updated for current version**。

### Microsoft IQ 到底是在解什麼問題？

它解的是 grounding 的平台化與 permission-aware access 問題。你不是先選產品，而是先看資料 domain：

- **Work IQ**：Microsoft 365 signals 與工作脈絡
- **Foundry IQ**：enterprise documents / knowledge bases / structured content
- **Fabric IQ**：analytical / operational data 的 semantic layer

同一個 agent 可能同時用多個 IQ 服務；這是正常設計，不是例外。

### 為什麼還沒 build，就一直談 governance、identity、least privilege？

因為這些不是 implementation polish，而是 architecture input。agent 要不要 autonomous、要不要 agent user account、哪裡需要 guardrails、哪些 permissions 可接受、誰是 sponsor / owner，都會反過來影響 channel、workflow、data access 與 rollout 方式。晚談，通常就代表你要用事故或 rework 來補。

## 課前準備清單（開課前 1–2 天）

- [ ] 重新看一次 **Change Log**，確認自己講的是 **July 2026 major refresh** 的 3 模組版本。
- [ ] 重新看一次 **PowerPoint deck** 與 speaker notes，特別標出 Slides 8 / 13 / 29 / 36 / 41 / 47 / 53 / 70 / 78 / 90 / 91 / 92。
- [ ] 重新確認本文件中引用的官方 Learn / GitHub 連結仍對應到 current content；若 Learn 頁面標題或結構已變，先更新再開課。
- [ ] 決定你要不要做 **live portal demos**；若要做，只挑 1–2 個最能說明差異的畫面，不要臨場探索。
- [ ] 若要使用舊 demo videos，請 **先下載**、先測試可播放，並在講義或口頭上明確說明那是 **legacy / old**，不是 current workflow。
- [ ] 確認 **ESI logistics**：issued schedule、LxP / survey 流程、遠距或實體上課的 chat / 白板 / 分組方式。
- [ ] 提前驗證 **Knowledge Check Slides 91/92** 的答案來源；如果還沒驗證完，先決定要把它們當課後 review，而不是課內標準答案題。
- [ ] 檢查你準備示範的 current terminology 是否一致：Microsoft Foundry、Foundry Agent Service、Microsoft 365 Agents Toolkit、Copilot connectors、Microsoft Agent Framework。

## 講師小技巧

- **不要讀投影片**：Trainer Prep Guide 已明說，slides 與 imported graphics 只是 anchor。你要補的是 What / Why / How，不是逐字朗讀。
- **用同一個 customer scenario 貫穿三模組**：M01 定義 agent、M02 選平台與服務、M03 畫 blueprint，全都用同一個 scenario，學員最容易跟得住。
- **先蒐集痛點，再回勾**：Slide 8 收到的例子，後面在 M02 platform choice、M03 success metrics 時再拿回來用，學員會感覺整堂課是連續的。
- **時間不夠時，先砍 share-out，不先砍思路**：chat waterfall、pair-share、舉手投票都能省時間；但不要因為趕時間就跳過 baseline、workflow、identity 的關鍵邏輯。
- **demo 的最佳範圍是「看懂差異」，不是「從零做到完」**：最值得 demo 的通常是 Agent Builder / Copilot Studio / Microsoft Foundry 的界面差異、publishing path、Agent Application、IQ / guardrails / identity 的位置，而不是 live build。
- **對 Slides 91/92 保持紀律**：未驗證就不公布標準答案，這比講錯還專業。

## 參考

- [Learning path (EN)](https://learn.microsoft.com/en-us/training/paths/build-foundation-extend-microsoft-365-copilot/)
- [Learning path (ZH-TW)](https://learn.microsoft.com/zh-tw/training/paths/build-foundation-extend-microsoft-365-copilot/)
- [M01 module page](https://learn.microsoft.com/en-us/training/modules/introduction-develop-ai-agents/)
- [M02 module page](https://learn.microsoft.com/en-us/training/modules/build-solutions-microsoft-agent-platform/)
- [M03 module page](https://learn.microsoft.com/en-us/training/modules/plan-design-ai-agent-solution/)
- [學員版 README](../README.md)
- [版本差異說明](version-change-notes.md)
