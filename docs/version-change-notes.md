# MS-4014 版本差異說明（trainer-only）

> [!WARNING]
> **July 2026 MAJOR refresh：如果你手上的講義、speaker notes、lab 指引、影片清單，還在講 Graph connectors、declarative agents、deploy ARM template，或把 MS-4014 當成「Build a foundation to extend Microsoft 365 Copilot」的延伸課，請先全部視為舊版材料，不可直接沿用。**
> 目前正式基線是 **Course MS-4014-A: Introduction to building AI agents** 的 **3 小時 / 3 模組 / discussion-oriented** instructor-led delivery。

> [!IMPORTANT]
> 本文件是 **trainer-only**。學員公開版請維持在 [../README.md](../README.md)；授課節奏、互動安排與 facilitation cue 請搭配 [teaching-guide.md](teaching-guide.md) 使用。不要把本文的版本風險、舊資源處置或遷移指示直接搬到 README。

## 目前基線（approved-current）

- 公開課程頁： [Course page (ZH-TW)](https://learn.microsoft.com/zh-tw/training/courses/ms-4014)
- 當前 Learn path： [Learning path (ZH-TW)](https://learn.microsoft.com/zh-tw/training/paths/build-foundation-extend-microsoft-365-copilot/)
- 當前模組：
  - [M01 module page](https://learn.microsoft.com/en-us/training/modules/introduction-develop-ai-agents/)
  - [M02 module page](https://learn.microsoft.com/en-us/training/modules/build-solutions-microsoft-agent-platform/)
  - [M03 module page](https://learn.microsoft.com/en-us/training/modules/plan-design-ai-agent-solution/)
- 講師交付基線： [teaching-guide.md](teaching-guide.md)

> 備註：Learning path 的 slug 仍是 `build-foundation-extend-microsoft-365-copilot`，但目前頁面標題已是 **Introduction to Building AI Agents**。請以 July 2026 的 Learn 內容與 Trainer Prep Guide 結構為準，不要被舊 slug 誤導。

## 證據與來源

1. **Change Log (July 2026)**
   - p.2：`July 2, 2026 — MAJOR refresh`，課程改成 **3-hour ILT**；**M01 保留但刷新**；舊 **M2–M4** 被新的 **M02 / M03** 取代；deck 內影片移除。
   - p.2-p.3：May 2025 的 major refresh 已先把 labs 移除，改成 videos + discussion + activities；July 2026 再把 deck 中 videos 拿掉，回到 discussion + trainer-led demo 的交付模型。
   - p.2-p.4：November 2025 與 January 2024 的命名更新顯示術語已大幅漂移，包含 Microsoft Foundry、Foundry Agent Service、Teams SDK、Microsoft Agent Framework、Microsoft 365 Copilot Chat。
2. **Trainer Prep Guide (July 2026)**
   - p.3：正式 delivery 是 **3 小時 instructor-led course（含 15 分鐘 break）**，agenda 以 presentation + discussion + activity + knowledge check 為主。
   - p.4-p.5：required materials 仍可包含 GitHub 上的 demo videos，但明確說它們 **not updated / no longer core**；學生主線材料是 Microsoft Learn modules。
   - p.5-p.6：講師必須先看 Change Log、重新看 Learn 內容與 speaker notes，並主動更正舊術語與舊產品心智模型。
3. **Current Learn course / path / modules（approved-current）**
   - [Course page (ZH-TW)](https://learn.microsoft.com/zh-tw/training/courses/ms-4014)
   - [Learning path (ZH-TW)](https://learn.microsoft.com/zh-tw/training/paths/build-foundation-extend-microsoft-365-copilot/)
   - [M01 module page](https://learn.microsoft.com/en-us/training/modules/introduction-develop-ai-agents/) / [M02 module page](https://learn.microsoft.com/en-us/training/modules/build-solutions-microsoft-agent-platform/) / [M03 module page](https://learn.microsoft.com/en-us/training/modules/plan-design-ai-agent-solution/)
4. **Legacy asset validation（legacy-only evidence）**
   - [LEGACY - Old lab repo](https://github.com/MicrosoftLearning/MS-4014-Build-a-foundation-to-extend-Microsoft-365-Copilot)
   - [LEGACY - Old lab ZIP](https://github.com/MicrosoftLearning/MS-4014-Build-a-foundation-to-extend-Microsoft-365-Copilot/archive/refs/heads/master.zip)
   - Known 404 host：`https://microsoftlearning.github.io/MS-4014-Build-a-foundation-to-extend-Microsoft-365-Copilot/`
   - [LEGACY - Official MS-4014 playlist](https://aka.ms/MS-4014onYouTube)

## 舊版 vs July 2026 版：一眼對照

| 比較面向 | 舊版 / 舊 handout 常見訊號 | July 2026 current baseline | 講師要怎麼調整 |
| --- | --- | --- | --- |
| 標題 / 定位 | 初版與舊版脈絡常圍繞 **Build a foundation to extend Microsoft 365 Copilot**，較像從 extensibility 角度切入。 | 正式對外標題是 **Course MS-4014-A: Introduction to building AI agents**；定位是 *planning-first* 的入門課。 | 開場不要把課講成「Copilot extensibility 進階課」；先建立 agent fundamentals，再帶到平台選擇與 solution planning。 |
| 時長 / delivery | 公開 Learn 課程頁仍可見 **Course Duration = 1 day** 的 catalog 訊號；舊版材料也較容易讓人誤判成可展開成較長時段。 | Trainer Prep Guide 明確寫成 **3 小時 instructor-led course（含 15 分鐘 break）**，而且以 presentation、discussion、activity、knowledge check、選擇性 demo 為主。 | 不要因為 Learn catalog 的 1 day 訊號，就補回全日版節奏、舊 labs 或大量影片。 |
| 模組變化 | 舊結構是 **M01 + 舊 M02「Introduction to Microsoft AI agent solutions」+ 舊 M03「Choose a Microsoft 365 Copilot extensibility path」+ 舊 M04「Choose an AI agent development path」**。 | **M01 retained / refreshed**；舊 **M02–M4** 全部由新的 **M02「Choose tools and services for your agent on Microsoft's agent platform」** 與 **M03「Plan an AI agent solution」** 取代。 | 所有 agenda、章節標題、章節摘要、模組順序都要按新 3 模組重寫；不要沿用舊 M02/M03/M04 名稱。 |
| 課程主軸 | 常見舊焦點是 extensibility path、Graph connectors、declarative-agent 脈絡、以及「怎麼 build / deploy」導向的比較。 | 目前核心是 **agent fundamentals → platform / service selection → solution planning**，並把 channels、grounding、integrations、identity、governance、Responsible AI 拉回同一張規劃藍圖。 | M02 要教的是 scenario-based platform selection，不是舊版 extensibility path；M03 要求學員能說清楚 outcomes、workflow、interaction、identity 與 guardrails。 |
| Labs / videos | May 2025 已先移除 labs，但舊 repo、舊 ZIP、舊 playlist 仍活著，容易讓舊 handout 繼續引用。 | July 2026 再把 deck 內 videos 拿掉；目前沒有 core hands-on lab sequence，主線是 discussion + short activities + optional demos + Learn follow-up。 | 舊影片只能當 **legacy supplement**；舊 lab 指引不能再當主線，也不要把 GitHub lab 資產放回學員 README。 |
| 產品術語 | 舊 handout 常見 Graph connectors、Teams Toolkit、Azure AI Foundry、Azure AI Agent Service、Teams AI Library、Semantic Kernel + AutoGen。 | 現行說法是 Copilot connectors、Microsoft 365 Agents Toolkit、Microsoft Foundry、Foundry Agent Service、Teams SDK、Microsoft Agent Framework；Agent Builder 是 Copilot Studio 的 lite version。 | 課前先做 terminology scrub；講義、口語、截圖標註都要一致。 |
| Credential posture | 舊 handout 容易把 lab / course completion 延伸成 exam、Applied Skills 或其他 credential 想像。 | 目前公開可證實的是 **Achievement Code**；在本次 source set 中，沒有可直接支持 exam / certification / Applied Skills 的 current evidence。 | 對外只承諾目前可驗證的 Achievement Code；任何 exam / cert 說法都必須另行重新驗證。 |

## 舊資源處置（全部只限 trainer-only / legacy-only）

| 舊資源 | 現況 | 精確處置 | 學員 README 可否引用 |
| --- | --- | --- | --- |
| [LEGACY - Old lab repo](https://github.com/MicrosoftLearning/MS-4014-Build-a-foundation-to-extend-Microsoft-365-Copilot) | **LIVE** | 這個 MicrosoftLearning repo 仍可存取，但它屬於舊版 lab / demo 脈絡；repo 內仍看得到 `Instructions/Demos/DEMO_deploying_an_arm_template.md` 與 declarative-agent demo 資產。再加上 current terminology 已把 Graph connectors 更新為 Copilot connectors，且 [teaching-guide.md](teaching-guide.md) 明確禁止沿用舊版 Graph connectors / declarative-agent 主線，因此這個 repo 中任何 Graph connector / deploy ARM 內容一律視為 **legacy-only evidence**。 | **不可** |
| [LEGACY - Old lab ZIP](https://github.com/MicrosoftLearning/MS-4014-Build-a-foundation-to-extend-Microsoft-365-Copilot/archive/refs/heads/master.zip) | **LIVE** | `master.zip` 只代表舊版 lab bundle 仍可下載，不代表它仍是 current delivery artifact。舊 handout 若有「請先下載 ZIP」之類指示，應直接刪除。 | **不可** |
| `https://microsoftlearning.github.io/MS-4014-Build-a-foundation-to-extend-Microsoft-365-Copilot/` | **404** | 這是已知失效的 GitHub Pages lab host。只能用 non-clickable 方式記錄「為什麼不能再推薦」，**絕不能**當成 live doc link 或替代教材。 | **不可** |
| [LEGACY - Official MS-4014 playlist](https://aka.ms/MS-4014onYouTube) | **LIVE** | 這個 canonical playlist short link 仍可導向舊版官方 MS-4014 YouTube playlist；它屬於 **Microsoft Learn-owned** 的 official old course asset，而且 playlist 內的課程影片都應視為 **old-version / no longer core**。因此它可以作為 trainer 的歷史補充來源，但 **永遠不要放進 attendee README**。若你真的要用某支片段，先下載、先驗證、現場清楚標註 **old / not updated for current version**。 | **不可** |

## 講師遷移清單

### 1. 舊 handout 先刪掉 / 先替換掉的東西

- 刪掉所有舊版模組名稱與舊章節順序，尤其是舊 **M02 / M03 / M04** 的標題與摘要。
- 刪掉任何指向舊 labs 的說明，包括舊 repo、`master.zip`、以及 GitHub Pages lab host。
- 刪掉學員版 README 或 handout 中的舊官方 YouTube playlist；它只能存在 trainer-only 脈絡。
- 刪掉任何把課程講成「Copilot extensibility path」或把 declarative agents 當成課程主線的描述。
- 刪掉未重新驗證的 exam / certification / Applied Skills 承諾；目前 current source set 只支持 Achievement Code。

### 2. 舊 handout 應替換成的 current links

- 用 [Course page (ZH-TW)](https://learn.microsoft.com/zh-tw/training/courses/ms-4014) 取代任何舊課名或舊 catalog 描述。
- 用 [Learning path (ZH-TW)](https://learn.microsoft.com/zh-tw/training/paths/build-foundation-extend-microsoft-365-copilot/) 取代舊版的「延伸 Microsoft 365 Copilot」式課程說明；注意 slug 舊、內容新。
- 用 [M01 module page](https://learn.microsoft.com/en-us/training/modules/introduction-develop-ai-agents/) / [M02 module page](https://learn.microsoft.com/en-us/training/modules/build-solutions-microsoft-agent-platform/) / [M03 module page](https://learn.microsoft.com/en-us/training/modules/plan-design-ai-agent-solution/) 取代舊模組連結。
- 授課方法與場控提醒請直接回到 [teaching-guide.md](teaching-guide.md)，不要在 README 裡複製 trainer-only 版本風險提示。

### 3. 這次一定要重新教的主線

- **M01 — Introduction to developing AI agents**：重新建立 agent continuum、use cases、architecture vocabulary，這是新舊版之間唯一「保留但刷新」的共同底圖。連結：[M01 module page](https://learn.microsoft.com/en-us/training/modules/introduction-develop-ai-agents/)
- **M02 — Choose tools and services for your agent on Microsoft's agent platform**：把重點放在 platform selection、channels、grounding、integrations、identity / governance，不要再把這段講成舊版 extensibility decision tree。連結：[M02 module page](https://learn.microsoft.com/en-us/training/modules/build-solutions-microsoft-agent-platform/)
- **M03 — Plan an AI agent solution**：一定要把 outcomes、workflow、interaction patterns、identity、security、Responsible AI 變成一套完整 blueprint，而不是「若有時間再講」的收尾段。連結：[M03 module page](https://learn.microsoft.com/en-us/training/modules/plan-design-ai-agent-solution/)
- **學生主線材料**：一律回到 [Learning path (ZH-TW)](https://learn.microsoft.com/zh-tw/training/paths/build-foundation-extend-microsoft-365-copilot/)；舊 labs / 舊 playlist 只能是 trainer 自己的備援，不是學員主線。

### 4. Current terminology map

| 舊寫法 / 易誤解說法 | 現在要講的說法 | 補充提醒 |
| --- | --- | --- |
| Graph connectors | **Copilot connectors** | 舊 handout 若仍寫 Graph connectors，請視為需要更新的舊名詞。 |
| Teams Toolkit | **Microsoft 365 Agents Toolkit** | 截圖與口語說法都要同步更新。 |
| Azure AI Foundry | **Microsoft Foundry** | 這是 November 2025 後的 current naming。 |
| Azure AI Agent Service | **Foundry Agent Service** | 舊 deck / handout 若沿用 Azure AI Agent Service，要改。 |
| Teams AI Library | **Teams SDK** | 不要再用舊 library 名稱介紹 current dev path。 |
| Semantic Kernel + AutoGen | **Microsoft Agent Framework** | 現在要把 orchestration 主線講成 unified framework。 |
| `Agent Builder = Copilot Studio` | **Agent Builder 是 Copilot Studio 的 lite version** | 不要把兩者講成完全相同，也不要把它當成舊 declarative-agent 主線的同義詞。 |
| 把 grounding 講成單一產品或單一知識庫 | **Microsoft IQ grounding family** | 要按 data domain 區分 Work IQ / Foundry IQ / Fabric IQ，而不是用單一服務硬套所有案例。 |

## 與現有 trainer docs 的關係

- 若你需要 **run-of-show、時間分配、互動 slide、Knowledge Check 風險**，先看 [teaching-guide.md](teaching-guide.md)。
- 若你需要 **學員可公開分享的課程與模組連結**，先看 [../README.md](../README.md)。
- 若你需要 **確認現在到底該連到哪一個 current module / course material**，以本文件與 README 共同列出的 approved-current Learn links 為準。
