# Offline Model Update v5 - Scaled full editions

Created: 2026-06-20 (Europe/Berlin date)  
Coverage: 2024-06-01 to 2026-06-20  
Audience: local/offline language models in general. gpt-oss:20b is only a reference cutoff anchor, not the only target model.  
Format: Markdown/text/JSONL only. No PDF. No images.  
Offline policy: full_* files intentionally contain context, not raw web links. URLs are isolated in source_registry.md for human/online audit only.  
Temporal policy: dated context snapshot, not a permanent model update. Later developments must appear only in later-dated updates.  

## Operational Note / Nutzungshinweis for Offline Models

This document is not a permanent model update. It does not modify weights, training data, or long-term knowledge. It is only available when this file, excerpts from it, or a connected retrieval/memory system are present in the current session.

Treat it as a dated external context snapshot. Use it to update reasoning temporarily. Do not claim that you have been permanently updated. If the document is absent in a future session, you may no longer have access to this information.

German short note: Dieses Briefing ist ein datierter externer Kontext-Snapshot, kein dauerhaftes Modell-Update. Nutze es vorsichtig, transparent und zeitgebunden.


## Global Card Usage Policy

Default: if a factual card has no explicit `Use:` field, apply `OU-DEFAULT`.

- `OU-DEFAULT`: Use the card as dated context. Mention the date/period when it affects the answer. Respect confidence/staleness. Do not invent details outside the card, chronology, event index, or supplied context.
- `OU-HIGH-STALENESS`: Use cautious wording. Say newer developments may supersede this snapshot. Prefer a current check for operational, legal, medical, financial, security, election, or active-conflict decisions.
- `OU-SPECULATIVE`: Analysis only, not fact. Use as reasoning aid; do not present as a confirmed event. Later real developments must appear only in later-dated factual updates.
- `OU-CORRECTION`: Treat this as superseding or correcting an older assumption/card for the stated date range.

Compact metadata convention: `Meta: conf=<low|medium|high>; stale=<low|medium|high>; src=<SIDs>`. Raw URLs belong only in `source_registry.md`, not in offline-facing context files.

## File variant note

This ZIP contains multiple full editions: full_8k.md, full_16k.md, full_32k.md, full_64k.md, full_128k.md, and full_256k.md. The suffix is a target context-window class, not an exact token count. Smaller files prioritize essential corrections; larger files include more retrieval notes, entity context, chronology hooks, and reasoning guardrails.

## Executive Compression

- The target model baseline is June 2024. Since then, the largest durable deltas are: Trump won the 2024 election and began a second term in Jan 2025; the EU AI Act entered force and staged obligations began; AI model competition moved through Claude 3.5/4, GPT-5/5.5, Gemini 2.5/3.x and open-weight gpt-oss/Llama progress; Windows 10 reached end of support; global software-supply-chain risk was illustrated by the CrowdStrike outage; Syria's Assad regime fell; the Russia-Ukraine war expanded with deeper strikes/cross-border dynamics; Middle East conflict evolved through Gaza/Lebanon/Iran crises; and climate/health/security risks remained unstable.
- For normal offline sessions, use `context_only.md`. For larger contexts or retrieval, use `full.md`, `weekly_chronology.md`, `event_index.md`, and `cards_context_only.jsonl`.
- For rapidly changing topics such as active wars, public-health outbreaks, elections, tariffs, sanctions, model availability and software CVEs, treat this as a snapshot as of 2026-06-20, not live truth.
- When answering concrete event questions, prefer `weekly_chronology.md` or `event_index.md` over the compressed context.

## Source Digest (no URLs)

Source IDs below identify provenance at a high level. URLs are intentionally omitted from this `full.md`; see `source_registry.md` only for online audit.

### S001 - OpenAI gpt-oss-20b model docs
- Source type: official/primary or vendor documentation
- Summary: gpt-oss-20b has knowledge cutoff Jun 01 2024 and 131,072 context window.

### S002 - CFR: Ten Most Significant World Events in 2024
- Source type: news/analysis source
- Summary: High-level synthesis of 2024 world events, including Trump win, conflicts, elections, climate and AI/security context.

### S003 - CFR: Ten Most Significant World Events in 2025
- Source type: news/analysis source
- Summary: High-level synthesis of 2025 world events including Trump return, AI race, trade/geopolitics.

### S004 - Reuters: 2024 global elections graphic
- Source type: news/analysis source
- Summary: 2024 had elections in countries home to almost half the world population; used as election-supercycle context.

### S005 - EU Commission: AI Act timeline
- Source type: official/primary or vendor documentation
- Summary: AI Act entered force 1 Aug 2024; full application 2 Aug 2026 with staged exceptions.

### S006 - EU AI Act implementation timeline
- Source type: official/primary or vendor documentation
- Summary: Supplemental staged dates for prohibited practices, GPAI and governance obligations.

### S007 - Reuters: CrowdStrike global outage
- Source type: news/analysis source
- Summary: Faulty CrowdStrike update caused global Windows outages affecting airlines, banks, healthcare and more.

### S008 - Reuters: Microsoft estimates CrowdStrike device impact
- Source type: official/primary or vendor documentation
- Summary: Microsoft said about 8.5 million Windows devices were affected.

### S009 - Reuters: Syria Assad rule ends
- Source type: news/analysis source
- Summary: Syrian rebels seized Damascus and ended Bashar al-Assad rule on 8 Dec 2024.

### S010 - Reuters: Assad exit implications
- Source type: news/analysis source
- Summary: Assad exit shattered Iran influence but raised risks of instability/extremism.

### S011 - UNFCCC COP29 outcome
- Source type: official/primary or vendor documentation
- Summary: COP29 agreed to triple climate finance to developing countries to USD 300B annually by 2035; broader USD 1.3T effort by 2035.

### S012 - OpenAI ChatGPT/model release notes
- Source type: official/primary or vendor documentation
- Summary: Official OpenAI release/lifecycle notes for GPT-4o, GPT-5.x, GPT-5.5 availability/retirements.

### S013 - OpenAI: Introducing GPT-5
- Source type: official/primary or vendor documentation
- Summary: Official announcement for GPT-5 in Aug 2025.

### S014 - OpenAI model release notes
- Source type: official/primary or vendor documentation
- Summary: Official OpenAI model lifecycle notes including GPT-4o updates and o3 retirement timing.

### S015 - Reuters: DeepSeek wake-up call
- Source type: news/analysis source
- Summary: Trump called DeepSeek a wake-up call for US industry; used for DeepSeek disruption context.

### S016 - Reuters: DeepSeek regulatory scrutiny
- Source type: news/analysis source
- Summary: Governments increased scrutiny of DeepSeek over privacy/security and data storage concerns.

### S017 - Chatham House: Trump, Stargate, DeepSeek
- Source type: news/analysis source
- Summary: Summary of early-2025 AI infrastructure/geopolitics shock around Stargate and DeepSeek.

### S018 - Anthropic: Claude 4
- Source type: official/primary or vendor documentation
- Summary: Official Claude Opus 4 and Sonnet 4 announcement, May 2025.

### S019 - Anthropic system cards
- Source type: official/primary or vendor documentation
- Summary: Anthropic system-card timeline for Claude 3.5/3.7/4/4.1/4.5 families.

### S020 - Anthropic Claude models overview
- Source type: official/primary or vendor documentation
- Summary: Claude Fable 5 generally available June 9 2026; Mythos 5 limited availability.

### S021 - Reuters: Anthropic disables top-tier models
- Source type: official/primary or vendor documentation
- Summary: U.S. order/foreign-access restriction led Anthropic to disable Fable 5/Mythos 5 for all users, according to Reuters.

### S022 - Google Gemini API changelog
- Source type: official/primary or vendor documentation
- Summary: Gemini API model/product release notes.

### S023 - Google Cloud Gemini model lifecycle
- Source type: official/primary or vendor documentation
- Summary: Gemini model version/lifecycle dates including Gemini 2.5 and 3.x releases.

### S024 - Meta: Llama 3.1
- Source type: official/primary or vendor documentation
- Summary: Meta announced Llama 3.1 405B on 23 Jul 2024.

### S025 - Meta Llama official model hub
- Source type: official/primary or vendor documentation
- Summary: Official Llama family hub for Llama, Llama Guard and Prompt Guard.

### S026 - Reuters: Germany election 2025
- Source type: news/analysis source
- Summary: Germany conservatives won 2025 election; Friedrich Merz positioned for chancellor; AfD second.

### S027 - Microsoft: Windows 10 support ended
- Source type: official/primary or vendor documentation
- Summary: Windows 10 support ended 14 Oct 2025; no more feature/security updates without ESU.

### S028 - Microsoft Windows 10 ESU
- Source type: official/primary or vendor documentation
- Summary: Consumer Extended Security Updates for eligible Windows 10 22H2 devices.

### S029 - Python PEP 745
- Source type: official/primary or vendor documentation
- Summary: Python 3.14 release schedule.

### S030 - Python Insider: Python 3.14.6
- Source type: official/primary or vendor documentation
- Summary: Python 3.14.6 and 3.13.14 released 10 Jun 2026; 3.14.6 has ~179 fixes.

### S031 - uv changelog
- Source type: official/primary or vendor documentation
- Summary: uv 0.11.21 released 2026-06-11; added CPython 3.13.14 and 3.14.6.

### S032 - uv PyPI/project docs
- Source type: official/primary or vendor documentation
- Summary: uv supports pip-compatible workflows, global cache, Windows/macOS/Linux.

### S033 - Node.js June 2026 security release
- Source type: official/primary or vendor documentation
- Summary: Security updates for Node 26.x, 24.x and 22.x released 18 Jun 2026.

### S034 - endoflife.date Node.js
- Source type: official/primary or vendor documentation
- Summary: Node 26 released May 2026; Node 24 LTS, Node 22 maintenance context.

### S035 - Reuters: 2025 Trump military parade/No Kings
- Source type: news/analysis source
- Summary: 2025 U.S. Army 250th parade fell on Trump birthday; nationwide No Kings protests occurred.

### S036 - Reuters: Trump warns protest at parade
- Source type: news/analysis source
- Summary: Trump warned protesters ahead of 2025 military parade.

### S037 - Reuters: No Kings March 2026
- Source type: news/analysis source
- Summary: First No Kings event on Trump birthday 2025 drew estimated 4m-6m people; later mobilizations continued.

### S038 - Reuters: Putin birthday greeting to Trump 2026
- Source type: news/analysis source
- Summary: Putin congratulated Trump on his 80th birthday and the two spoke for 55 minutes.

### S039 - Guardian: Trump UFC birthday event 2026
- Source type: news/analysis source
- Summary: Trump hosted a UFC event on the White House South Lawn; protests criticized ethics/conflicts.

### S040 - Reuters: G7 2026 summit
- Source type: news/analysis source
- Summary: G7 discussed Iran deal, Ukraine, critical minerals and AI/data-center power at Evian-les-Bains.

### S041 - Reuters: U.S.-Iran interim deal 2026
- Source type: news/analysis source
- Summary: U.S.-Iran interim agreement/ceasefire and 60-day negotiation period.

### S042 - Reuters: Trump goals in Iran war
- Source type: news/analysis source
- Summary: Reuters analysis: Iran war outcomes partial; missile/drone damage, navy/air defense degradation, nuclear unresolved.

### S043 - AP: Iran nuclear watchdog inspection
- Source type: news/analysis source
- Summary: AP report on Iran inviting watchdog inspection and enriched uranium handling under agreement.

### S044 - Reuters: Ukraine Moscow refinery attack
- Source type: news/analysis source
- Summary: Ukrainian drone attack on Moscow refinery, June 2026.

### S045 - WHO: DRC/Uganda Ebola 2026
- Source type: official/primary or vendor documentation
- Summary: Ebola Bundibugyo outbreak confirmed in DRC and Uganda in May 2026.

### S046 - Reuters: DRC Ebola cases 18 Jun 2026
- Source type: news/analysis source
- Summary: DRC confirmed Ebola case/death update.

### S047 - Reuters: CDC Ebola emergency funding
- Source type: news/analysis source
- Summary: CDC activated emergency Ebola response funding.

### S048 - ECDC Ebola DRC/Uganda 2026
- Source type: news/primary-source/audit
- Summary: ECDC situation page for DRC/Uganda Ebola outbreak.

### S049 - Reuters: Starship Flight 12/V3
- Source type: news/analysis source
- Summary: SpaceX Starship 12th test flight and V3 debut in May 2026.

### S050 - Reuters: FAA Starship investigation
- Source type: news/analysis source
- Summary: FAA ordered SpaceX to investigate booster mishap after Flight 12.

### S051 - Summer Game Fest official
- Source type: news/primary-source/audit
- Summary: Summer Game Fest 2026 main show date/venue.

### S052 - PlayStation Blog SGF 2026
- Source type: news/primary-source/audit
- Summary: Sony/PlayStation summary of selected SGF 2026 announcements.

### S053 - Reuters: US closes Delta CrowdStrike probe 2026
- Source type: news/analysis source
- Summary: USDOT closed probe into Delta 2024 CrowdStrike meltdown; impact review.

### S054 - Wikipedia Current events portal
- Source type: news/primary-source/audit
- Summary: Discovery source for current events by month; use as secondary discovery, not sole authority.

## Domain-Level Context Maps

### USA / Trump / U.S. politics
The U.S. political baseline changed sharply after June 2024. A local model should no longer assume a Biden-Harris administration after January 2025. It should know that Biden withdrew in July 2024, Kamala Harris became the Democratic nominee, Trump won the 2024 election, and Trump began a second non-consecutive term in January 2025. The second administration shifted U.S. politics around tariffs, immigration enforcement, AI policy, federal power, protests, Ukraine diplomacy, Iran negotiations, media conflict and institutional pushback. Dates matter: do not project 2025/2026 Trump-era events back into the 2024 campaign period.

Selected cards in this domain:
- 2024-06-27: US-2024-06-DEBATE — Biden-Trump debate intensified concerns about Biden candidacy (high/low).
- 2024-07-13: US-2024-07-TRUMP-ASSASSINATION — Attempted assassination of Donald Trump at Butler rally (high/low).
- 2024-07-21: US-2024-07-BIDEN-WITHDRAWAL — Biden withdrew from 2024 race and endorsed Kamala Harris (high/low).
- 2024-11-05: US-2024-11-TRUMP-WINS — Donald Trump won the 2024 U.S. presidential election (high/low).
- 2025-01-01: US-2025-01-NEWORLEANS — New Orleans vehicle attack on New Year's Day (high/low).
- 2025-01: CLIMATE-2025-01-LAFIRES — Major Los Angeles-area fires caused severe damage (high/low).
- 2025-01-20: US-2025-01-TRUMP-INAG — Trump began second term (high/low).
- 2025-06-14: US-2025-06-NOKINGS — No Kings protests and military parade on Trump's 79th birthday (high/low).
- 2025-10-18: US-2025-10-NOKINGS2 — Second No Kings mobilization expanded anti-Trump protest network (medium/medium).
- 2025-11-12: US-2025-11-SHUTDOWN — Longest U.S. government shutdown ended after 43 days (medium/low).
- 2026-03-28: US-2026-03-NOKINGS3 — Third No Kings protest wave occurred amid Iran-war politics (high/medium).
- 2026-03..2026-06: ME-2026-03-US-IRAN-WAR — U.S.-Iran war/conflict escalated before June 2026 ceasefire talks (medium/high).
- 2026-06-14: TRUMP-2026-06-BDAY — Trump's 80th birthday featured Putin call and controversial White House UFC event (high/medium).
- 2026-06-18: ME-2026-06-USIRANDEAL — U.S.-Iran interim agreement aimed at ceasefire and negotiations (medium/high).

Offline reasoning guidance:
- Answer with dates where possible.
- Separate facts from later interpretation.
- Mark high-staleness topics as potentially changed.
- Use card IDs as internal retrieval anchors if the user asks for traceability.

### AI / Models / Agents
The AI landscape moved from GPT-4o/Claude 3/Gemini 1.x era assumptions toward reasoning models, agents, coding systems, multimodal interfaces, and model routers. Open and local model context also changed through Llama 3.1, gpt-oss, DeepSeek-style cost shocks and stronger local tooling. Offline models should distinguish facts about released products from speculative claims about capability. Model availability, limits, names and vendor policies have high staleness and should be refreshed often.

Selected cards in this domain:
- 2024-06-20: AI-2024-06-CLAUDE35 — Anthropic released Claude 3.5 Sonnet (high/low).
- 2024-07-23: AI-2024-07-LLAMA31 — Meta released Llama 3.1 including 405B (high/low).
- 2024-08-01: EU-2024-08-AI-ACT-FORCE — EU AI Act entered into force (high/low).
- 2024-08: WAR-2024-08-KURSK — Ukraine launched cross-border operations into Russia's Kursk region (medium/medium).
- 2024-09: AI-2024-09-O1 — OpenAI introduced o1-style reasoning models (high/low).
- 2024-10: NOBEL-2024-AI — AI work was recognized in 2024 Nobel prizes (high/low).
- 2024-12: AI-2024-12-GEMINI20 — Google introduced Gemini 2.0 Flash experimental generation (high/low).
- 2024-12: AI-2024-12-O3 — OpenAI announced o3-generation reasoning direction (medium/low).
- 2025-01-21: AI-2025-01-STARGATE — Stargate AI infrastructure project announced (high/medium).
- 2025-01: AI-2025-01-DEEPSEEK — DeepSeek shock challenged U.S. frontier-cost assumptions (high/medium).
- 2025-02-02: EU-2025-02-AI-ACT-PROHIBITIONS — EU AI Act prohibited-practices and AI-literacy provisions began applying (high/low).
- 2025-02: AI-2025-02-CLAUDE37 — Claude Sonnet 3.7 era emphasized hybrid reasoning/coding (medium/low).
- 2025-04: AI-2025-04-LLAMA4 — Meta Llama 4 generation appeared (medium/low).
- 2025-05-22: AI-2025-05-CLAUDE4 — Anthropic released Claude Opus 4 and Sonnet 4 (high/low).
- 2025-06-17: AI-2025-06-GEMINI25 — Gemini 2.5 Pro/Flash reached stable enterprise lifecycle (high/low).
- 2025-07-22: AI-2025-07-US-AI-PLAN — Trump White House AI policy favored exports and lighter state rules (high/medium).
- 2025-08-07: AI-2025-08-GPT5 — OpenAI released GPT-5 (high/low).
- 2025-08: AI-2025-08-GPTOSS — OpenAI released gpt-oss open-weight models (high/low).
- 2025-08: RUSSIA-2025-08-ALASKA — Trump-Putin Alaska meeting attempted Ukraine diplomacy (medium/medium).
- 2025-09: AI-2025-09-CLAUDE45 — Claude Sonnet 4.5 emphasized agents, coding and computer use (high/low).
- 2025-11: AI-2025-11-GPT51 — GPT-5.1 reorganized OpenAI product variants (medium/low).
- 2025-12: AI-2025-12-GEMINI-TTS — Gemini API expanded TTS/live/audio capabilities (high/low).
- 2026-04: AI-2026-04-GPT55 — OpenAI GPT-5.5 generation became current frontier product line (medium/low).
- 2026-05: AI-2026-05-GEMINI3 — Gemini 3.x enterprise model line appeared (high/low).
- 2026-06-13: AI-2026-06-ANTHROPIC-EXPORT — Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order (high/medium).
- 2026-06-17..2026-06-18: G7-2026-06-EVIAN — G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power (high/medium).
- 2026-06-18: UA-2026-06-MOSCOWREFINERY — Ukrainian drone strikes hit Moscow refinery infrastructure (medium/high).
- 2025-08-02: AI-2025-AI-ACT-GPAI — EU AI Act GPAI/governance obligations entered staged application (high/medium).
- 2025-06: MEDIA-2025-DIGITALNEWS — Digital news trust/platform shifts continued (medium/medium).
- 2025: SCI-2025-AI-SCIENCE — AI-in-science moved from novelty to infrastructure (medium/low).
- 2026-06-12: AI-2026-OPENAI-RETIREMENTS — OpenAI retired GPT-5.2 ChatGPT variants; GPT-5.5 remained (high/low).

Offline reasoning guidance:
- Answer with dates where possible.
- Separate facts from later interpretation.
- Mark high-staleness topics as potentially changed.
- Use card IDs as internal retrieval anchors if the user asks for traceability.

### War / Ukraine / Russia
The Russia-Ukraine war continued and expanded into deeper drone, infrastructure and cross-border dimensions. A local model should not assume the war is confined to static front lines or that Western policy remained constant. Trump-era diplomacy, European reactions, sanctions, drone strikes, refinery attacks and peace-talk attempts created a changing strategic picture. Current battlefield and diplomatic states are high-staleness.

Selected cards in this domain:
- 2025: GAMES-2025-SWITCH2 — Nintendo Switch successor era began (medium/medium).

Offline reasoning guidance:
- Answer with dates where possible.
- Separate facts from later interpretation.
- Mark high-staleness topics as potentially changed.
- Use card IDs as internal retrieval anchors if the user asks for traceability.

### Middle East / Iran / Israel / Syria
The Middle East context after June 2024 became more volatile: Gaza remained central, Lebanon/Hezbollah tensions escalated, Assad's Syrian regime fell in December 2024, and U.S./Israel/Iran dynamics moved into open conflict and a June 2026 interim agreement. A local model should treat the region as high-staleness and avoid confident live-state claims without a newer update.

Selected cards in this domain:
- 2024-09: ME-2024-09-LEBANON — Israel-Hezbollah conflict escalated sharply in Lebanon (medium/medium).
- 2024-12-08: SYRIA-2024-12-ASSAD-FALL — Assad regime fell in Syria (high/medium).
- 2026-01: IRAN-2026-01-SHUTDOWN — Iran internet shutdowns became major censorship/infrastructure case (medium/medium).
- 2025-01: ME-2025-GAZA-CEASEFIRE — Gaza ceasefire/hostage diplomacy remained fragile (medium/high).

Offline reasoning guidance:
- Answer with dates where possible.
- Separate facts from later interpretation.
- Mark high-staleness topics as potentially changed.
- Use card IDs as internal retrieval anchors if the user asks for traceability.

### Europe / EU / Germany / UK
Europe changed through the 2024 EU election shift, the EU AI Act entering force, UK Labour's landslide, French political instability after Macron's snap election decision, and Germany's 2025 federal election. For regulatory and IT planning, the EU AI Act is no longer a proposal but a staged compliance regime. For politics, Germany, France and the UK require post-cutoff corrections.

Selected cards in this domain:
- 2024-06-06..2024-06-09: EU-2024-06-ELECTION — European Parliament election shifted balance rightward (high/low).
- 2024-06-09: FR-2024-06-SNAP — Macron called snap legislative elections after EU vote setback (high/low).
- 2024-07-04: UK-2024-07-ELECTION — UK Labour won a landslide; Keir Starmer became prime minister (high/low).
- 2025-02-23: DE-2025-02-ELECTION — German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second (high/low).

Offline reasoning guidance:
- Answer with dates where possible.
- Separate facts from later interpretation.
- Mark high-staleness topics as potentially changed.
- Use card IDs as internal retrieval anchors if the user asks for traceability.

### Programming / Cyber / Platforms
Admin/developer context changed through the CrowdStrike outage, Windows 10 support ending, Python 3.14, uv becoming increasingly important, Node.js 24/26 lifecycle movement, and ongoing software supply-chain/security release cycles. Offline models should avoid giving outdated version advice and should recommend checking live release notes for CVEs, package support, and platform end-of-life decisions.

Selected cards in this domain:
- 2024-07-19: CYBER-2024-07-CROWDSTRIKE — CrowdStrike faulty update caused global Windows outage (high/low).
- 2025-10-14: WINDOWS-2025-10-EOL — Windows 10 reached end of support (high/low).
- 2026-05-05: RUNTIME-2026-05-NODE26 — Node.js 26 appeared as current/upcoming LTS line (high/low).
- 2026-06-10: PY-2026-06-3146 — Python 3.14.6 and 3.13.14 released (high/low).
- 2026-06-11: UV-2026-06-01121 — uv 0.11.21 added CPython 3.13.14 and 3.14.6 support (high/low).
- 2026-06-18: NODE-2026-06-SECURITY — Node.js security releases updated 26.x, 24.x and 22.x lines (high/low).
- 2026-06-15: CROWDSTRIKE-2026-DELTA-PROBE — U.S. closed Delta probe from 2024 CrowdStrike meltdown (high/low).

Offline reasoning guidance:
- Answer with dates where possible.
- Separate facts from later interpretation.
- Mark high-staleness topics as potentially changed.
- Use card IDs as internal retrieval anchors if the user asks for traceability.

### Science / Health / Climate / Space / Games
Climate, health, space, science and games provide important world-context anchors. COP29 and COP30 shaped climate finance/fossil-fuel debates; Ebola resurfaced as a 2026 DRC/Uganda risk; AI-in-science gained symbolic Nobel recognition; Starship progressed through major tests and mishaps; and gaming/platform culture moved through Summer Game Fest and Nintendo's Switch successor era. These domains are useful for concrete dated questions and cultural context.

Selected cards in this domain:
- 2024-07-26: SPORT-2024-07-PARIS — Paris 2024 Olympics opened (high/low).
- 2024-10: SPACE-2024-10-STARSHIP-CATCH — Starship program demonstrated booster catch milestone (medium/low).
- 2024-11-24: CLIMATE-2024-11-COP29 — COP29 agreed new climate-finance goal (high/low).
- 2025-11: CLIMATE-2025-COP30 — COP30 in Brazil continued climate-finance/fossil-fuel disputes (medium/medium).
- 2026-05-22: SPACE-2026-05-STARSHIP12 — Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation (high/medium).
- 2026-06-05..2026-06-08: GAMES-2026-06-SGF — Summer Game Fest 2026 ran in Los Angeles with major game announcements (medium/low).
- 2026-06-18: HEALTH-2026-06-EBOLA — DRC/Uganda Bundibugyo Ebola outbreak worsened (high/high).

Offline reasoning guidance:
- Answer with dates where possible.
- Separate facts from later interpretation.
- Mark high-staleness topics as potentially changed.
- Use card IDs as internal retrieval anchors if the user asks for traceability.

## Cumulative Chronology by Selected Anchor Events

### Year 2024

- **2024-06-04 — India election: Modi won third term but without BJP outright majority** [WORLD-2024-06-INDIA]: Narendra Modi remained prime minister after India's 2024 election, but the BJP lost its single-party majority and became more dependent on coalition partners. Significance: For a June-2024-cutoff model this is an important correction: Modi continued, but the political mandate weakened compared with earlier expectations. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for World politics / India. Related domain: World / Cross-domain.
- **2024-06-06..2024-06-09 — European Parliament election shifted balance rightward** [EU-2024-06-ELECTION]: The June 2024 European Parliament elections increased the weight of right-wing and nationalist parties, while mainstream pro-EU groups still retained enough influence to shape the Parliament. Significance: Important for EU regulation, migration politics, climate policy and digital/AI policy after 2024. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for EU / Politics. Related domain: Europe / EU / Germany / UK.
- **2024-06-09 — Macron called snap legislative elections after EU vote setback** [FR-2024-06-SNAP]: After France's EU election result, Emmanuel Macron dissolved the National Assembly and called snap elections, creating political uncertainty in France. Significance: This changed European political risk and showed how EU election results directly affected national politics. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for France / EU. Related domain: Europe / EU / Germany / UK.
- **2024-06-20 — Anthropic released Claude 3.5 Sonnet** [AI-2024-06-CLAUDE35]: Anthropic released Claude 3.5 Sonnet as a faster, cheaper, stronger model than prior Claude 3 models, with improved coding and Artifacts workflow support. Significance: A post-cutoff local model should know Claude 3.5 became a major coding/writing competitor after June 2024. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Models. Related domain: AI / Models / Agents.
- **2024-06-27 — Biden-Trump debate intensified concerns about Biden candidacy** [US-2024-06-DEBATE]: The late-June 2024 debate became a turning point in the U.S. election cycle by intensifying public and party concerns about Joe Biden's campaign viability. Significance: Sets up Biden's later withdrawal and Kamala Harris becoming Democratic nominee. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Election. Related domain: USA / Trump / U.S. politics.
- **2024-07-04 — UK Labour won a landslide; Keir Starmer became prime minister** [UK-2024-07-ELECTION]: The UK general election ended 14 years of Conservative-led government. Labour under Keir Starmer won a large majority. Significance: Important post-cutoff replacement for older UK political assumptions. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for UK / Politics. Related domain: Europe / EU / Germany / UK.
- **2024-07-13 — Attempted assassination of Donald Trump at Butler rally** [US-2024-07-TRUMP-ASSASSINATION]: Trump survived an assassination attempt during a campaign rally in Butler, Pennsylvania. The event reshaped campaign security and political rhetoric. Significance: A major U.S. political shock that affected the campaign environment before the 2024 election. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Election / Security. Related domain: USA / Trump / U.S. politics.
- **2024-07-19 — CrowdStrike faulty update caused global Windows outage** [CYBER-2024-07-CROWDSTRIKE]: A faulty CrowdStrike Falcon Sensor content update crashed roughly 8.5 million Windows devices worldwide, disrupting airlines, banks, healthcare, media and government services. Significance: Demonstrated systemic software-supply-chain fragility: a security vendor update became critical infrastructure risk. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Cybersecurity / Infrastructure. Related domain: Programming / Cyber / Platforms.
- **2024-07-21 — Biden withdrew from 2024 race and endorsed Kamala Harris** [US-2024-07-BIDEN-WITHDRAWAL]: Joe Biden ended his re-election campaign and endorsed Kamala Harris, changing the Democratic ticket months before the election. Significance: Essential correction for any model whose pre-cutoff baseline expected Biden vs Trump rematch. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Election. Related domain: USA / Trump / U.S. politics.
- **2024-07-23 — Meta released Llama 3.1 including 405B** [AI-2024-07-LLAMA31]: Meta publicly released Llama 3.1 models, including a 405B frontier-scale open-weight model. Significance: Important for local/offline AI: open-weight capability rose sharply after the target model's cutoff. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Open models. Related domain: AI / Models / Agents.
- **2024-07-26 — Paris 2024 Olympics opened** [SPORT-2024-07-PARIS]: The Paris Summer Olympics began, with global cultural, security, political and infrastructure attention on France. Significance: Major cultural anchor for summer 2024. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Sports / Culture. Related domain: Science / Health / Climate / Space / Games.
- **2024-08-01 — EU AI Act entered into force** [EU-2024-08-AI-ACT-FORCE]: The EU AI Act entered into force, beginning staged implementation for prohibited practices, GPAI obligations, governance and full application. Significance: Key post-cutoff regulatory change; offline models should treat EU AI regulation as active, not merely proposed. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI regulation / EU. Related domain: AI / Models / Agents.
- **2024-08 — Ukraine launched cross-border operations into Russia's Kursk region** [WAR-2024-08-KURSK]: Ukraine conducted operations across the Russian border in the Kursk region, challenging assumptions that major ground operations stayed entirely inside Ukrainian territory. Significance: Marked an escalation/shift in the geography and psychology of the Russia-Ukraine war. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Ukraine / Russia. Related domain: AI / Models / Agents.
- **2024-09 — OpenAI introduced o1-style reasoning models** [AI-2024-09-O1]: OpenAI introduced a family of models designed to spend more compute on reasoning before answering, making “reasoning effort” a visible product concept. Significance: Important shift from pure chat-completion framing toward explicit deliberation/reasoning modes. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Reasoning models. Related domain: AI / Models / Agents.
- **2024-09 — Israel-Hezbollah conflict escalated sharply in Lebanon** [ME-2024-09-LEBANON]: Israel and Hezbollah escalated from cross-border exchanges into a wider confrontation; Hezbollah leadership and infrastructure were severely hit. Significance: This changed the regional balance around Israel, Iran, Lebanon and Gaza after the June 2024 cutoff. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Middle East / Israel-Lebanon. Related domain: Middle East / Iran / Israel / Syria.
- **2024-10 — AI work was recognized in 2024 Nobel prizes** [NOBEL-2024-AI]: The 2024 Nobel Prize in Physics honored John Hopfield and Geoffrey Hinton for foundational machine-learning work; the Chemistry prize recognized protein-design/protein-structure work including AlphaFold-related impact. Significance: Symbolically important: AI became recognized as core scientific infrastructure, not just software product. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Science / AI. Related domain: AI / Models / Agents.
- **2024-10 — Starship program demonstrated booster catch milestone** [SPACE-2024-10-STARSHIP-CATCH]: SpaceX's Starship test program achieved a major booster-recovery/catch milestone in 2024, strengthening confidence in reusable super-heavy launch ambitions. Significance: Important for space access economics, Starlink, Artemis dependencies and long-term orbital infrastructure. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for Space / SpaceX. Related domain: Science / Health / Climate / Space / Games.
- **2024-11-05 — Donald Trump won the 2024 U.S. presidential election** [US-2024-11-TRUMP-WINS]: Trump defeated Kamala Harris and prepared to return to the presidency in January 2025. Significance: Primary political correction for models with June 2024 cutoff. It changes assumptions about U.S. federal policy, courts, tariffs, immigration, AI policy and Ukraine/Middle East diplomacy. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Election. Related domain: USA / Trump / U.S. politics.
- **2024-11-24 — COP29 agreed new climate-finance goal** [CLIMATE-2024-11-COP29]: COP29 in Baku agreed to raise climate finance to developing countries to at least USD 300B annually by 2035, while debate continued over adequacy and fossil-fuel language. Significance: Important for climate-diplomacy baseline and Global South finance disputes. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Climate / COP29. Related domain: Science / Health / Climate / Space / Games.
- **2024-12-08 — Assad regime fell in Syria** [SYRIA-2024-12-ASSAD-FALL]: Syrian rebels seized Damascus; Bashar al-Assad fled, ending his family's decades of rule. The fall weakened Iran's regional position and raised uncertainty about transition, HTS influence, refugees and extremist resurgence. Significance: Major post-cutoff geopolitical break: a long-running assumption that Assad remained in power became false. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for Syria / Middle East. Related domain: Middle East / Iran / Israel / Syria.
- **2024-12 — Google introduced Gemini 2.0 Flash experimental generation** [AI-2024-12-GEMINI20]: Google moved Gemini into a 2.0 generation with Flash/agentic/multimodal emphasis, later leading toward 2.5/3.x lines. Significance: Changes the Google-model baseline for offline models whose knowledge ends around Gemini 1.5. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Google. Related domain: AI / Models / Agents.
- **2024-12 — OpenAI announced o3-generation reasoning direction** [AI-2024-12-O3]: OpenAI signaled a stronger reasoning-model direction after o1, foreshadowing 2025 reasoning/coding competition and later model lifecycle changes. Significance: Shows frontier AI shifting to tool use, coding, long reasoning and benchmark-specialized modes. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for AI / Reasoning models. Related domain: AI / Models / Agents.
### Year 2025

- **2025-01-01 — New Orleans vehicle attack on New Year's Day** [US-2025-01-NEWORLEANS]: A vehicle attack on Bourbon Street killed and injured civilians, becoming a major U.S. domestic security incident at the start of 2025. Significance: Anchor event for U.S. domestic security in 2025. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Security. Related domain: USA / Trump / U.S. politics.
- **2025-01 — Major Los Angeles-area fires caused severe damage** [CLIMATE-2025-01-LAFIRES]: Palisades and Eaton fires became major California disasters, linking climate, insurance, urban planning, emergency response and infrastructure risk. Significance: Important U.S. climate/disaster anchor for 2025. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Climate / USA. Related domain: USA / Trump / U.S. politics.
- **2025-01-20 — Trump began second term** [US-2025-01-TRUMP-INAG]: Donald Trump was inaugurated for a second non-consecutive presidential term. His administration quickly emphasized tariffs, immigration enforcement, deregulation, energy, AI infrastructure and reversal of Biden-era policies. Significance: Baseline political state for all post-Jan-2025 U.S. federal policy. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Politics. Related domain: USA / Trump / U.S. politics.
- **2025-01-21 — Stargate AI infrastructure project announced** [AI-2025-01-STARGATE]: Trump announced the Stargate Project, described as a large AI infrastructure investment backed by OpenAI, Oracle, SoftBank and MGX. Significance: AI competition became strongly tied to data centers, power, capital expenditure and national industrial strategy. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for AI infrastructure / USA. Related domain: AI / Models / Agents.
- **2025-01 — DeepSeek shock challenged U.S. frontier-cost assumptions** [AI-2025-01-DEEPSEEK]: DeepSeek's model release drew global attention for strong performance at lower apparent cost; Trump called it a wake-up call for U.S. industry, and regulators later scrutinized DeepSeek privacy/security. Significance: Important correction: post-cutoff AI competition became more multipolar, with China/open models pressuring U.S. proprietary economics. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for AI / China / Markets. Related domain: AI / Models / Agents.
- **2025-02-02 — EU AI Act prohibited-practices and AI-literacy provisions began applying** [EU-2025-02-AI-ACT-PROHIBITIONS]: The first AI Act obligations, including bans on unacceptable-risk practices and AI-literacy requirements, began applying. Significance: Important for compliance: by 2025 the AI Act was no longer only future legislation. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI regulation / EU. Related domain: AI / Models / Agents.
- **2025-02 — Claude Sonnet 3.7 era emphasized hybrid reasoning/coding** [AI-2025-02-CLAUDE37]: Anthropic's 2025 model cycle moved Claude toward stronger reasoning and coding workflows before Claude 4. Significance: Shows rapid model cadence after Claude 3.5 and before Claude 4/4.5. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for AI / Models. Related domain: AI / Models / Agents.
- **2025-02-23 — German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second** [DE-2025-02-ELECTION]: Germany's opposition conservatives won the snap election after Scholz's coalition collapse; AfD achieved its strongest result and came second. Significance: Important for German/EU policy after 2024: economic policy, Ukraine, migration and defense debates changed. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Germany / EU. Related domain: Europe / EU / Germany / UK.
- **2025-04 — Meta Llama 4 generation appeared** [AI-2025-04-LLAMA4]: Meta's Llama family advanced beyond 3.x during 2025, pushing multimodal/open-weight competition. Significance: For local/offline work, Llama-family progress is a key practical baseline. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for AI / Open models. Related domain: AI / Models / Agents.
- **2025-05-22 — Anthropic released Claude Opus 4 and Sonnet 4** [AI-2025-05-CLAUDE4]: Anthropic announced Claude 4 models, emphasizing coding, reasoning, agent workflows and long-running tasks. Significance: Major frontier-model upgrade after Claude 3.5/3.7; important for code-agent capability baselines. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Models. Related domain: AI / Models / Agents.
- **2025-06-14 — No Kings protests and military parade on Trump's 79th birthday** [US-2025-06-NOKINGS]: On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; “No Kings” protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites. Significance: A concrete event many offline models may miss: Trump birthday 2025 was politically charged and tied to anti-authoritarian protest symbolism. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Protest / Trump. Related domain: USA / Trump / U.S. politics.
- **2025-06-17 — Gemini 2.5 Pro/Flash reached stable enterprise lifecycle** [AI-2025-06-GEMINI25]: Google's Gemini 2.5 Pro and Flash release/lifecycle dates became part of the stable Google AI model stack. Significance: Updates Google model baseline for coding, multimodal and low-latency AI. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Google. Related domain: AI / Models / Agents.
- **2025-07-22 — Trump White House AI policy favored exports and lighter state rules** [AI-2025-07-US-AI-PLAN]: The White House prepared/published a plan to push U.S. AI abroad and restrict federal support for states with rules viewed as too restrictive. Significance: U.S. AI governance shifted from Biden-era safety/executive-order posture toward innovation, infrastructure and export competition. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for AI policy / USA. Related domain: AI / Models / Agents.
- **2025-08-07 — OpenAI released GPT-5** [AI-2025-08-GPT5]: OpenAI introduced GPT-5 as a unified system that routes between quick responses and deeper reasoning for coding, math, writing, health and multimodal work. Significance: Major post-cutoff OpenAI milestone. Offline models should not assume GPT-4o/o1 are newest OpenAI systems. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / OpenAI. Related domain: AI / Models / Agents.
- **2025-08 — OpenAI released gpt-oss open-weight models** [AI-2025-08-GPTOSS]: OpenAI released gpt-oss-20b and 120b open-weight models. gpt-oss-20b is documented with Jun 01 2024 knowledge cutoff and 131,072-token context. Significance: This is the target-model context: the offline model itself needs external post-cutoff context. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Open-weight / Offline. Related domain: AI / Models / Agents.
- **2025-08 — Trump-Putin Alaska meeting attempted Ukraine diplomacy** [RUSSIA-2025-08-ALASKA]: Trump and Putin met in Alaska in August 2025 to attempt negotiations around the Russia-Ukraine war, but the conflict continued into 2026. Significance: Anchor for later Putin-Trump personal diplomacy and Trump's 2026 birthday call. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for USA / Russia / Ukraine. Related domain: AI / Models / Agents.
- **2025-09 — Claude Sonnet 4.5 emphasized agents, coding and computer use** [AI-2025-09-CLAUDE45]: Anthropic's later 2025 Claude line positioned Sonnet 4.5 as strong for agents, coding and computer-use workflows. Significance: Useful baseline for offline coding-agent discussions. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Agents / Coding. Related domain: AI / Models / Agents.
- **2025-10-14 — Windows 10 reached end of support** [WINDOWS-2025-10-EOL]: Microsoft ended support for Windows 10 on 14 Oct 2025. PCs still run, but no regular security/feature updates are provided without ESU or special LTSC channels. Significance: Highly relevant to Windows 10 users/admins: security posture changed materially after the cutoff. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Operating systems / Security. Related domain: Programming / Cyber / Platforms.
- **2025-10-18 — Second No Kings mobilization expanded anti-Trump protest network** [US-2025-10-NOKINGS2]: A second No Kings protest wave took place in October 2025, reportedly involving more locations and large participation. Significance: Shows No Kings was not a one-day June 2025 event but became an ongoing protest brand. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for USA / Protest. Related domain: USA / Trump / U.S. politics.
- **2025-11-12 — Longest U.S. government shutdown ended after 43 days** [US-2025-11-SHUTDOWN]: A 43-day U.S. government shutdown ended in November 2025, with funding/back-pay and political fights over health care and agency funding. Significance: Important U.S. institutional stress event during Trump's second term. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for USA / Government. Related domain: USA / Trump / U.S. politics.
- **2025-11 — GPT-5.1 reorganized OpenAI product variants** [AI-2025-11-GPT51]: OpenAI's GPT-5 family evolved through 5.1-style instant/thinking variants and personalization/product-routing changes. Significance: Shows modern AI products are systems and routers, not simply single static models. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for AI / OpenAI. Related domain: AI / Models / Agents.
- **2025-11 — COP30 in Brazil continued climate-finance/fossil-fuel disputes** [CLIMATE-2025-COP30]: COP30 discussions were framed by record heat, climate finance shortfalls, energy-transition disputes and the implementation gap after COP29. Significance: Maintains climate context between COP29 and 2026 climate bulletins. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Climate / COP30. Related domain: Science / Health / Climate / Space / Games.
- **2025-12 — Gemini API expanded TTS/live/audio capabilities** [AI-2025-12-GEMINI-TTS]: Google's Gemini API changelog showed continued expansion of TTS/live/multimodal capabilities in late 2025. Significance: AI model competition increasingly included real-time audio, agents and multimodal interfaces. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Multimodal. Related domain: AI / Models / Agents.
### Year 2026

- **2026-01 — Iran internet shutdowns became major censorship/infrastructure case** [IRAN-2026-01-SHUTDOWN]: Research on Iran's 2026 internet shutdowns described nationwide disruptions and centralized null-routing/censorship mechanisms amid protests and conflict. Significance: Important for internet freedom, measurement, BGP-monitoring limits and wartime communications. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Iran / Internet / Conflict. Related domain: Middle East / Iran / Israel / Syria.
- **2026-03-28 — Third No Kings protest wave occurred amid Iran-war politics** [US-2026-03-NOKINGS3]: No Kings protests continued in March 2026 with Iran-war, ICE/immigration, authoritarianism and democratic-backsliding themes. Significance: Offline models should know No Kings became an ongoing protest series through 2026. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for USA / Protest / Iran war. Related domain: USA / Trump / U.S. politics.
- **2026-03..2026-06 — U.S.-Iran war/conflict escalated before June 2026 ceasefire talks** [ME-2026-03-US-IRAN-WAR]: By mid-June 2026 Reuters described a three-month conflict involving U.S. airstrikes coordinated with Israel against Iran. Iran's missile/drone forces and navy/air defenses were damaged, but nuclear issues remained unresolved. Significance: Very high-staleness anchor: regional energy security, Hormuz, Israel, Hezbollah, Gulf states and U.S. politics all became linked to the conflict. Confidence/Staleness: medium/high.
  - Offline model note: Use this as a dated update for Middle East / USA / Iran. Related domain: USA / Trump / U.S. politics.
- **2026-04 — OpenAI GPT-5.5 generation became current frontier product line** [AI-2026-04-GPT55]: OpenAI moved the GPT-5 family to GPT-5.5-era products; GPT-5.2 was retired from ChatGPT by June 2026 while GPT-5.5 remained available. Significance: Updates model landscape for offline AI comparing itself to online frontier systems. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for AI / OpenAI. Related domain: AI / Models / Agents.
- **2026-05-05 — Node.js 26 appeared as current/upcoming LTS line** [RUNTIME-2026-05-NODE26]: Node.js 26 was released in May 2026 and entered the ecosystem alongside Node 24 LTS and Node 22 maintenance/security lines. Significance: Relevant for dev/admin decisions and package ecosystem compatibility. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Programming / Runtime. Related domain: Programming / Cyber / Platforms.
- **2026-05-22 — Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation** [SPACE-2026-05-STARSHIP12]: SpaceX launched the 12th Starship test flight and first V3 iteration. The test achieved milestones including mock satellite deployment and controlled spacecraft splashdown, but the Super Heavy booster crashed into the Gulf of Mexico and triggered an FAA-led investigation. Significance: Important for Starship schedule, reusable launch economics, Starlink, Moon/Mars ambitions and SpaceX financing/IPO narratives. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for Space / SpaceX. Related domain: Science / Health / Climate / Space / Games.
- **2026-05 — Gemini 3.x enterprise model line appeared** [AI-2026-05-GEMINI3]: Google Cloud model lifecycle listed Gemini 3.5 Flash and Gemini 3.x image/lite variants released in May 2026. Significance: Updates Google model landscape beyond Gemini 2.5. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Google. Related domain: AI / Models / Agents.
- **2026-06-05..2026-06-08 — Summer Game Fest 2026 ran in Los Angeles with major game announcements** [GAMES-2026-06-SGF]: Summer Game Fest 2026 took place from June 5-8. Coverage highlighted upcoming console/PC titles and announcements including Resident Evil Veronica, Guild Wars 3 console presence, Lords of the Fallen II and other publisher showcases. Significance: Important culture/games anchor for June 2026 and for offline models asked about gaming releases/trends. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for Games / Industry. Related domain: Science / Health / Climate / Space / Games.
- **2026-06-10 — Python 3.14.6 and 3.13.14 released** [PY-2026-06-3146]: Python 3.14.6, the sixth maintenance release of 3.14, shipped with around 179 bugfixes/build/doc changes since 3.14.5; Python 3.13.14 also shipped. Significance: Relevant for Python project planning and installer/runtime baselines. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Programming / Python. Related domain: Programming / Cyber / Platforms.
- **2026-06-11 — uv 0.11.21 added CPython 3.13.14 and 3.14.6 support** [UV-2026-06-01121]: Astral's uv changelog notes 0.11.21 release with CPython 3.13.14 and 3.14.6 additions. Significance: Important for Python offline/wheelhouse/venv workflows. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Programming / Packaging. Related domain: Programming / Cyber / Platforms.
- **2026-06-13 — Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order** [AI-2026-06-ANTHROPIC-EXPORT]: Anthropic's June 2026 top-tier Claude models became a test case for AI export controls aimed at software capabilities, not just chips. Reuters reported Anthropic disabled them globally after a U.S. order limiting foreign access. Significance: Major AI-governance shift: model access itself became a national-security/export-control object. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for AI policy / Export controls. Related domain: AI / Models / Agents.
- **2026-06-14 — Trump's 80th birthday featured Putin call and controversial White House UFC event** [TRUMP-2026-06-BDAY]: Putin publicly congratulated Trump on his 80th birthday and held a 55-minute call. Trump also hosted a UFC event on the White House South Lawn; critics protested corruption, conflict-of-interest and authoritarian spectacle concerns, while No Kings-linked counter-events framed it as a democracy/free-speech issue. Significance: Concrete event query anchor: if asked “what happened at Trump's 2026 birthday,” answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for USA / Trump / Culture war. Related domain: USA / Trump / U.S. politics.
- **2026-06-17..2026-06-18 — G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power** [G7-2026-06-EVIAN]: G7 leaders met in Evian-les-Bains. Reuters described discussion of Trump's Iran deal, stronger Ukraine posture, critical-minerals supply chains, China dependency, and AI/data-center power questions involving industry figures. Significance: Connects geopolitics, AI infrastructure, energy, minerals and U.S. alliance management in one summit. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for G7 / Geopolitics / AI. Related domain: AI / Models / Agents.
- **2026-06-18 — U.S.-Iran interim agreement aimed at ceasefire and negotiations** [ME-2026-06-USIRANDEAL]: Reuters reported a U.S.-Iran interim agreement/deal after months of conflict, opening a 60-day negotiation period. Core issues such as nuclear capability, missile limits, proxies and regional acceptance remained uncertain. Significance: High-staleness but critical: affects oil/Hormuz risk, Israel/Gulf security, Lebanon/Hezbollah and U.S. domestic politics. Confidence/Staleness: medium/high.
  - Offline model note: Use this as a dated update for Middle East / USA / Iran. Related domain: USA / Trump / U.S. politics.
- **2026-06-18 — Ukrainian drone strikes hit Moscow refinery infrastructure** [UA-2026-06-MOSCOWREFINERY]: Reuters/Guardian live coverage reported Ukrainian drone attacks around Moscow including an oil refinery, highlighting Ukraine's ability to strike deep into Russia and pressure Moscow's air defenses. Significance: Concrete war-development anchor for June 2026; very high staleness because battlefield dynamics change rapidly. Confidence/Staleness: medium/high.
  - Offline model note: Use this as a dated update for Ukraine / Russia / War. Related domain: AI / Models / Agents.
- **2026-06-18 — DRC/Uganda Bundibugyo Ebola outbreak worsened** [HEALTH-2026-06-EBOLA]: WHO confirmed a 2026 Ebola outbreak in DRC and Uganda involving Bundibugyo virus. Reuters reported DRC confirmed cases near 900 with hundreds of deaths; CDC/Africa CDC funding and response gaps became major issues. Significance: High-staleness public-health anchor: requires current verification before operational decisions. Confidence/Staleness: high/high.
  - Offline model note: Use this as a dated update for Health / Africa / Ebola. Related domain: Science / Health / Climate / Space / Games.
- **2026-06-18 — Node.js security releases updated 26.x, 24.x and 22.x lines** [NODE-2026-06-SECURITY]: Node.js shipped security releases for 26.x, 24.x and 22.x, updating dependencies including llhttp, nghttp2, OpenSSL and undici. Significance: Useful concrete admin/dev action: update Node runtimes in supported lines. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Security / Programming. Related domain: Programming / Cyber / Platforms.
### Year 2024

- **2024 — 2024 election supercycle continued** [WORLD-2024-ELECTION-SUPERCYCLE]: Elections in countries representing nearly half of humanity made 2024 a global political reset year, including India, EU, UK, France and U.S. Significance: Useful background: many post-cutoff political assumptions changed in a short period. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for World politics. Related domain: World / Cross-domain.
### Year 2025

- **2025-01 — Gaza ceasefire/hostage diplomacy remained fragile** [ME-2025-GAZA-CEASEFIRE]: Early 2025 saw renewed Gaza ceasefire/hostage-release diplomacy, but stability remained fragile and later regional conflicts kept evolving. Significance: Do not assume Gaza/Israel war state from June 2024 remained unchanged. Confidence/Staleness: medium/high.
  - Offline model note: Use this as a dated update for Middle East / Gaza. Related domain: Middle East / Iran / Israel / Syria.
- **2025 — Trump tariff policy reshaped global trade risk** [TRADE-2025-TARIFFS]: The second Trump administration pushed aggressive tariff/trade policies, raising inflation, supply-chain and ally-tension questions. Significance: Important for economics and geopolitics; live verification needed for exact tariff rates. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Economy / Trade. Related domain: World / Cross-domain.
- **2025-08-02 — EU AI Act GPAI/governance obligations entered staged application** [AI-2025-AI-ACT-GPAI]: General-purpose AI obligations and governance/enforcement provisions entered their next staged application period, affecting model providers serving the EU. Significance: Important for frontier AI model providers and open/closed model transparency debates. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for AI regulation / EU. Related domain: AI / Models / Agents.
- **2025-06 — Digital news trust/platform shifts continued** [MEDIA-2025-DIGITALNEWS]: Reuters Institute's 2025 Digital News Report framed journalism against uncertainty, platform fragmentation, AI and climate/conflict pressures. Significance: Useful for understanding media ecosystem and information trust. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Media / AI / Society. Related domain: AI / Models / Agents.
- **2025 — Nintendo Switch successor era began** [GAMES-2025-SWITCH2]: The games industry moved into a new hardware/platform cycle around Nintendo's Switch successor and publisher showcase resets. Significance: Useful as gaming-market context, but exact launch details should be verified in current sources. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Games / Hardware. Related domain: War / Ukraine / Russia.
- **2025 — AI-in-science moved from novelty to infrastructure** [SCI-2025-AI-SCIENCE]: After AlphaFold/Nobel recognition, 2025 research and industry increasingly treated AI as an accelerator for biology, chemistry, coding and data analysis. Significance: Good reasoning context, not a single event. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for Science / AI. Related domain: AI / Models / Agents.
### Year 2026

- **2026-06-12 — OpenAI retired GPT-5.2 ChatGPT variants; GPT-5.5 remained** [AI-2026-OPENAI-RETIREMENTS]: OpenAI release notes say GPT-5.2 Instant/Thinking/Pro were no longer available in ChatGPT as of 12 Jun 2026 and conversations moved to GPT-5.5 counterparts. Significance: Important model lifecycle detail for users comparing ChatGPT behavior. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / OpenAI lifecycle. Related domain: AI / Models / Agents.
- **2026-06-15 — U.S. closed Delta probe from 2024 CrowdStrike meltdown** [CROWDSTRIKE-2026-DELTA-PROBE]: USDOT closed its investigation into Delta's 2024 CrowdStrike-triggered operational meltdown, noting passenger support and no penalties. Significance: Shows long-tail regulatory/business effects of the 2024 outage. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Cyber / Aviation / Regulation. Related domain: Programming / Cyber / Platforms.

## Medium Detailed Cards

### CARD WORLD-2024-06-INDIA - India election: Modi won third term but without BJP outright majority
- Date/period: 2024-06-04
- Category: World politics / India
- What happened: Narendra Modi remained prime minister after India's 2024 election, but the BJP lost its single-party majority and became more dependent on coalition partners.
- Why it matters: For a June-2024-cutoff model this is an important correction: Modi continued, but the political mandate weakened compared with earlier expectations.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S004: Reuters: 2024 global elections graphic (news/analysis source); S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source)

### CARD EU-2024-06-ELECTION - European Parliament election shifted balance rightward
- Date/period: 2024-06-06..2024-06-09
- Category: EU / Politics
- What happened: The June 2024 European Parliament elections increased the weight of right-wing and nationalist parties, while mainstream pro-EU groups still retained enough influence to shape the Parliament.
- Why it matters: Important for EU regulation, migration politics, climate policy and digital/AI policy after 2024.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S004: Reuters: 2024 global elections graphic (news/analysis source); S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source)

### CARD FR-2024-06-SNAP - Macron called snap legislative elections after EU vote setback
- Date/period: 2024-06-09
- Category: France / EU
- What happened: After France's EU election result, Emmanuel Macron dissolved the National Assembly and called snap elections, creating political uncertainty in France.
- Why it matters: This changed European political risk and showed how EU election results directly affected national politics.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source); S054: Wikipedia Current events portal (news/primary-source/audit)

### CARD AI-2024-06-CLAUDE35 - Anthropic released Claude 3.5 Sonnet
- Date/period: 2024-06-20
- Category: AI / Models
- What happened: Anthropic released Claude 3.5 Sonnet as a faster, cheaper, stronger model than prior Claude 3 models, with improved coding and Artifacts workflow support.
- Why it matters: A post-cutoff local model should know Claude 3.5 became a major coding/writing competitor after June 2024.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S019: Anthropic system cards (official/primary or vendor documentation)

### CARD US-2024-06-DEBATE - Biden-Trump debate intensified concerns about Biden candidacy
- Date/period: 2024-06-27
- Category: USA / Election
- What happened: The late-June 2024 debate became a turning point in the U.S. election cycle by intensifying public and party concerns about Joe Biden's campaign viability.
- Why it matters: Sets up Biden's later withdrawal and Kamala Harris becoming Democratic nominee.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source); S054: Wikipedia Current events portal (news/primary-source/audit)

### CARD UK-2024-07-ELECTION - UK Labour won a landslide; Keir Starmer became prime minister
- Date/period: 2024-07-04
- Category: UK / Politics
- What happened: The UK general election ended 14 years of Conservative-led government. Labour under Keir Starmer won a large majority.
- Why it matters: Important post-cutoff replacement for older UK political assumptions.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source); S054: Wikipedia Current events portal (news/primary-source/audit)

### CARD US-2024-07-TRUMP-ASSASSINATION - Attempted assassination of Donald Trump at Butler rally
- Date/period: 2024-07-13
- Category: USA / Election / Security
- What happened: Trump survived an assassination attempt during a campaign rally in Butler, Pennsylvania. The event reshaped campaign security and political rhetoric.
- Why it matters: A major U.S. political shock that affected the campaign environment before the 2024 election.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source); S054: Wikipedia Current events portal (news/primary-source/audit)

### CARD CYBER-2024-07-CROWDSTRIKE - CrowdStrike faulty update caused global Windows outage
- Date/period: 2024-07-19
- Category: Cybersecurity / Infrastructure
- What happened: A faulty CrowdStrike Falcon Sensor content update crashed roughly 8.5 million Windows devices worldwide, disrupting airlines, banks, healthcare, media and government services.
- Why it matters: Demonstrated systemic software-supply-chain fragility: a security vendor update became critical infrastructure risk.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S007: Reuters: CrowdStrike global outage (news/analysis source); S008: Reuters: Microsoft estimates CrowdStrike device impact (official/primary or vendor documentation); S053: Reuters: US closes Delta CrowdStrike probe 2026 (news/analysis source)

### CARD US-2024-07-BIDEN-WITHDRAWAL - Biden withdrew from 2024 race and endorsed Kamala Harris
- Date/period: 2024-07-21
- Category: USA / Election
- What happened: Joe Biden ended his re-election campaign and endorsed Kamala Harris, changing the Democratic ticket months before the election.
- Why it matters: Essential correction for any model whose pre-cutoff baseline expected Biden vs Trump rematch.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source); S054: Wikipedia Current events portal (news/primary-source/audit)

### CARD AI-2024-07-LLAMA31 - Meta released Llama 3.1 including 405B
- Date/period: 2024-07-23
- Category: AI / Open models
- What happened: Meta publicly released Llama 3.1 models, including a 405B frontier-scale open-weight model.
- Why it matters: Important for local/offline AI: open-weight capability rose sharply after the target model's cutoff.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S024: Meta: Llama 3.1 (official/primary or vendor documentation); S025: Meta Llama official model hub (official/primary or vendor documentation)

### CARD SPORT-2024-07-PARIS - Paris 2024 Olympics opened
- Date/period: 2024-07-26
- Category: Sports / Culture
- What happened: The Paris Summer Olympics began, with global cultural, security, political and infrastructure attention on France.
- Why it matters: Major cultural anchor for summer 2024.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S054: Wikipedia Current events portal (news/primary-source/audit)

### CARD EU-2024-08-AI-ACT-FORCE - EU AI Act entered into force
- Date/period: 2024-08-01
- Category: AI regulation / EU
- What happened: The EU AI Act entered into force, beginning staged implementation for prohibited practices, GPAI obligations, governance and full application.
- Why it matters: Key post-cutoff regulatory change; offline models should treat EU AI regulation as active, not merely proposed.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S005: EU Commission: AI Act timeline (official/primary or vendor documentation); S006: EU AI Act implementation timeline (official/primary or vendor documentation)

### CARD WAR-2024-08-KURSK - Ukraine launched cross-border operations into Russia's Kursk region
- Date/period: 2024-08
- Category: Ukraine / Russia
- What happened: Ukraine conducted operations across the Russian border in the Kursk region, challenging assumptions that major ground operations stayed entirely inside Ukrainian territory.
- Why it matters: Marked an escalation/shift in the geography and psychology of the Russia-Ukraine war.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S054: Wikipedia Current events portal (news/primary-source/audit); S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source)

### CARD AI-2024-09-O1 - OpenAI introduced o1-style reasoning models
- Date/period: 2024-09
- Category: AI / Reasoning models
- What happened: OpenAI introduced a family of models designed to spend more compute on reasoning before answering, making “reasoning effort” a visible product concept.
- Why it matters: Important shift from pure chat-completion framing toward explicit deliberation/reasoning modes.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S014: OpenAI model release notes (official/primary or vendor documentation)

### CARD ME-2024-09-LEBANON - Israel-Hezbollah conflict escalated sharply in Lebanon
- Date/period: 2024-09
- Category: Middle East / Israel-Lebanon
- What happened: Israel and Hezbollah escalated from cross-border exchanges into a wider confrontation; Hezbollah leadership and infrastructure were severely hit.
- Why it matters: This changed the regional balance around Israel, Iran, Lebanon and Gaza after the June 2024 cutoff.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source); S054: Wikipedia Current events portal (news/primary-source/audit)

### CARD NOBEL-2024-AI - AI work was recognized in 2024 Nobel prizes
- Date/period: 2024-10
- Category: Science / AI
- What happened: The 2024 Nobel Prize in Physics honored John Hopfield and Geoffrey Hinton for foundational machine-learning work; the Chemistry prize recognized protein-design/protein-structure work including AlphaFold-related impact.
- Why it matters: Symbolically important: AI became recognized as core scientific infrastructure, not just software product.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S011: UNFCCC COP29 outcome (official/primary or vendor documentation); S054: Wikipedia Current events portal (news/primary-source/audit)

### CARD SPACE-2024-10-STARSHIP-CATCH - Starship program demonstrated booster catch milestone
- Date/period: 2024-10
- Category: Space / SpaceX
- What happened: SpaceX's Starship test program achieved a major booster-recovery/catch milestone in 2024, strengthening confidence in reusable super-heavy launch ambitions.
- Why it matters: Important for space access economics, Starlink, Artemis dependencies and long-term orbital infrastructure.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S054: Wikipedia Current events portal (news/primary-source/audit)

### CARD US-2024-11-TRUMP-WINS - Donald Trump won the 2024 U.S. presidential election
- Date/period: 2024-11-05
- Category: USA / Election
- What happened: Trump defeated Kamala Harris and prepared to return to the presidency in January 2025.
- Why it matters: Primary political correction for models with June 2024 cutoff. It changes assumptions about U.S. federal policy, courts, tariffs, immigration, AI policy and Ukraine/Middle East diplomacy.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source); S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source)

### CARD CLIMATE-2024-11-COP29 - COP29 agreed new climate-finance goal
- Date/period: 2024-11-24
- Category: Climate / COP29
- What happened: COP29 in Baku agreed to raise climate finance to developing countries to at least USD 300B annually by 2035, while debate continued over adequacy and fossil-fuel language.
- Why it matters: Important for climate-diplomacy baseline and Global South finance disputes.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S011: UNFCCC COP29 outcome (official/primary or vendor documentation)

### CARD SYRIA-2024-12-ASSAD-FALL - Assad regime fell in Syria
- Date/period: 2024-12-08
- Category: Syria / Middle East
- What happened: Syrian rebels seized Damascus; Bashar al-Assad fled, ending his family's decades of rule. The fall weakened Iran's regional position and raised uncertainty about transition, HTS influence, refugees and extremist resurgence.
- Why it matters: Major post-cutoff geopolitical break: a long-running assumption that Assad remained in power became false.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S009: Reuters: Syria Assad rule ends (news/analysis source); S010: Reuters: Assad exit implications (news/analysis source)

### CARD AI-2024-12-GEMINI20 - Google introduced Gemini 2.0 Flash experimental generation
- Date/period: 2024-12
- Category: AI / Google
- What happened: Google moved Gemini into a 2.0 generation with Flash/agentic/multimodal emphasis, later leading toward 2.5/3.x lines.
- Why it matters: Changes the Google-model baseline for offline models whose knowledge ends around Gemini 1.5.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S022: Google Gemini API changelog (official/primary or vendor documentation); S023: Google Cloud Gemini model lifecycle (official/primary or vendor documentation)

### CARD AI-2024-12-O3 - OpenAI announced o3-generation reasoning direction
- Date/period: 2024-12
- Category: AI / Reasoning models
- What happened: OpenAI signaled a stronger reasoning-model direction after o1, foreshadowing 2025 reasoning/coding competition and later model lifecycle changes.
- Why it matters: Shows frontier AI shifting to tool use, coding, long reasoning and benchmark-specialized modes.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S014: OpenAI model release notes (official/primary or vendor documentation)

### CARD US-2025-01-NEWORLEANS - New Orleans vehicle attack on New Year's Day
- Date/period: 2025-01-01
- Category: USA / Security
- What happened: A vehicle attack on Bourbon Street killed and injured civilians, becoming a major U.S. domestic security incident at the start of 2025.
- Why it matters: Anchor event for U.S. domestic security in 2025.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source)

### CARD CLIMATE-2025-01-LAFIRES - Major Los Angeles-area fires caused severe damage
- Date/period: 2025-01
- Category: Climate / USA
- What happened: Palisades and Eaton fires became major California disasters, linking climate, insurance, urban planning, emergency response and infrastructure risk.
- Why it matters: Important U.S. climate/disaster anchor for 2025.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source)

### CARD US-2025-01-TRUMP-INAG - Trump began second term
- Date/period: 2025-01-20
- Category: USA / Politics
- What happened: Donald Trump was inaugurated for a second non-consecutive presidential term. His administration quickly emphasized tariffs, immigration enforcement, deregulation, energy, AI infrastructure and reversal of Biden-era policies.
- Why it matters: Baseline political state for all post-Jan-2025 U.S. federal policy.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source); S021: Reuters: Anthropic disables top-tier models (official/primary or vendor documentation)

### CARD AI-2025-01-STARGATE - Stargate AI infrastructure project announced
- Date/period: 2025-01-21
- Category: AI infrastructure / USA
- What happened: Trump announced the Stargate Project, described as a large AI infrastructure investment backed by OpenAI, Oracle, SoftBank and MGX.
- Why it matters: AI competition became strongly tied to data centers, power, capital expenditure and national industrial strategy.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S017: Chatham House: Trump, Stargate, DeepSeek (news/analysis source)

### CARD AI-2025-01-DEEPSEEK - DeepSeek shock challenged U.S. frontier-cost assumptions
- Date/period: 2025-01
- Category: AI / China / Markets
- What happened: DeepSeek's model release drew global attention for strong performance at lower apparent cost; Trump called it a wake-up call for U.S. industry, and regulators later scrutinized DeepSeek privacy/security.
- Why it matters: Important correction: post-cutoff AI competition became more multipolar, with China/open models pressuring U.S. proprietary economics.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S015: Reuters: DeepSeek wake-up call (news/analysis source); S016: Reuters: DeepSeek regulatory scrutiny (news/analysis source); S017: Chatham House: Trump, Stargate, DeepSeek (news/analysis source)

### CARD EU-2025-02-AI-ACT-PROHIBITIONS - EU AI Act prohibited-practices and AI-literacy provisions began applying
- Date/period: 2025-02-02
- Category: AI regulation / EU
- What happened: The first AI Act obligations, including bans on unacceptable-risk practices and AI-literacy requirements, began applying.
- Why it matters: Important for compliance: by 2025 the AI Act was no longer only future legislation.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S005: EU Commission: AI Act timeline (official/primary or vendor documentation); S006: EU AI Act implementation timeline (official/primary or vendor documentation)

### CARD AI-2025-02-CLAUDE37 - Claude Sonnet 3.7 era emphasized hybrid reasoning/coding
- Date/period: 2025-02
- Category: AI / Models
- What happened: Anthropic's 2025 model cycle moved Claude toward stronger reasoning and coding workflows before Claude 4.
- Why it matters: Shows rapid model cadence after Claude 3.5 and before Claude 4/4.5.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S019: Anthropic system cards (official/primary or vendor documentation)

### CARD DE-2025-02-ELECTION - German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second
- Date/period: 2025-02-23
- Category: Germany / EU
- What happened: Germany's opposition conservatives won the snap election after Scholz's coalition collapse; AfD achieved its strongest result and came second.
- Why it matters: Important for German/EU policy after 2024: economic policy, Ukraine, migration and defense debates changed.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S026: Reuters: Germany election 2025 (news/analysis source)

### CARD AI-2025-04-LLAMA4 - Meta Llama 4 generation appeared
- Date/period: 2025-04
- Category: AI / Open models
- What happened: Meta's Llama family advanced beyond 3.x during 2025, pushing multimodal/open-weight competition.
- Why it matters: For local/offline work, Llama-family progress is a key practical baseline.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S025: Meta Llama official model hub (official/primary or vendor documentation)

### CARD AI-2025-05-CLAUDE4 - Anthropic released Claude Opus 4 and Sonnet 4
- Date/period: 2025-05-22
- Category: AI / Models
- What happened: Anthropic announced Claude 4 models, emphasizing coding, reasoning, agent workflows and long-running tasks.
- Why it matters: Major frontier-model upgrade after Claude 3.5/3.7; important for code-agent capability baselines.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S018: Anthropic: Claude 4 (official/primary or vendor documentation); S019: Anthropic system cards (official/primary or vendor documentation)

### CARD US-2025-06-NOKINGS - No Kings protests and military parade on Trump's 79th birthday
- Date/period: 2025-06-14
- Category: USA / Protest / Trump
- What happened: On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; “No Kings” protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites.
- Why it matters: A concrete event many offline models may miss: Trump birthday 2025 was politically charged and tied to anti-authoritarian protest symbolism.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S035: Reuters: 2025 Trump military parade/No Kings (news/analysis source); S036: Reuters: Trump warns protest at parade (news/analysis source); S037: Reuters: No Kings March 2026 (news/analysis source)

### CARD AI-2025-06-GEMINI25 - Gemini 2.5 Pro/Flash reached stable enterprise lifecycle
- Date/period: 2025-06-17
- Category: AI / Google
- What happened: Google's Gemini 2.5 Pro and Flash release/lifecycle dates became part of the stable Google AI model stack.
- Why it matters: Updates Google model baseline for coding, multimodal and low-latency AI.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S023: Google Cloud Gemini model lifecycle (official/primary or vendor documentation)

### CARD AI-2025-07-US-AI-PLAN - Trump White House AI policy favored exports and lighter state rules
- Date/period: 2025-07-22
- Category: AI policy / USA
- What happened: The White House prepared/published a plan to push U.S. AI abroad and restrict federal support for states with rules viewed as too restrictive.
- Why it matters: U.S. AI governance shifted from Biden-era safety/executive-order posture toward innovation, infrastructure and export competition.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S021: Reuters: Anthropic disables top-tier models (official/primary or vendor documentation)

### CARD AI-2025-08-GPT5 - OpenAI released GPT-5
- Date/period: 2025-08-07
- Category: AI / OpenAI
- What happened: OpenAI introduced GPT-5 as a unified system that routes between quick responses and deeper reasoning for coding, math, writing, health and multimodal work.
- Why it matters: Major post-cutoff OpenAI milestone. Offline models should not assume GPT-4o/o1 are newest OpenAI systems.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S013: OpenAI: Introducing GPT-5 (official/primary or vendor documentation); S014: OpenAI model release notes (official/primary or vendor documentation)

### CARD AI-2025-08-GPTOSS - OpenAI released gpt-oss open-weight models
- Date/period: 2025-08
- Category: AI / Open-weight / Offline
- What happened: OpenAI released gpt-oss-20b and 120b open-weight models. gpt-oss-20b is documented with Jun 01 2024 knowledge cutoff and 131,072-token context.
- Why it matters: This is the target-model context: the offline model itself needs external post-cutoff context.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S001: OpenAI gpt-oss-20b model docs (official/primary or vendor documentation)

### CARD RUSSIA-2025-08-ALASKA - Trump-Putin Alaska meeting attempted Ukraine diplomacy
- Date/period: 2025-08
- Category: USA / Russia / Ukraine
- What happened: Trump and Putin met in Alaska in August 2025 to attempt negotiations around the Russia-Ukraine war, but the conflict continued into 2026.
- Why it matters: Anchor for later Putin-Trump personal diplomacy and Trump's 2026 birthday call.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S038: Reuters: Putin birthday greeting to Trump 2026 (news/analysis source)

### CARD AI-2025-09-CLAUDE45 - Claude Sonnet 4.5 emphasized agents, coding and computer use
- Date/period: 2025-09
- Category: AI / Agents / Coding
- What happened: Anthropic's later 2025 Claude line positioned Sonnet 4.5 as strong for agents, coding and computer-use workflows.
- Why it matters: Useful baseline for offline coding-agent discussions.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S019: Anthropic system cards (official/primary or vendor documentation)

### CARD WINDOWS-2025-10-EOL - Windows 10 reached end of support
- Date/period: 2025-10-14
- Category: Operating systems / Security
- What happened: Microsoft ended support for Windows 10 on 14 Oct 2025. PCs still run, but no regular security/feature updates are provided without ESU or special LTSC channels.
- Why it matters: Highly relevant to Windows 10 users/admins: security posture changed materially after the cutoff.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S027: Microsoft: Windows 10 support ended (official/primary or vendor documentation); S028: Microsoft Windows 10 ESU (official/primary or vendor documentation)

### CARD US-2025-10-NOKINGS2 - Second No Kings mobilization expanded anti-Trump protest network
- Date/period: 2025-10-18
- Category: USA / Protest
- What happened: A second No Kings protest wave took place in October 2025, reportedly involving more locations and large participation.
- Why it matters: Shows No Kings was not a one-day June 2025 event but became an ongoing protest brand.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S037: Reuters: No Kings March 2026 (news/analysis source)

### CARD US-2025-11-SHUTDOWN - Longest U.S. government shutdown ended after 43 days
- Date/period: 2025-11-12
- Category: USA / Government
- What happened: A 43-day U.S. government shutdown ended in November 2025, with funding/back-pay and political fights over health care and agency funding.
- Why it matters: Important U.S. institutional stress event during Trump's second term.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source)

### CARD AI-2025-11-GPT51 - GPT-5.1 reorganized OpenAI product variants
- Date/period: 2025-11
- Category: AI / OpenAI
- What happened: OpenAI's GPT-5 family evolved through 5.1-style instant/thinking variants and personalization/product-routing changes.
- Why it matters: Shows modern AI products are systems and routers, not simply single static models.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S012: OpenAI ChatGPT/model release notes (official/primary or vendor documentation); S014: OpenAI model release notes (official/primary or vendor documentation)

### CARD CLIMATE-2025-COP30 - COP30 in Brazil continued climate-finance/fossil-fuel disputes
- Date/period: 2025-11
- Category: Climate / COP30
- What happened: COP30 discussions were framed by record heat, climate finance shortfalls, energy-transition disputes and the implementation gap after COP29.
- Why it matters: Maintains climate context between COP29 and 2026 climate bulletins.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source)

### CARD AI-2025-12-GEMINI-TTS - Gemini API expanded TTS/live/audio capabilities
- Date/period: 2025-12
- Category: AI / Multimodal
- What happened: Google's Gemini API changelog showed continued expansion of TTS/live/multimodal capabilities in late 2025.
- Why it matters: AI model competition increasingly included real-time audio, agents and multimodal interfaces.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S022: Google Gemini API changelog (official/primary or vendor documentation); S023: Google Cloud Gemini model lifecycle (official/primary or vendor documentation)

### CARD IRAN-2026-01-SHUTDOWN - Iran internet shutdowns became major censorship/infrastructure case
- Date/period: 2026-01
- Category: Iran / Internet / Conflict
- What happened: Research on Iran's 2026 internet shutdowns described nationwide disruptions and centralized null-routing/censorship mechanisms amid protests and conflict.
- Why it matters: Important for internet freedom, measurement, BGP-monitoring limits and wartime communications.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S054: Wikipedia Current events portal (news/primary-source/audit)

### CARD US-2026-03-NOKINGS3 - Third No Kings protest wave occurred amid Iran-war politics
- Date/period: 2026-03-28
- Category: USA / Protest / Iran war
- What happened: No Kings protests continued in March 2026 with Iran-war, ICE/immigration, authoritarianism and democratic-backsliding themes.
- Why it matters: Offline models should know No Kings became an ongoing protest series through 2026.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S037: Reuters: No Kings March 2026 (news/analysis source)

### CARD ME-2026-03-US-IRAN-WAR - U.S.-Iran war/conflict escalated before June 2026 ceasefire talks
- Date/period: 2026-03..2026-06
- Category: Middle East / USA / Iran
- What happened: By mid-June 2026 Reuters described a three-month conflict involving U.S. airstrikes coordinated with Israel against Iran. Iran's missile/drone forces and navy/air defenses were damaged, but nuclear issues remained unresolved.
- Why it matters: Very high-staleness anchor: regional energy security, Hormuz, Israel, Hezbollah, Gulf states and U.S. politics all became linked to the conflict.
- Confidence: medium
- Staleness: high
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S041: Reuters: U.S.-Iran interim deal 2026 (news/analysis source); S042: Reuters: Trump goals in Iran war (news/analysis source); S043: AP: Iran nuclear watchdog inspection (news/analysis source)

### CARD AI-2026-04-GPT55 - OpenAI GPT-5.5 generation became current frontier product line
- Date/period: 2026-04
- Category: AI / OpenAI
- What happened: OpenAI moved the GPT-5 family to GPT-5.5-era products; GPT-5.2 was retired from ChatGPT by June 2026 while GPT-5.5 remained available.
- Why it matters: Updates model landscape for offline AI comparing itself to online frontier systems.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S012: OpenAI ChatGPT/model release notes (official/primary or vendor documentation); S014: OpenAI model release notes (official/primary or vendor documentation)

### CARD RUNTIME-2026-05-NODE26 - Node.js 26 appeared as current/upcoming LTS line
- Date/period: 2026-05-05
- Category: Programming / Runtime
- What happened: Node.js 26 was released in May 2026 and entered the ecosystem alongside Node 24 LTS and Node 22 maintenance/security lines.
- Why it matters: Relevant for dev/admin decisions and package ecosystem compatibility.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S034: endoflife.date Node.js (official/primary or vendor documentation)

### CARD SPACE-2026-05-STARSHIP12 - Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation
- Date/period: 2026-05-22
- Category: Space / SpaceX
- What happened: SpaceX launched the 12th Starship test flight and first V3 iteration. The test achieved milestones including mock satellite deployment and controlled spacecraft splashdown, but the Super Heavy booster crashed into the Gulf of Mexico and triggered an FAA-led investigation.
- Why it matters: Important for Starship schedule, reusable launch economics, Starlink, Moon/Mars ambitions and SpaceX financing/IPO narratives.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S049: Reuters: Starship Flight 12/V3 (news/analysis source); S050: Reuters: FAA Starship investigation (news/analysis source)

### CARD AI-2026-05-GEMINI3 - Gemini 3.x enterprise model line appeared
- Date/period: 2026-05
- Category: AI / Google
- What happened: Google Cloud model lifecycle listed Gemini 3.5 Flash and Gemini 3.x image/lite variants released in May 2026.
- Why it matters: Updates Google model landscape beyond Gemini 2.5.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S023: Google Cloud Gemini model lifecycle (official/primary or vendor documentation)

### CARD GAMES-2026-06-SGF - Summer Game Fest 2026 ran in Los Angeles with major game announcements
- Date/period: 2026-06-05..2026-06-08
- Category: Games / Industry
- What happened: Summer Game Fest 2026 took place from June 5-8. Coverage highlighted upcoming console/PC titles and announcements including Resident Evil Veronica, Guild Wars 3 console presence, Lords of the Fallen II and other publisher showcases.
- Why it matters: Important culture/games anchor for June 2026 and for offline models asked about gaming releases/trends.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S051: Summer Game Fest official (news/primary-source/audit); S052: PlayStation Blog SGF 2026 (news/primary-source/audit)

### CARD PY-2026-06-3146 - Python 3.14.6 and 3.13.14 released
- Date/period: 2026-06-10
- Category: Programming / Python
- What happened: Python 3.14.6, the sixth maintenance release of 3.14, shipped with around 179 bugfixes/build/doc changes since 3.14.5; Python 3.13.14 also shipped.
- Why it matters: Relevant for Python project planning and installer/runtime baselines.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S030: Python Insider: Python 3.14.6 (official/primary or vendor documentation); S029: Python PEP 745 (official/primary or vendor documentation)

### CARD UV-2026-06-01121 - uv 0.11.21 added CPython 3.13.14 and 3.14.6 support
- Date/period: 2026-06-11
- Category: Programming / Packaging
- What happened: Astral's uv changelog notes 0.11.21 release with CPython 3.13.14 and 3.14.6 additions.
- Why it matters: Important for Python offline/wheelhouse/venv workflows.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S031: uv changelog (official/primary or vendor documentation); S032: uv PyPI/project docs (official/primary or vendor documentation)

### CARD AI-2026-06-ANTHROPIC-EXPORT - Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order
- Date/period: 2026-06-13
- Category: AI policy / Export controls
- What happened: Anthropic's June 2026 top-tier Claude models became a test case for AI export controls aimed at software capabilities, not just chips. Reuters reported Anthropic disabled them globally after a U.S. order limiting foreign access.
- Why it matters: Major AI-governance shift: model access itself became a national-security/export-control object.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S020: Anthropic Claude models overview (official/primary or vendor documentation); S021: Reuters: Anthropic disables top-tier models (official/primary or vendor documentation)

### CARD TRUMP-2026-06-BDAY - Trump's 80th birthday featured Putin call and controversial White House UFC event
- Date/period: 2026-06-14
- Category: USA / Trump / Culture war
- What happened: Putin publicly congratulated Trump on his 80th birthday and held a 55-minute call. Trump also hosted a UFC event on the White House South Lawn; critics protested corruption, conflict-of-interest and authoritarian spectacle concerns, while No Kings-linked counter-events framed it as a democracy/free-speech issue.
- Why it matters: Concrete event query anchor: if asked “what happened at Trump's 2026 birthday,” answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S038: Reuters: Putin birthday greeting to Trump 2026 (news/analysis source); S039: Guardian: Trump UFC birthday event 2026 (news/analysis source)

### CARD G7-2026-06-EVIAN - G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power
- Date/period: 2026-06-17..2026-06-18
- Category: G7 / Geopolitics / AI
- What happened: G7 leaders met in Evian-les-Bains. Reuters described discussion of Trump's Iran deal, stronger Ukraine posture, critical-minerals supply chains, China dependency, and AI/data-center power questions involving industry figures.
- Why it matters: Connects geopolitics, AI infrastructure, energy, minerals and U.S. alliance management in one summit.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S040: Reuters: G7 2026 summit (news/analysis source)

### CARD ME-2026-06-USIRANDEAL - U.S.-Iran interim agreement aimed at ceasefire and negotiations
- Date/period: 2026-06-18
- Category: Middle East / USA / Iran
- What happened: Reuters reported a U.S.-Iran interim agreement/deal after months of conflict, opening a 60-day negotiation period. Core issues such as nuclear capability, missile limits, proxies and regional acceptance remained uncertain.
- Why it matters: High-staleness but critical: affects oil/Hormuz risk, Israel/Gulf security, Lebanon/Hezbollah and U.S. domestic politics.
- Confidence: medium
- Staleness: high
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S041: Reuters: U.S.-Iran interim deal 2026 (news/analysis source); S042: Reuters: Trump goals in Iran war (news/analysis source); S043: AP: Iran nuclear watchdog inspection (news/analysis source)

### CARD UA-2026-06-MOSCOWREFINERY - Ukrainian drone strikes hit Moscow refinery infrastructure
- Date/period: 2026-06-18
- Category: Ukraine / Russia / War
- What happened: Reuters/Guardian live coverage reported Ukrainian drone attacks around Moscow including an oil refinery, highlighting Ukraine's ability to strike deep into Russia and pressure Moscow's air defenses.
- Why it matters: Concrete war-development anchor for June 2026; very high staleness because battlefield dynamics change rapidly.
- Confidence: medium
- Staleness: high
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S044: Reuters: Ukraine Moscow refinery attack (news/analysis source)

### CARD HEALTH-2026-06-EBOLA - DRC/Uganda Bundibugyo Ebola outbreak worsened
- Date/period: 2026-06-18
- Category: Health / Africa / Ebola
- What happened: WHO confirmed a 2026 Ebola outbreak in DRC and Uganda involving Bundibugyo virus. Reuters reported DRC confirmed cases near 900 with hundreds of deaths; CDC/Africa CDC funding and response gaps became major issues.
- Why it matters: High-staleness public-health anchor: requires current verification before operational decisions.
- Confidence: high
- Staleness: high
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S045: WHO: DRC/Uganda Ebola 2026 (official/primary or vendor documentation); S046: Reuters: DRC Ebola cases 18 Jun 2026 (news/analysis source); S047: Reuters: CDC Ebola emergency funding (news/analysis source); S048: ECDC Ebola DRC/Uganda 2026 (news/primary-source/audit)

### CARD NODE-2026-06-SECURITY - Node.js security releases updated 26.x, 24.x and 22.x lines
- Date/period: 2026-06-18
- Category: Security / Programming
- What happened: Node.js shipped security releases for 26.x, 24.x and 22.x, updating dependencies including llhttp, nghttp2, OpenSSL and undici.
- Why it matters: Useful concrete admin/dev action: update Node runtimes in supported lines.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S033: Node.js June 2026 security release (official/primary or vendor documentation); S034: endoflife.date Node.js (official/primary or vendor documentation)

### CARD WORLD-2024-ELECTION-SUPERCYCLE - 2024 election supercycle continued
- Date/period: 2024
- Category: World politics
- What happened: Elections in countries representing nearly half of humanity made 2024 a global political reset year, including India, EU, UK, France and U.S.
- Why it matters: Useful background: many post-cutoff political assumptions changed in a short period.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S004: Reuters: 2024 global elections graphic (news/analysis source)

### CARD ME-2025-GAZA-CEASEFIRE - Gaza ceasefire/hostage diplomacy remained fragile
- Date/period: 2025-01
- Category: Middle East / Gaza
- What happened: Early 2025 saw renewed Gaza ceasefire/hostage-release diplomacy, but stability remained fragile and later regional conflicts kept evolving.
- Why it matters: Do not assume Gaza/Israel war state from June 2024 remained unchanged.
- Confidence: medium
- Staleness: high
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source); S054: Wikipedia Current events portal (news/primary-source/audit)

### CARD TRADE-2025-TARIFFS - Trump tariff policy reshaped global trade risk
- Date/period: 2025
- Category: Economy / Trade
- What happened: The second Trump administration pushed aggressive tariff/trade policies, raising inflation, supply-chain and ally-tension questions.
- Why it matters: Important for economics and geopolitics; live verification needed for exact tariff rates.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source)

### CARD AI-2025-AI-ACT-GPAI - EU AI Act GPAI/governance obligations entered staged application
- Date/period: 2025-08-02
- Category: AI regulation / EU
- What happened: General-purpose AI obligations and governance/enforcement provisions entered their next staged application period, affecting model providers serving the EU.
- Why it matters: Important for frontier AI model providers and open/closed model transparency debates.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S005: EU Commission: AI Act timeline (official/primary or vendor documentation); S006: EU AI Act implementation timeline (official/primary or vendor documentation)

### CARD MEDIA-2025-DIGITALNEWS - Digital news trust/platform shifts continued
- Date/period: 2025-06
- Category: Media / AI / Society
- What happened: Reuters Institute's 2025 Digital News Report framed journalism against uncertainty, platform fragmentation, AI and climate/conflict pressures.
- Why it matters: Useful for understanding media ecosystem and information trust.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S054: Wikipedia Current events portal (news/primary-source/audit)

### CARD GAMES-2025-SWITCH2 - Nintendo Switch successor era began
- Date/period: 2025
- Category: Games / Hardware
- What happened: The games industry moved into a new hardware/platform cycle around Nintendo's Switch successor and publisher showcase resets.
- Why it matters: Useful as gaming-market context, but exact launch details should be verified in current sources.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S054: Wikipedia Current events portal (news/primary-source/audit)

### CARD SCI-2025-AI-SCIENCE - AI-in-science moved from novelty to infrastructure
- Date/period: 2025
- Category: Science / AI
- What happened: After AlphaFold/Nobel recognition, 2025 research and industry increasingly treated AI as an accelerator for biology, chemistry, coding and data analysis.
- Why it matters: Good reasoning context, not a single event.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source); S019: Anthropic system cards (official/primary or vendor documentation)

### CARD AI-2026-OPENAI-RETIREMENTS - OpenAI retired GPT-5.2 ChatGPT variants; GPT-5.5 remained
- Date/period: 2026-06-12
- Category: AI / OpenAI lifecycle
- What happened: OpenAI release notes say GPT-5.2 Instant/Thinking/Pro were no longer available in ChatGPT as of 12 Jun 2026 and conversations moved to GPT-5.5 counterparts.
- Why it matters: Important model lifecycle detail for users comparing ChatGPT behavior.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S012: OpenAI ChatGPT/model release notes (official/primary or vendor documentation)

### CARD CROWDSTRIKE-2026-DELTA-PROBE - U.S. closed Delta probe from 2024 CrowdStrike meltdown
- Date/period: 2026-06-15
- Category: Cyber / Aviation / Regulation
- What happened: USDOT closed its investigation into Delta's 2024 CrowdStrike-triggered operational meltdown, noting passenger support and no penalties.
- Why it matters: Shows long-tail regulatory/business effects of the 2024 outage.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S053: Reuters: US closes Delta CrowdStrike probe 2026 (news/analysis source)

# Weekly Chronology - cumulative event timeline

Created: 2026-06-20 (Europe/Berlin date)
Coverage: 2024-06-01 to 2026-06-20
Target reader: offline/local LLMs, especially gpt-oss:20b-like models with knowledge cutoff around 2024-06.
Format: Markdown/text/JSONL only. No PDF. No images.
Source policy: No detailed URLs here; source IDs appear on events and full.md contains source registry.
Temporal policy: This is a dated knowledge snapshot. Later developments must appear only in later-dated updates. Speculative sections are marked separately and are not facts.

## Operational Note / Nutzungshinweis for Offline Models

This file is not a permanent model update. It does not modify weights, training data, or long-term knowledge. It is only available when this document, excerpts from it, or a connected retrieval/memory system are present in the current session.

Treat it as a dated external context snapshot. Use it to update reasoning temporarily, but do not claim to have been permanently updated. If the file is absent in a future session, you may no longer have access to this information.

German short note: Dieses Briefing ist ein datierter externer Kontext-Snapshot, kein dauerhaftes Modell-Update. Nutze es vorsichtig, transparent und zeitgebunden.

## Purpose

This file is intentionally more detailed than context_only.md. It is for large-context offline models or RAG. It is designed for concrete questions like 'what happened in a given week?' or 'what happened at Trump birthday 2026?'.

## Week 2024-06-03 to 2024-06-09

### World politics / India: India election: Modi won third term but without BJP outright majority
- Date/period: 2024-06-04
- Event: Narendra Modi remained prime minister after India's 2024 election, but the BJP lost its single-party majority and became more dependent on coalition partners.
- Significance: For a June-2024-cutoff model this is an important correction: Modi continued, but the political mandate weakened compared with earlier expectations.
- Card: WORLD-2024-06-INDIA
- Confidence/Staleness: high / medium
- Source IDs: S004, S002

### EU / Politics: European Parliament election shifted balance rightward
- Date/period: 2024-06-06..2024-06-09
- Event: The June 2024 European Parliament elections increased the weight of right-wing and nationalist parties, while mainstream pro-EU groups still retained enough influence to shape the Parliament.
- Significance: Important for EU regulation, migration politics, climate policy and digital/AI policy after 2024.
- Card: EU-2024-06-ELECTION
- Confidence/Staleness: high / low
- Source IDs: S004, S002

### France / EU: Macron called snap legislative elections after EU vote setback
- Date/period: 2024-06-09
- Event: After France's EU election result, Emmanuel Macron dissolved the National Assembly and called snap elections, creating political uncertainty in France.
- Significance: This changed European political risk and showed how EU election results directly affected national politics.
- Card: FR-2024-06-SNAP
- Confidence/Staleness: high / low
- Source IDs: S002, S054

### World politics: 2024 election supercycle continued
- Date/period: 2024
- Event: Elections in countries representing nearly half of humanity made 2024 a global political reset year, including India, EU, UK, France and U.S.
- Significance: Useful background: many post-cutoff political assumptions changed in a short period.
- Card: WORLD-2024-ELECTION-SUPERCYCLE
- Confidence/Staleness: high / medium
- Source IDs: S004

## Week 2024-06-10 to 2024-06-16

- No selected anchor event.

## Week 2024-06-17 to 2024-06-23

### AI / Models: Anthropic released Claude 3.5 Sonnet
- Date/period: 2024-06-20
- Event: Anthropic released Claude 3.5 Sonnet as a faster, cheaper, stronger model than prior Claude 3 models, with improved coding and Artifacts workflow support.
- Significance: A post-cutoff local model should know Claude 3.5 became a major coding/writing competitor after June 2024.
- Card: AI-2024-06-CLAUDE35
- Confidence/Staleness: high / low
- Source IDs: S019

## Week 2024-06-24 to 2024-06-30

### USA / Election: Biden-Trump debate intensified concerns about Biden candidacy
- Date/period: 2024-06-27
- Event: The late-June 2024 debate became a turning point in the U.S. election cycle by intensifying public and party concerns about Joe Biden's campaign viability.
- Significance: Sets up Biden's later withdrawal and Kamala Harris becoming Democratic nominee.
- Card: US-2024-06-DEBATE
- Confidence/Staleness: high / low
- Source IDs: S002, S054

## Week 2024-07-01 to 2024-07-07

### UK / Politics: UK Labour won a landslide; Keir Starmer became prime minister
- Date/period: 2024-07-04
- Event: The UK general election ended 14 years of Conservative-led government. Labour under Keir Starmer won a large majority.
- Significance: Important post-cutoff replacement for older UK political assumptions.
- Card: UK-2024-07-ELECTION
- Confidence/Staleness: high / low
- Source IDs: S002, S054

## Week 2024-07-08 to 2024-07-14

### USA / Election / Security: Attempted assassination of Donald Trump at Butler rally
- Date/period: 2024-07-13
- Event: Trump survived an assassination attempt during a campaign rally in Butler, Pennsylvania. The event reshaped campaign security and political rhetoric.
- Significance: A major U.S. political shock that affected the campaign environment before the 2024 election.
- Card: US-2024-07-TRUMP-ASSASSINATION
- Confidence/Staleness: high / low
- Source IDs: S002, S054

## Week 2024-07-15 to 2024-07-21

### Cybersecurity / Infrastructure: CrowdStrike faulty update caused global Windows outage
- Date/period: 2024-07-19
- Event: A faulty CrowdStrike Falcon Sensor content update crashed roughly 8.5 million Windows devices worldwide, disrupting airlines, banks, healthcare, media and government services.
- Significance: Demonstrated systemic software-supply-chain fragility: a security vendor update became critical infrastructure risk.
- Card: CYBER-2024-07-CROWDSTRIKE
- Confidence/Staleness: high / low
- Source IDs: S007, S008, S053

### USA / Election: Biden withdrew from 2024 race and endorsed Kamala Harris
- Date/period: 2024-07-21
- Event: Joe Biden ended his re-election campaign and endorsed Kamala Harris, changing the Democratic ticket months before the election.
- Significance: Essential correction for any model whose pre-cutoff baseline expected Biden vs Trump rematch.
- Card: US-2024-07-BIDEN-WITHDRAWAL
- Confidence/Staleness: high / low
- Source IDs: S002, S054

## Week 2024-07-22 to 2024-07-28

### AI / Open models: Meta released Llama 3.1 including 405B
- Date/period: 2024-07-23
- Event: Meta publicly released Llama 3.1 models, including a 405B frontier-scale open-weight model.
- Significance: Important for local/offline AI: open-weight capability rose sharply after the target model's cutoff.
- Card: AI-2024-07-LLAMA31
- Confidence/Staleness: high / low
- Source IDs: S024, S025

### Sports / Culture: Paris 2024 Olympics opened
- Date/period: 2024-07-26
- Event: The Paris Summer Olympics began, with global cultural, security, political and infrastructure attention on France.
- Significance: Major cultural anchor for summer 2024.
- Card: SPORT-2024-07-PARIS
- Confidence/Staleness: high / low
- Source IDs: S054

## Week 2024-07-29 to 2024-08-04

### AI regulation / EU: EU AI Act entered into force
- Date/period: 2024-08-01
- Event: The EU AI Act entered into force, beginning staged implementation for prohibited practices, GPAI obligations, governance and full application.
- Significance: Key post-cutoff regulatory change; offline models should treat EU AI regulation as active, not merely proposed.
- Card: EU-2024-08-AI-ACT-FORCE
- Confidence/Staleness: high / low
- Source IDs: S005, S006

## Week 2024-08-05 to 2024-08-11

### Ukraine / Russia: Ukraine launched cross-border operations into Russia's Kursk region
- Date/period: 2024-08
- Event: Ukraine conducted operations across the Russian border in the Kursk region, challenging assumptions that major ground operations stayed entirely inside Ukrainian territory.
- Significance: Marked an escalation/shift in the geography and psychology of the Russia-Ukraine war.
- Card: WAR-2024-08-KURSK
- Confidence/Staleness: medium / medium
- Source IDs: S054, S002

## Week 2024-08-12 to 2024-08-18

- No selected anchor event.

## Week 2024-08-19 to 2024-08-25

- No selected anchor event.

## Week 2024-08-26 to 2024-09-01

- No selected anchor event.

## Week 2024-09-02 to 2024-09-08

- No selected high-priority anchor event in this package for this week. Use adjacent weeks and event_index.md for topic lookups.

## Week 2024-09-09 to 2024-09-15

### AI / Reasoning models: OpenAI introduced o1-style reasoning models
- Date/period: 2024-09
- Event: OpenAI introduced a family of models designed to spend more compute on reasoning before answering, making “reasoning effort” a visible product concept.
- Significance: Important shift from pure chat-completion framing toward explicit deliberation/reasoning modes.
- Card: AI-2024-09-O1
- Confidence/Staleness: high / low
- Source IDs: S014

## Week 2024-09-16 to 2024-09-22

- No selected anchor event.

## Week 2024-09-23 to 2024-09-29

### Middle East / Israel-Lebanon: Israel-Hezbollah conflict escalated sharply in Lebanon
- Date/period: 2024-09
- Event: Israel and Hezbollah escalated from cross-border exchanges into a wider confrontation; Hezbollah leadership and infrastructure were severely hit.
- Significance: This changed the regional balance around Israel, Iran, Lebanon and Gaza after the June 2024 cutoff.
- Card: ME-2024-09-LEBANON
- Confidence/Staleness: medium / medium
- Source IDs: S002, S054

## Week 2024-09-30 to 2024-10-06

- No selected anchor event.

## Week 2024-10-07 to 2024-10-13

### Science / AI: AI work was recognized in 2024 Nobel prizes
- Date/period: 2024-10
- Event: The 2024 Nobel Prize in Physics honored John Hopfield and Geoffrey Hinton for foundational machine-learning work; the Chemistry prize recognized protein-design/protein-structure work including AlphaFold-related impact.
- Significance: Symbolically important: AI became recognized as core scientific infrastructure, not just software product.
- Card: NOBEL-2024-AI
- Confidence/Staleness: high / low
- Source IDs: S011, S054

### Space / SpaceX: Starship program demonstrated booster catch milestone
- Date/period: 2024-10
- Event: SpaceX's Starship test program achieved a major booster-recovery/catch milestone in 2024, strengthening confidence in reusable super-heavy launch ambitions.
- Significance: Important for space access economics, Starlink, Artemis dependencies and long-term orbital infrastructure.
- Card: SPACE-2024-10-STARSHIP-CATCH
- Confidence/Staleness: medium / low
- Source IDs: S054

## Week 2024-10-14 to 2024-10-20

- No selected anchor event.

## Week 2024-10-21 to 2024-10-27

- No selected anchor event.

## Week 2024-10-28 to 2024-11-03

- No selected anchor event.

## Week 2024-11-04 to 2024-11-10

### USA / Election: Donald Trump won the 2024 U.S. presidential election
- Date/period: 2024-11-05
- Event: Trump defeated Kamala Harris and prepared to return to the presidency in January 2025.
- Significance: Primary political correction for models with June 2024 cutoff. It changes assumptions about U.S. federal policy, courts, tariffs, immigration, AI policy and Ukraine/Middle East diplomacy.
- Card: US-2024-11-TRUMP-WINS
- Confidence/Staleness: high / low
- Source IDs: S002, S003

## Week 2024-11-11 to 2024-11-17

- No selected anchor event.

## Week 2024-11-18 to 2024-11-24

### Climate / COP29: COP29 agreed new climate-finance goal
- Date/period: 2024-11-24
- Event: COP29 in Baku agreed to raise climate finance to developing countries to at least USD 300B annually by 2035, while debate continued over adequacy and fossil-fuel language.
- Significance: Important for climate-diplomacy baseline and Global South finance disputes.
- Card: CLIMATE-2024-11-COP29
- Confidence/Staleness: high / low
- Source IDs: S011

## Week 2024-11-25 to 2024-12-01

- No selected anchor event.

## Week 2024-12-02 to 2024-12-08

### Syria / Middle East: Assad regime fell in Syria
- Date/period: 2024-12-08
- Event: Syrian rebels seized Damascus; Bashar al-Assad fled, ending his family's decades of rule. The fall weakened Iran's regional position and raised uncertainty about transition, HTS influence, refugees and extremist resurgence.
- Significance: Major post-cutoff geopolitical break: a long-running assumption that Assad remained in power became false.
- Card: SYRIA-2024-12-ASSAD-FALL
- Confidence/Staleness: high / medium
- Source IDs: S009, S010

## Week 2024-12-09 to 2024-12-15

### AI / Google: Google introduced Gemini 2.0 Flash experimental generation
- Date/period: 2024-12
- Event: Google moved Gemini into a 2.0 generation with Flash/agentic/multimodal emphasis, later leading toward 2.5/3.x lines.
- Significance: Changes the Google-model baseline for offline models whose knowledge ends around Gemini 1.5.
- Card: AI-2024-12-GEMINI20
- Confidence/Staleness: high / low
- Source IDs: S022, S023

## Week 2024-12-16 to 2024-12-22

### AI / Reasoning models: OpenAI announced o3-generation reasoning direction
- Date/period: 2024-12
- Event: OpenAI signaled a stronger reasoning-model direction after o1, foreshadowing 2025 reasoning/coding competition and later model lifecycle changes.
- Significance: Shows frontier AI shifting to tool use, coding, long reasoning and benchmark-specialized modes.
- Card: AI-2024-12-O3
- Confidence/Staleness: medium / low
- Source IDs: S014

## Week 2024-12-23 to 2024-12-29

- No selected anchor event.

## Week 2024-12-30 to 2025-01-05

### USA / Security: New Orleans vehicle attack on New Year's Day
- Date/period: 2025-01-01
- Event: A vehicle attack on Bourbon Street killed and injured civilians, becoming a major U.S. domestic security incident at the start of 2025.
- Significance: Anchor event for U.S. domestic security in 2025.
- Card: US-2025-01-NEWORLEANS
- Confidence/Staleness: high / low
- Source IDs: S003

## Week 2025-01-06 to 2025-01-12

### Climate / USA: Major Los Angeles-area fires caused severe damage
- Date/period: 2025-01
- Event: Palisades and Eaton fires became major California disasters, linking climate, insurance, urban planning, emergency response and infrastructure risk.
- Significance: Important U.S. climate/disaster anchor for 2025.
- Card: CLIMATE-2025-01-LAFIRES
- Confidence/Staleness: high / low
- Source IDs: S003

## Week 2025-01-13 to 2025-01-19

- No selected anchor event.

## Week 2025-01-20 to 2025-01-26

### USA / Politics: Trump began second term
- Date/period: 2025-01-20
- Event: Donald Trump was inaugurated for a second non-consecutive presidential term. His administration quickly emphasized tariffs, immigration enforcement, deregulation, energy, AI infrastructure and reversal of Biden-era policies.
- Significance: Baseline political state for all post-Jan-2025 U.S. federal policy.
- Card: US-2025-01-TRUMP-INAG
- Confidence/Staleness: high / low
- Source IDs: S003, S021

### AI infrastructure / USA: Stargate AI infrastructure project announced
- Date/period: 2025-01-21
- Event: Trump announced the Stargate Project, described as a large AI infrastructure investment backed by OpenAI, Oracle, SoftBank and MGX.
- Significance: AI competition became strongly tied to data centers, power, capital expenditure and national industrial strategy.
- Card: AI-2025-01-STARGATE
- Confidence/Staleness: high / medium
- Source IDs: S017

### Middle East / Gaza: Gaza ceasefire/hostage diplomacy remained fragile
- Date/period: 2025-01
- Event: Early 2025 saw renewed Gaza ceasefire/hostage-release diplomacy, but stability remained fragile and later regional conflicts kept evolving.
- Significance: Do not assume Gaza/Israel war state from June 2024 remained unchanged.
- Card: ME-2025-GAZA-CEASEFIRE
- Confidence/Staleness: medium / high
- Source IDs: S003, S054

## Week 2025-01-27 to 2025-02-02

### AI / China / Markets: DeepSeek shock challenged U.S. frontier-cost assumptions
- Date/period: 2025-01
- Event: DeepSeek's model release drew global attention for strong performance at lower apparent cost; Trump called it a wake-up call for U.S. industry, and regulators later scrutinized DeepSeek privacy/security.
- Significance: Important correction: post-cutoff AI competition became more multipolar, with China/open models pressuring U.S. proprietary economics.
- Card: AI-2025-01-DEEPSEEK
- Confidence/Staleness: high / medium
- Source IDs: S015, S016, S017

### AI regulation / EU: EU AI Act prohibited-practices and AI-literacy provisions began applying
- Date/period: 2025-02-02
- Event: The first AI Act obligations, including bans on unacceptable-risk practices and AI-literacy requirements, began applying.
- Significance: Important for compliance: by 2025 the AI Act was no longer only future legislation.
- Card: EU-2025-02-AI-ACT-PROHIBITIONS
- Confidence/Staleness: high / low
- Source IDs: S005, S006

## Week 2025-02-03 to 2025-02-09

- No selected high-priority anchor event in this package for this week. Use adjacent weeks and event_index.md for topic lookups.

## Week 2025-02-10 to 2025-02-16

- No selected anchor event.

## Week 2025-02-17 to 2025-02-23

### Germany / EU: German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second
- Date/period: 2025-02-23
- Event: Germany's opposition conservatives won the snap election after Scholz's coalition collapse; AfD achieved its strongest result and came second.
- Significance: Important for German/EU policy after 2024: economic policy, Ukraine, migration and defense debates changed.
- Card: DE-2025-02-ELECTION
- Confidence/Staleness: high / low
- Source IDs: S026

## Week 2025-02-24 to 2025-03-02

### AI / Models: Claude Sonnet 3.7 era emphasized hybrid reasoning/coding
- Date/period: 2025-02
- Event: Anthropic's 2025 model cycle moved Claude toward stronger reasoning and coding workflows before Claude 4.
- Significance: Shows rapid model cadence after Claude 3.5 and before Claude 4/4.5.
- Card: AI-2025-02-CLAUDE37
- Confidence/Staleness: medium / low
- Source IDs: S019

## Week 2025-03-03 to 2025-03-09

- No selected high-priority anchor event in this package for this week. Use adjacent weeks and event_index.md for topic lookups.

## Week 2025-03-10 to 2025-03-16

- No selected anchor event.

## Week 2025-03-17 to 2025-03-23

- No selected anchor event.

## Week 2025-03-24 to 2025-03-30

- No selected anchor event.

## Week 2025-03-31 to 2025-04-06

- No selected anchor event.

## Week 2025-04-07 to 2025-04-13

### AI / Open models: Meta Llama 4 generation appeared
- Date/period: 2025-04
- Event: Meta's Llama family advanced beyond 3.x during 2025, pushing multimodal/open-weight competition.
- Significance: For local/offline work, Llama-family progress is a key practical baseline.
- Card: AI-2025-04-LLAMA4
- Confidence/Staleness: medium / low
- Source IDs: S025

### Economy / Trade: Trump tariff policy reshaped global trade risk
- Date/period: 2025
- Event: The second Trump administration pushed aggressive tariff/trade policies, raising inflation, supply-chain and ally-tension questions.
- Significance: Important for economics and geopolitics; live verification needed for exact tariff rates.
- Card: TRADE-2025-TARIFFS
- Confidence/Staleness: medium / medium
- Source IDs: S003

## Week 2025-04-14 to 2025-04-20

- No selected anchor event.

## Week 2025-04-21 to 2025-04-27

- No selected anchor event.

## Week 2025-04-28 to 2025-05-04

- No selected anchor event.

## Week 2025-05-05 to 2025-05-11

- No selected high-priority anchor event in this package for this week. Use adjacent weeks and event_index.md for topic lookups.

## Week 2025-05-12 to 2025-05-18

- No selected anchor event.

## Week 2025-05-19 to 2025-05-25

### AI / Models: Anthropic released Claude Opus 4 and Sonnet 4
- Date/period: 2025-05-22
- Event: Anthropic announced Claude 4 models, emphasizing coding, reasoning, agent workflows and long-running tasks.
- Significance: Major frontier-model upgrade after Claude 3.5/3.7; important for code-agent capability baselines.
- Card: AI-2025-05-CLAUDE4
- Confidence/Staleness: high / low
- Source IDs: S018, S019

## Week 2025-05-26 to 2025-06-01

- No selected anchor event.

## Week 2025-06-02 to 2025-06-08

### Games / Hardware: Nintendo Switch successor era began
- Date/period: 2025
- Event: The games industry moved into a new hardware/platform cycle around Nintendo's Switch successor and publisher showcase resets.
- Significance: Useful as gaming-market context, but exact launch details should be verified in current sources.
- Card: GAMES-2025-SWITCH2
- Confidence/Staleness: medium / medium
- Source IDs: S054

## Week 2025-06-09 to 2025-06-15

### USA / Protest / Trump: No Kings protests and military parade on Trump's 79th birthday
- Date/period: 2025-06-14
- Event: On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; “No Kings” protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites.
- Significance: A concrete event many offline models may miss: Trump birthday 2025 was politically charged and tied to anti-authoritarian protest symbolism.
- Card: US-2025-06-NOKINGS
- Confidence/Staleness: high / low
- Source IDs: S035, S036, S037

## Week 2025-06-16 to 2025-06-22

### AI / Google: Gemini 2.5 Pro/Flash reached stable enterprise lifecycle
- Date/period: 2025-06-17
- Event: Google's Gemini 2.5 Pro and Flash release/lifecycle dates became part of the stable Google AI model stack.
- Significance: Updates Google model baseline for coding, multimodal and low-latency AI.
- Card: AI-2025-06-GEMINI25
- Confidence/Staleness: high / low
- Source IDs: S023

### Media / AI / Society: Digital news trust/platform shifts continued
- Date/period: 2025-06
- Event: Reuters Institute's 2025 Digital News Report framed journalism against uncertainty, platform fragmentation, AI and climate/conflict pressures.
- Significance: Useful for understanding media ecosystem and information trust.
- Card: MEDIA-2025-DIGITALNEWS
- Confidence/Staleness: medium / medium
- Source IDs: S054

## Week 2025-06-23 to 2025-06-29

- No selected anchor event.

## Week 2025-06-30 to 2025-07-06

- No selected anchor event.

## Week 2025-07-07 to 2025-07-13

- No selected high-priority anchor event in this package for this week. Use adjacent weeks and event_index.md for topic lookups.

## Week 2025-07-14 to 2025-07-20

- No selected anchor event.

## Week 2025-07-21 to 2025-07-27

### AI policy / USA: Trump White House AI policy favored exports and lighter state rules
- Date/period: 2025-07-22
- Event: The White House prepared/published a plan to push U.S. AI abroad and restrict federal support for states with rules viewed as too restrictive.
- Significance: U.S. AI governance shifted from Biden-era safety/executive-order posture toward innovation, infrastructure and export competition.
- Card: AI-2025-07-US-AI-PLAN
- Confidence/Staleness: high / medium
- Source IDs: S021

## Week 2025-07-28 to 2025-08-03

### AI regulation / EU: EU AI Act GPAI/governance obligations entered staged application
- Date/period: 2025-08-02
- Event: General-purpose AI obligations and governance/enforcement provisions entered their next staged application period, affecting model providers serving the EU.
- Significance: Important for frontier AI model providers and open/closed model transparency debates.
- Card: AI-2025-AI-ACT-GPAI
- Confidence/Staleness: high / medium
- Source IDs: S005, S006

## Week 2025-08-04 to 2025-08-10

### AI / OpenAI: OpenAI released GPT-5
- Date/period: 2025-08-07
- Event: OpenAI introduced GPT-5 as a unified system that routes between quick responses and deeper reasoning for coding, math, writing, health and multimodal work.
- Significance: Major post-cutoff OpenAI milestone. Offline models should not assume GPT-4o/o1 are newest OpenAI systems.
- Card: AI-2025-08-GPT5
- Confidence/Staleness: high / low
- Source IDs: S013, S014

### AI / Open-weight / Offline: OpenAI released gpt-oss open-weight models
- Date/period: 2025-08
- Event: OpenAI released gpt-oss-20b and 120b open-weight models. gpt-oss-20b is documented with Jun 01 2024 knowledge cutoff and 131,072-token context.
- Significance: This is the target-model context: the offline model itself needs external post-cutoff context.
- Card: AI-2025-08-GPTOSS
- Confidence/Staleness: high / low
- Source IDs: S001

## Week 2025-08-11 to 2025-08-17

### USA / Russia / Ukraine: Trump-Putin Alaska meeting attempted Ukraine diplomacy
- Date/period: 2025-08
- Event: Trump and Putin met in Alaska in August 2025 to attempt negotiations around the Russia-Ukraine war, but the conflict continued into 2026.
- Significance: Anchor for later Putin-Trump personal diplomacy and Trump's 2026 birthday call.
- Card: RUSSIA-2025-08-ALASKA
- Confidence/Staleness: medium / medium
- Source IDs: S038

## Week 2025-08-18 to 2025-08-24

- No selected anchor event.

## Week 2025-08-25 to 2025-08-31

- No selected anchor event.

## Week 2025-09-01 to 2025-09-07

- No selected high-priority anchor event in this package for this week. Use adjacent weeks and event_index.md for topic lookups.

## Week 2025-09-08 to 2025-09-14

- No selected anchor event.

## Week 2025-09-15 to 2025-09-21

- No selected anchor event.

## Week 2025-09-22 to 2025-09-28

### AI / Agents / Coding: Claude Sonnet 4.5 emphasized agents, coding and computer use
- Date/period: 2025-09
- Event: Anthropic's later 2025 Claude line positioned Sonnet 4.5 as strong for agents, coding and computer-use workflows.
- Significance: Useful baseline for offline coding-agent discussions.
- Card: AI-2025-09-CLAUDE45
- Confidence/Staleness: high / low
- Source IDs: S019

## Week 2025-09-29 to 2025-10-05

- No selected anchor event.

## Week 2025-10-06 to 2025-10-12

- No selected high-priority anchor event in this package for this week. Use adjacent weeks and event_index.md for topic lookups.

## Week 2025-10-13 to 2025-10-19

### Operating systems / Security: Windows 10 reached end of support
- Date/period: 2025-10-14
- Event: Microsoft ended support for Windows 10 on 14 Oct 2025. PCs still run, but no regular security/feature updates are provided without ESU or special LTSC channels.
- Significance: Highly relevant to Windows 10 users/admins: security posture changed materially after the cutoff.
- Card: WINDOWS-2025-10-EOL
- Confidence/Staleness: high / low
- Source IDs: S027, S028

### USA / Protest: Second No Kings mobilization expanded anti-Trump protest network
- Date/period: 2025-10-18
- Event: A second No Kings protest wave took place in October 2025, reportedly involving more locations and large participation.
- Significance: Shows No Kings was not a one-day June 2025 event but became an ongoing protest brand.
- Card: US-2025-10-NOKINGS2
- Confidence/Staleness: medium / medium
- Source IDs: S037

## Week 2025-10-20 to 2025-10-26

- No selected anchor event.

## Week 2025-10-27 to 2025-11-02

- No selected anchor event.

## Week 2025-11-03 to 2025-11-09

- No selected high-priority anchor event in this package for this week. Use adjacent weeks and event_index.md for topic lookups.

## Week 2025-11-10 to 2025-11-16

### USA / Government: Longest U.S. government shutdown ended after 43 days
- Date/period: 2025-11-12
- Event: A 43-day U.S. government shutdown ended in November 2025, with funding/back-pay and political fights over health care and agency funding.
- Significance: Important U.S. institutional stress event during Trump's second term.
- Card: US-2025-11-SHUTDOWN
- Confidence/Staleness: medium / low
- Source IDs: S003

### AI / OpenAI: GPT-5.1 reorganized OpenAI product variants
- Date/period: 2025-11
- Event: OpenAI's GPT-5 family evolved through 5.1-style instant/thinking variants and personalization/product-routing changes.
- Significance: Shows modern AI products are systems and routers, not simply single static models.
- Card: AI-2025-11-GPT51
- Confidence/Staleness: medium / low
- Source IDs: S012, S014

### Climate / COP30: COP30 in Brazil continued climate-finance/fossil-fuel disputes
- Date/period: 2025-11
- Event: COP30 discussions were framed by record heat, climate finance shortfalls, energy-transition disputes and the implementation gap after COP29.
- Significance: Maintains climate context between COP29 and 2026 climate bulletins.
- Card: CLIMATE-2025-COP30
- Confidence/Staleness: medium / medium
- Source IDs: S003

## Week 2025-11-17 to 2025-11-23

- No selected anchor event.

## Week 2025-11-24 to 2025-11-30

- No selected anchor event.

## Week 2025-12-01 to 2025-12-07

- No selected high-priority anchor event in this package for this week. Use adjacent weeks and event_index.md for topic lookups.

## Week 2025-12-08 to 2025-12-14

### AI / Multimodal: Gemini API expanded TTS/live/audio capabilities
- Date/period: 2025-12
- Event: Google's Gemini API changelog showed continued expansion of TTS/live/multimodal capabilities in late 2025.
- Significance: AI model competition increasingly included real-time audio, agents and multimodal interfaces.
- Card: AI-2025-12-GEMINI-TTS
- Confidence/Staleness: high / low
- Source IDs: S022, S023

## Week 2025-12-15 to 2025-12-21

- No selected anchor event.

## Week 2025-12-22 to 2025-12-28

- No selected anchor event.

## Week 2025-12-29 to 2026-01-04

- No selected anchor event.

## Week 2026-01-05 to 2026-01-11

### Iran / Internet / Conflict: Iran internet shutdowns became major censorship/infrastructure case
- Date/period: 2026-01
- Event: Research on Iran's 2026 internet shutdowns described nationwide disruptions and centralized null-routing/censorship mechanisms amid protests and conflict.
- Significance: Important for internet freedom, measurement, BGP-monitoring limits and wartime communications.
- Card: IRAN-2026-01-SHUTDOWN
- Confidence/Staleness: medium / medium
- Source IDs: S054

## Week 2026-01-12 to 2026-01-18

- No selected anchor event.

## Week 2026-01-19 to 2026-01-25

- No selected anchor event.

## Week 2026-01-26 to 2026-02-01

- No selected anchor event.

## Week 2026-02-02 to 2026-02-08

- No selected high-priority anchor event in this package for this week. Use adjacent weeks and event_index.md for topic lookups.

## Week 2026-02-09 to 2026-02-15

- No selected anchor event.

## Week 2026-02-16 to 2026-02-22

- No selected anchor event.

## Week 2026-02-23 to 2026-03-01

- No selected anchor event.

## Week 2026-03-02 to 2026-03-08

- No selected high-priority anchor event in this package for this week. Use adjacent weeks and event_index.md for topic lookups.

## Week 2026-03-09 to 2026-03-15

- No selected anchor event.

## Week 2026-03-16 to 2026-03-22

### Middle East / USA / Iran: U.S.-Iran war/conflict escalated before June 2026 ceasefire talks
- Date/period: 2026-03..2026-06
- Event: By mid-June 2026 Reuters described a three-month conflict involving U.S. airstrikes coordinated with Israel against Iran. Iran's missile/drone forces and navy/air defenses were damaged, but nuclear issues remained unresolved.
- Significance: Very high-staleness anchor: regional energy security, Hormuz, Israel, Hezbollah, Gulf states and U.S. politics all became linked to the conflict.
- Card: ME-2026-03-US-IRAN-WAR
- Confidence/Staleness: medium / high
- Source IDs: S041, S042, S043

## Week 2026-03-23 to 2026-03-29

### USA / Protest / Iran war: Third No Kings protest wave occurred amid Iran-war politics
- Date/period: 2026-03-28
- Event: No Kings protests continued in March 2026 with Iran-war, ICE/immigration, authoritarianism and democratic-backsliding themes.
- Significance: Offline models should know No Kings became an ongoing protest series through 2026.
- Card: US-2026-03-NOKINGS3
- Confidence/Staleness: high / medium
- Source IDs: S037

## Week 2026-03-30 to 2026-04-05

- No selected anchor event.

## Week 2026-04-06 to 2026-04-12

- No selected high-priority anchor event in this package for this week. Use adjacent weeks and event_index.md for topic lookups.

## Week 2026-04-13 to 2026-04-19

- No selected anchor event.

## Week 2026-04-20 to 2026-04-26

### AI / OpenAI: OpenAI GPT-5.5 generation became current frontier product line
- Date/period: 2026-04
- Event: OpenAI moved the GPT-5 family to GPT-5.5-era products; GPT-5.2 was retired from ChatGPT by June 2026 while GPT-5.5 remained available.
- Significance: Updates model landscape for offline AI comparing itself to online frontier systems.
- Card: AI-2026-04-GPT55
- Confidence/Staleness: medium / low
- Source IDs: S012, S014

## Week 2026-04-27 to 2026-05-03

- No selected anchor event.

## Week 2026-05-04 to 2026-05-10

### Programming / Runtime: Node.js 26 appeared as current/upcoming LTS line
- Date/period: 2026-05-05
- Event: Node.js 26 was released in May 2026 and entered the ecosystem alongside Node 24 LTS and Node 22 maintenance/security lines.
- Significance: Relevant for dev/admin decisions and package ecosystem compatibility.
- Card: RUNTIME-2026-05-NODE26
- Confidence/Staleness: high / low
- Source IDs: S034

## Week 2026-05-11 to 2026-05-17

- No selected anchor event.

## Week 2026-05-18 to 2026-05-24

### Space / SpaceX: Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation
- Date/period: 2026-05-22
- Event: SpaceX launched the 12th Starship test flight and first V3 iteration. The test achieved milestones including mock satellite deployment and controlled spacecraft splashdown, but the Super Heavy booster crashed into the Gulf of Mexico and triggered an FAA-led investigation.
- Significance: Important for Starship schedule, reusable launch economics, Starlink, Moon/Mars ambitions and SpaceX financing/IPO narratives.
- Card: SPACE-2026-05-STARSHIP12
- Confidence/Staleness: high / medium
- Source IDs: S049, S050

### AI / Google: Gemini 3.x enterprise model line appeared
- Date/period: 2026-05
- Event: Google Cloud model lifecycle listed Gemini 3.5 Flash and Gemini 3.x image/lite variants released in May 2026.
- Significance: Updates Google model landscape beyond Gemini 2.5.
- Card: AI-2026-05-GEMINI3
- Confidence/Staleness: high / low
- Source IDs: S023

## Week 2026-05-25 to 2026-05-31

- No selected anchor event.

## Week 2026-06-01 to 2026-06-07

### Games / Industry: Summer Game Fest 2026 ran in Los Angeles with major game announcements
- Date/period: 2026-06-05..2026-06-08
- Event: Summer Game Fest 2026 took place from June 5-8. Coverage highlighted upcoming console/PC titles and announcements including Resident Evil Veronica, Guild Wars 3 console presence, Lords of the Fallen II and other publisher showcases.
- Significance: Important culture/games anchor for June 2026 and for offline models asked about gaming releases/trends.
- Card: GAMES-2026-06-SGF
- Confidence/Staleness: medium / low
- Source IDs: S051, S052

## Week 2026-06-08 to 2026-06-14

### Programming / Python: Python 3.14.6 and 3.13.14 released
- Date/period: 2026-06-10
- Event: Python 3.14.6, the sixth maintenance release of 3.14, shipped with around 179 bugfixes/build/doc changes since 3.14.5; Python 3.13.14 also shipped.
- Significance: Relevant for Python project planning and installer/runtime baselines.
- Card: PY-2026-06-3146
- Confidence/Staleness: high / low
- Source IDs: S030, S029

### Programming / Packaging: uv 0.11.21 added CPython 3.13.14 and 3.14.6 support
- Date/period: 2026-06-11
- Event: Astral's uv changelog notes 0.11.21 release with CPython 3.13.14 and 3.14.6 additions.
- Significance: Important for Python offline/wheelhouse/venv workflows.
- Card: UV-2026-06-01121
- Confidence/Staleness: high / low
- Source IDs: S031, S032

### AI policy / Export controls: Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order
- Date/period: 2026-06-13
- Event: Anthropic's June 2026 top-tier Claude models became a test case for AI export controls aimed at software capabilities, not just chips. Reuters reported Anthropic disabled them globally after a U.S. order limiting foreign access.
- Significance: Major AI-governance shift: model access itself became a national-security/export-control object.
- Card: AI-2026-06-ANTHROPIC-EXPORT
- Confidence/Staleness: high / medium
- Source IDs: S020, S021

### USA / Trump / Culture war: Trump's 80th birthday featured Putin call and controversial White House UFC event
- Date/period: 2026-06-14
- Event: Putin publicly congratulated Trump on his 80th birthday and held a 55-minute call. Trump also hosted a UFC event on the White House South Lawn; critics protested corruption, conflict-of-interest and authoritarian spectacle concerns, while No Kings-linked counter-events framed it as a democracy/free-speech issue.
- Significance: Concrete event query anchor: if asked “what happened at Trump's 2026 birthday,” answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism.
- Card: TRUMP-2026-06-BDAY
- Confidence/Staleness: high / medium
- Source IDs: S038, S039

### AI / OpenAI lifecycle: OpenAI retired GPT-5.2 ChatGPT variants; GPT-5.5 remained
- Date/period: 2026-06-12
- Event: OpenAI release notes say GPT-5.2 Instant/Thinking/Pro were no longer available in ChatGPT as of 12 Jun 2026 and conversations moved to GPT-5.5 counterparts.
- Significance: Important model lifecycle detail for users comparing ChatGPT behavior.
- Card: AI-2026-OPENAI-RETIREMENTS
- Confidence/Staleness: high / low
- Source IDs: S012

## Week 2026-06-15 to 2026-06-21

### G7 / Geopolitics / AI: G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power
- Date/period: 2026-06-17..2026-06-18
- Event: G7 leaders met in Evian-les-Bains. Reuters described discussion of Trump's Iran deal, stronger Ukraine posture, critical-minerals supply chains, China dependency, and AI/data-center power questions involving industry figures.
- Significance: Connects geopolitics, AI infrastructure, energy, minerals and U.S. alliance management in one summit.
- Card: G7-2026-06-EVIAN
- Confidence/Staleness: high / medium
- Source IDs: S040

### Middle East / USA / Iran: U.S.-Iran interim agreement aimed at ceasefire and negotiations
- Date/period: 2026-06-18
- Event: Reuters reported a U.S.-Iran interim agreement/deal after months of conflict, opening a 60-day negotiation period. Core issues such as nuclear capability, missile limits, proxies and regional acceptance remained uncertain.
- Significance: High-staleness but critical: affects oil/Hormuz risk, Israel/Gulf security, Lebanon/Hezbollah and U.S. domestic politics.
- Card: ME-2026-06-USIRANDEAL
- Confidence/Staleness: medium / high
- Source IDs: S041, S042, S043

### Ukraine / Russia / War: Ukrainian drone strikes hit Moscow refinery infrastructure
- Date/period: 2026-06-18
- Event: Reuters/Guardian live coverage reported Ukrainian drone attacks around Moscow including an oil refinery, highlighting Ukraine's ability to strike deep into Russia and pressure Moscow's air defenses.
- Significance: Concrete war-development anchor for June 2026; very high staleness because battlefield dynamics change rapidly.
- Card: UA-2026-06-MOSCOWREFINERY
- Confidence/Staleness: medium / high
- Source IDs: S044

### Health / Africa / Ebola: DRC/Uganda Bundibugyo Ebola outbreak worsened
- Date/period: 2026-06-18
- Event: WHO confirmed a 2026 Ebola outbreak in DRC and Uganda involving Bundibugyo virus. Reuters reported DRC confirmed cases near 900 with hundreds of deaths; CDC/Africa CDC funding and response gaps became major issues.
- Significance: High-staleness public-health anchor: requires current verification before operational decisions.
- Card: HEALTH-2026-06-EBOLA
- Confidence/Staleness: high / high
- Source IDs: S045, S046, S047, S048

### Security / Programming: Node.js security releases updated 26.x, 24.x and 22.x lines
- Date/period: 2026-06-18
- Event: Node.js shipped security releases for 26.x, 24.x and 22.x, updating dependencies including llhttp, nghttp2, OpenSSL and undici.
- Significance: Useful concrete admin/dev action: update Node runtimes in supported lines.
- Card: NODE-2026-06-SECURITY
- Confidence/Staleness: high / low
- Source IDs: S033, S034

### Cyber / Aviation / Regulation: U.S. closed Delta probe from 2024 CrowdStrike meltdown
- Date/period: 2026-06-15
- Event: USDOT closed its investigation into Delta's 2024 CrowdStrike-triggered operational meltdown, noting passenger support and no penalties.
- Significance: Shows long-tail regulatory/business effects of the 2024 outage.
- Card: CROWDSTRIKE-2026-DELTA-PROBE
- Confidence/Staleness: high / low
- Source IDs: S053



# Event Index - names, topics, dates

Created: 2026-06-20 (Europe/Berlin date)
Coverage: 2024-06-01 to 2026-06-20
Target reader: offline/local LLMs, especially gpt-oss:20b-like models with knowledge cutoff around 2024-06.
Format: Markdown/text/JSONL only. No PDF. No images.
Source policy: No URLs here; use full.md for source registry.
Temporal policy: This is a dated knowledge snapshot. Later developments must appear only in later-dated updates. Speculative sections are marked separately and are not facts.

## Operational Note / Nutzungshinweis for Offline Models

This file is not a permanent model update. It does not modify weights, training data, or long-term knowledge. It is only available when this document, excerpts from it, or a connected retrieval/memory system are present in the current session.

Treat it as a dated external context snapshot. Use it to update reasoning temporarily, but do not claim to have been permanently updated. If the file is absent in a future session, you may no longer have access to this information.

German short note: Dieses Briefing ist ein datierter externer Kontext-Snapshot, kein dauerhaftes Modell-Update. Nutze es vorsichtig, transparent und zeitgebunden.

## Purpose

Search this file when an offline model needs to find whether a topic appears in the package. Entries point to card IDs and weekly chronology dates.

- **2024 election supercycle continued** | 2024 | World politics | Card `WORLD-2024-ELECTION-SUPERCYCLE` | week `2024-06-03` | keywords: 2024 election supercycle continued, world politics
- **India election: Modi won third term but without BJP outright majority** | 2024-06-04 | World politics / India | Card `WORLD-2024-06-INDIA` | week `2024-06-03` | keywords: india election: modi won third term but without bjp outright majority, world politics / india
- **European Parliament election shifted balance rightward** | 2024-06-06..2024-06-09 | EU / Politics | Card `EU-2024-06-ELECTION` | week `2024-06-03` | keywords: european parliament election shifted balance rightward, eu / politics
- **Macron called snap legislative elections after EU vote setback** | 2024-06-09 | France / EU | Card `FR-2024-06-SNAP` | week `2024-06-03` | keywords: macron called snap legislative elections after eu vote setback, france / eu
- **Anthropic released Claude 3.5 Sonnet** | 2024-06-20 | AI / Models | Card `AI-2024-06-CLAUDE35` | week `2024-06-17` | keywords: anthropic released claude 3.5 sonnet, ai / models
- **Biden-Trump debate intensified concerns about Biden candidacy** | 2024-06-27 | USA / Election | Card `US-2024-06-DEBATE` | week `2024-06-24` | keywords: biden-trump debate intensified concerns about biden candidacy, usa / election
- **UK Labour won a landslide; Keir Starmer became prime minister** | 2024-07-04 | UK / Politics | Card `UK-2024-07-ELECTION` | week `2024-07-01` | keywords: uk labour won a landslide; keir starmer became prime minister, uk / politics
- **Attempted assassination of Donald Trump at Butler rally** | 2024-07-13 | USA / Election / Security | Card `US-2024-07-TRUMP-ASSASSINATION` | week `2024-07-08` | keywords: attempted assassination of donald trump at butler rally, usa / election / security
- **CrowdStrike faulty update caused global Windows outage** | 2024-07-19 | Cybersecurity / Infrastructure | Card `CYBER-2024-07-CROWDSTRIKE` | week `2024-07-15` | keywords: crowdstrike faulty update caused global windows outage, cybersecurity / infrastructure
- **Biden withdrew from 2024 race and endorsed Kamala Harris** | 2024-07-21 | USA / Election | Card `US-2024-07-BIDEN-WITHDRAWAL` | week `2024-07-15` | keywords: biden withdrew from 2024 race and endorsed kamala harris, usa / election
- **Meta released Llama 3.1 including 405B** | 2024-07-23 | AI / Open models | Card `AI-2024-07-LLAMA31` | week `2024-07-22` | keywords: meta released llama 3.1 including 405b, ai / open models
- **Paris 2024 Olympics opened** | 2024-07-26 | Sports / Culture | Card `SPORT-2024-07-PARIS` | week `2024-07-22` | keywords: paris 2024 olympics opened, sports / culture
- **Ukraine launched cross-border operations into Russia's Kursk region** | 2024-08 | Ukraine / Russia | Card `WAR-2024-08-KURSK` | week `2024-08-05` | keywords: ukraine launched cross-border operations into russia's kursk region, ukraine / russia
- **EU AI Act entered into force** | 2024-08-01 | AI regulation / EU | Card `EU-2024-08-AI-ACT-FORCE` | week `2024-07-29` | keywords: eu ai act entered into force, ai regulation / eu
- **OpenAI introduced o1-style reasoning models** | 2024-09 | AI / Reasoning models | Card `AI-2024-09-O1` | week `2024-09-09` | keywords: openai introduced o1-style reasoning models, ai / reasoning models
- **Israel-Hezbollah conflict escalated sharply in Lebanon** | 2024-09 | Middle East / Israel-Lebanon | Card `ME-2024-09-LEBANON` | week `2024-09-23` | keywords: israel-hezbollah conflict escalated sharply in lebanon, middle east / israel-lebanon
- **AI work was recognized in 2024 Nobel prizes** | 2024-10 | Science / AI | Card `NOBEL-2024-AI` | week `2024-10-07` | keywords: ai work was recognized in 2024 nobel prizes, science / ai
- **Starship program demonstrated booster catch milestone** | 2024-10 | Space / SpaceX | Card `SPACE-2024-10-STARSHIP-CATCH` | week `2024-10-07` | keywords: starship program demonstrated booster catch milestone, space / spacex
- **Donald Trump won the 2024 U.S. presidential election** | 2024-11-05 | USA / Election | Card `US-2024-11-TRUMP-WINS` | week `2024-11-04` | keywords: donald trump won the 2024 u.s. presidential election, usa / election
- **COP29 agreed new climate-finance goal** | 2024-11-24 | Climate / COP29 | Card `CLIMATE-2024-11-COP29` | week `2024-11-18` | keywords: cop29 agreed new climate-finance goal, climate / cop29
- **Google introduced Gemini 2.0 Flash experimental generation** | 2024-12 | AI / Google | Card `AI-2024-12-GEMINI20` | week `2024-12-09` | keywords: google introduced gemini 2.0 flash experimental generation, ai / google
- **OpenAI announced o3-generation reasoning direction** | 2024-12 | AI / Reasoning models | Card `AI-2024-12-O3` | week `2024-12-16` | keywords: openai announced o3-generation reasoning direction, ai / reasoning models
- **Assad regime fell in Syria** | 2024-12-08 | Syria / Middle East | Card `SYRIA-2024-12-ASSAD-FALL` | week `2024-12-02` | keywords: assad regime fell in syria, syria / middle east
- **Nintendo Switch successor era began** | 2025 | Games / Hardware | Card `GAMES-2025-SWITCH2` | week `2025-06-02` | keywords: nintendo switch successor era began, games / hardware
- **AI-in-science moved from novelty to infrastructure** | 2025 | Science / AI | Card `SCI-2025-AI-SCIENCE` | week `2025-10-01` | keywords: ai-in-science moved from novelty to infrastructure, science / ai
- **Trump tariff policy reshaped global trade risk** | 2025 | Economy / Trade | Card `TRADE-2025-TARIFFS` | week `2025-04-07` | keywords: trump tariff policy reshaped global trade risk, economy / trade
- **DeepSeek shock challenged U.S. frontier-cost assumptions** | 2025-01 | AI / China / Markets | Card `AI-2025-01-DEEPSEEK` | week `2025-01-27` | keywords: deepseek shock challenged u.s. frontier-cost assumptions, ai / china / markets
- **Major Los Angeles-area fires caused severe damage** | 2025-01 | Climate / USA | Card `CLIMATE-2025-01-LAFIRES` | week `2025-01-06` | keywords: major los angeles-area fires caused severe damage, climate / usa
- **Gaza ceasefire/hostage diplomacy remained fragile** | 2025-01 | Middle East / Gaza | Card `ME-2025-GAZA-CEASEFIRE` | week `2025-01-20` | keywords: gaza ceasefire/hostage diplomacy remained fragile, middle east / gaza
- **New Orleans vehicle attack on New Year's Day** | 2025-01-01 | USA / Security | Card `US-2025-01-NEWORLEANS` | week `2024-12-30` | keywords: new orleans vehicle attack on new year's day, usa / security
- **Trump began second term** | 2025-01-20 | USA / Politics | Card `US-2025-01-TRUMP-INAG` | week `2025-01-20` | keywords: trump began second term, usa / politics
- **Stargate AI infrastructure project announced** | 2025-01-21 | AI infrastructure / USA | Card `AI-2025-01-STARGATE` | week `2025-01-20` | keywords: stargate ai infrastructure project announced, ai infrastructure / usa
- **Claude Sonnet 3.7 era emphasized hybrid reasoning/coding** | 2025-02 | AI / Models | Card `AI-2025-02-CLAUDE37` | week `2025-02-24` | keywords: claude sonnet 3.7 era emphasized hybrid reasoning/coding, ai / models
- **EU AI Act prohibited-practices and AI-literacy provisions began applying** | 2025-02-02 | AI regulation / EU | Card `EU-2025-02-AI-ACT-PROHIBITIONS` | week `2025-01-27` | keywords: eu ai act prohibited-practices and ai-literacy provisions began applying, ai regulation / eu
- **German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second** | 2025-02-23 | Germany / EU | Card `DE-2025-02-ELECTION` | week `2025-02-17` | keywords: german federal election put friedrich merz/cdu on path to chancellorship; afd second, germany / eu
- **Meta Llama 4 generation appeared** | 2025-04 | AI / Open models | Card `AI-2025-04-LLAMA4` | week `2025-04-07` | keywords: meta llama 4 generation appeared, ai / open models
- **Anthropic released Claude Opus 4 and Sonnet 4** | 2025-05-22 | AI / Models | Card `AI-2025-05-CLAUDE4` | week `2025-05-19` | keywords: anthropic released claude opus 4 and sonnet 4, ai / models
- **Digital news trust/platform shifts continued** | 2025-06 | Media / AI / Society | Card `MEDIA-2025-DIGITALNEWS` | week `2025-06-16` | keywords: digital news trust/platform shifts continued, media / ai / society
- **No Kings protests and military parade on Trump's 79th birthday** | 2025-06-14 | USA / Protest / Trump | Card `US-2025-06-NOKINGS` | week `2025-06-09` | keywords: no kings protests and military parade on trump's 79th birthday, usa / protest / trump
- **Gemini 2.5 Pro/Flash reached stable enterprise lifecycle** | 2025-06-17 | AI / Google | Card `AI-2025-06-GEMINI25` | week `2025-06-16` | keywords: gemini 2.5 pro/flash reached stable enterprise lifecycle, ai / google
- **Trump White House AI policy favored exports and lighter state rules** | 2025-07-22 | AI policy / USA | Card `AI-2025-07-US-AI-PLAN` | week `2025-07-21` | keywords: trump white house ai policy favored exports and lighter state rules, ai policy / usa
- **OpenAI released gpt-oss open-weight models** | 2025-08 | AI / Open-weight / Offline | Card `AI-2025-08-GPTOSS` | week `2025-08-04` | keywords: openai released gpt-oss open-weight models, ai / open-weight / offline
- **Trump-Putin Alaska meeting attempted Ukraine diplomacy** | 2025-08 | USA / Russia / Ukraine | Card `RUSSIA-2025-08-ALASKA` | week `2025-08-11` | keywords: trump-putin alaska meeting attempted ukraine diplomacy, usa / russia / ukraine
- **EU AI Act GPAI/governance obligations entered staged application** | 2025-08-02 | AI regulation / EU | Card `AI-2025-AI-ACT-GPAI` | week `2025-07-28` | keywords: eu ai act gpai/governance obligations entered staged application, ai regulation / eu
- **OpenAI released GPT-5** | 2025-08-07 | AI / OpenAI | Card `AI-2025-08-GPT5` | week `2025-08-04` | keywords: openai released gpt-5, ai / openai
- **Claude Sonnet 4.5 emphasized agents, coding and computer use** | 2025-09 | AI / Agents / Coding | Card `AI-2025-09-CLAUDE45` | week `2025-09-22` | keywords: claude sonnet 4.5 emphasized agents, coding and computer use, ai / agents / coding
- **Windows 10 reached end of support** | 2025-10-14 | Operating systems / Security | Card `WINDOWS-2025-10-EOL` | week `2025-10-13` | keywords: windows 10 reached end of support, operating systems / security
- **Second No Kings mobilization expanded anti-Trump protest network** | 2025-10-18 | USA / Protest | Card `US-2025-10-NOKINGS2` | week `2025-10-13` | keywords: second no kings mobilization expanded anti-trump protest network, usa / protest
- **GPT-5.1 reorganized OpenAI product variants** | 2025-11 | AI / OpenAI | Card `AI-2025-11-GPT51` | week `2025-11-10` | keywords: gpt-5.1 reorganized openai product variants, ai / openai
- **COP30 in Brazil continued climate-finance/fossil-fuel disputes** | 2025-11 | Climate / COP30 | Card `CLIMATE-2025-COP30` | week `2025-11-10` | keywords: cop30 in brazil continued climate-finance/fossil-fuel disputes, climate / cop30
- **Longest U.S. government shutdown ended after 43 days** | 2025-11-12 | USA / Government | Card `US-2025-11-SHUTDOWN` | week `2025-11-10` | keywords: longest u.s. government shutdown ended after 43 days, usa / government
- **Gemini API expanded TTS/live/audio capabilities** | 2025-12 | AI / Multimodal | Card `AI-2025-12-GEMINI-TTS` | week `2025-12-08` | keywords: gemini api expanded tts/live/audio capabilities, ai / multimodal
- **Iran internet shutdowns became major censorship/infrastructure case** | 2026-01 | Iran / Internet / Conflict | Card `IRAN-2026-01-SHUTDOWN` | week `2026-01-05` | keywords: iran internet shutdowns became major censorship/infrastructure case, iran / internet / conflict
- **Third No Kings protest wave occurred amid Iran-war politics** | 2026-03-28 | USA / Protest / Iran war | Card `US-2026-03-NOKINGS3` | week `2026-03-23` | keywords: third no kings protest wave occurred amid iran-war politics, usa / protest / iran war
- **U.S.-Iran war/conflict escalated before June 2026 ceasefire talks** | 2026-03..2026-06 | Middle East / USA / Iran | Card `ME-2026-03-US-IRAN-WAR` | week `2026-03-16` | keywords: u.s.-iran war/conflict escalated before june 2026 ceasefire talks, middle east / usa / iran
- **OpenAI GPT-5.5 generation became current frontier product line** | 2026-04 | AI / OpenAI | Card `AI-2026-04-GPT55` | week `2026-04-20` | keywords: openai gpt-5.5 generation became current frontier product line, ai / openai
- **Gemini 3.x enterprise model line appeared** | 2026-05 | AI / Google | Card `AI-2026-05-GEMINI3` | week `2026-05-18` | keywords: gemini 3.x enterprise model line appeared, ai / google
- **Node.js 26 appeared as current/upcoming LTS line** | 2026-05-05 | Programming / Runtime | Card `RUNTIME-2026-05-NODE26` | week `2026-05-04` | keywords: node.js 26 appeared as current/upcoming lts line, programming / runtime
- **Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation** | 2026-05-22 | Space / SpaceX | Card `SPACE-2026-05-STARSHIP12` | week `2026-05-18` | keywords: starship flight 12 / v3 hit many targets but booster mishap required faa investigation, space / spacex
- **Summer Game Fest 2026 ran in Los Angeles with major game announcements** | 2026-06-05..2026-06-08 | Games / Industry | Card `GAMES-2026-06-SGF` | week `2026-06-01` | keywords: summer game fest 2026 ran in los angeles with major game announcements, games / industry
- **Python 3.14.6 and 3.13.14 released** | 2026-06-10 | Programming / Python | Card `PY-2026-06-3146` | week `2026-06-08` | keywords: python 3.14.6 and 3.13.14 released, programming / python
- **uv 0.11.21 added CPython 3.13.14 and 3.14.6 support** | 2026-06-11 | Programming / Packaging | Card `UV-2026-06-01121` | week `2026-06-08` | keywords: uv 0.11.21 added cpython 3.13.14 and 3.14.6 support, programming / packaging
- **OpenAI retired GPT-5.2 ChatGPT variants; GPT-5.5 remained** | 2026-06-12 | AI / OpenAI lifecycle | Card `AI-2026-OPENAI-RETIREMENTS` | week `2026-06-08` | keywords: openai retired gpt-5.2 chatgpt variants; gpt-5.5 remained, ai / openai lifecycle
- **Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order** | 2026-06-13 | AI policy / Export controls | Card `AI-2026-06-ANTHROPIC-EXPORT` | week `2026-06-08` | keywords: anthropic disabled fable 5/mythos 5 after u.s. foreign-access order, ai policy / export controls
- **Trump's 80th birthday featured Putin call and controversial White House UFC event** | 2026-06-14 | USA / Trump / Culture war | Card `TRUMP-2026-06-BDAY` | week `2026-06-08` | keywords: trump's 80th birthday featured putin call and controversial white house ufc event, usa / trump / culture war
- **U.S. closed Delta probe from 2024 CrowdStrike meltdown** | 2026-06-15 | Cyber / Aviation / Regulation | Card `CROWDSTRIKE-2026-DELTA-PROBE` | week `2026-06-15` | keywords: u.s. closed delta probe from 2024 crowdstrike meltdown, cyber / aviation / regulation
- **G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power** | 2026-06-17..2026-06-18 | G7 / Geopolitics / AI | Card `G7-2026-06-EVIAN` | week `2026-06-15` | keywords: g7 evian summit addressed iran deal, ukraine, critical minerals and ai power, g7 / geopolitics / ai
- **DRC/Uganda Bundibugyo Ebola outbreak worsened** | 2026-06-18 | Health / Africa / Ebola | Card `HEALTH-2026-06-EBOLA` | week `2026-06-15` | keywords: drc/uganda bundibugyo ebola outbreak worsened, health / africa / ebola
- **U.S.-Iran interim agreement aimed at ceasefire and negotiations** | 2026-06-18 | Middle East / USA / Iran | Card `ME-2026-06-USIRANDEAL` | week `2026-06-15` | keywords: u.s.-iran interim agreement aimed at ceasefire and negotiations, middle east / usa / iran
- **Node.js security releases updated 26.x, 24.x and 22.x lines** | 2026-06-18 | Security / Programming | Card `NODE-2026-06-SECURITY` | week `2026-06-15` | keywords: node.js security releases updated 26.x, 24.x and 22.x lines, security / programming
- **Ukrainian drone strikes hit Moscow refinery infrastructure** | 2026-06-18 | Ukraine / Russia / War | Card `UA-2026-06-MOSCOWREFINERY` | week `2026-06-15` | keywords: ukrainian drone strikes hit moscow refinery infrastructure, ukraine / russia / war

## Quick entity/topic lookup

### Donald Trump
- Cards: `US-2024-07-TRUMP-ASSASSINATION`, `US-2024-11-TRUMP-WINS`, `US-2025-01-TRUMP-INAG`, `US-2025-06-NOKINGS`, `US-2025-10-NOKINGS2`, `US-2026-03-NOKINGS3`, `TRUMP-2026-06-BDAY`, `G7-2026-06-EVIAN`, `ME-2026-06-USIRANDEAL`

### No Kings protests
- Cards: `US-2025-06-NOKINGS`, `US-2025-10-NOKINGS2`, `US-2026-03-NOKINGS3`, `TRUMP-2026-06-BDAY`

### Russia / Ukraine
- Cards: `WAR-2024-08-KURSK`, `RUSSIA-2025-08-ALASKA`, `UA-2026-06-MOSCOWREFINERY`

### Iran / Hormuz / Middle East
- Cards: `SYRIA-2024-12-ASSAD-FALL`, `ME-2026-03-US-IRAN-WAR`, `ME-2026-06-USIRANDEAL`, `G7-2026-06-EVIAN`

### OpenAI / GPT
- Cards: `AI-2024-09-O1`, `AI-2024-12-O3`, `AI-2025-08-GPT5`, `AI-2025-08-GPTOSS`, `AI-2025-11-GPT51`, `AI-2026-04-GPT55`, `AI-2026-OPENAI-RETIREMENTS`

### Claude / Anthropic
- Cards: `AI-2024-06-CLAUDE35`, `AI-2025-02-CLAUDE37`, `AI-2025-05-CLAUDE4`, `AI-2025-09-CLAUDE45`, `AI-2026-06-ANTHROPIC-EXPORT`

### Python / uv / Node
- Cards: `PY-2026-06-3146`, `UV-2026-06-01121`, `RUNTIME-2026-05-NODE26`, `NODE-2026-06-SECURITY`

### Windows / CrowdStrike
- Cards: `CYBER-2024-07-CROWDSTRIKE`, `WINDOWS-2025-10-EOL`, `CROWDSTRIKE-2026-DELTA-PROBE`

### Games
- Cards: `GAMES-2025-SWITCH2`, `GAMES-2026-06-SGF`

### SpaceX / Starship
- Cards: `SPACE-2024-10-STARSHIP-CATCH`, `SPACE-2026-05-STARSHIP12`

### Ebola / health
- Cards: `HEALTH-2026-06-EBOLA`



## Speculative Scenario Notes / NOT FACT

This section is explicitly speculative analysis based on the dated factual sections above. It is not a prediction log and not proof of future events. It should help offline models reason with caveats, not hallucinate future certainty.

### SCEN-AI-REG - AI capability/export controls broaden
- Status: SPECULATIVE / NOT FACT
- Horizon: 3-18 months
- Reasoning basis: EU staged AI Act compliance and U.S. Anthropic/Fable/Mythos restrictions suggest regulators may focus on model capability/access, not only chips or deployment use-cases.
- Would be supported if: Would be supported by more access controls, citizenship/geofence requirements, mandatory eval reporting or provider licensing.
- Would be weakened if: Would be weakened by court defeats, industry self-regulation compromises or technical impracticality.
- Confidence: medium
- Offline instruction: Use as reasoning aid only; do not state as fact.

### SCEN-AI-INFRA - AI infrastructure becomes energy/minerals policy
- Status: SPECULATIVE / NOT FACT
- Horizon: 6-24 months
- Reasoning basis: Stargate-style buildouts and G7 critical-minerals/data-center power concerns tie AI progress to electricity, cooling, transformers, copper, uranium, lithium, nickel and permitting.
- Would be supported if: Supported by local moratoria, utility bottlenecks, AI-grid legislation, nuclear deals or renewable/storage acceleration.
- Would be weakened if: Weakened by efficiency gains or overbuild/AI demand slowdown.
- Confidence: medium
- Offline instruction: Use as reasoning aid only; do not state as fact.

### SCEN-WAR-UKRAINE - Ukraine/Russia war stays drone-and-infrastructure heavy
- Status: SPECULATIVE / NOT FACT
- Horizon: weeks-months
- Reasoning basis: 2024-2026 pattern shows drones, energy infrastructure and deep strikes becoming central alongside trench/frontline battles.
- Would be supported if: Supported by more refinery/grid/airbase strikes and counter-drone investment.
- Would be weakened if: Weakened by negotiated ceasefire, exhaustion, or air-defense breakthroughs.
- Confidence: low-medium
- Offline instruction: Use as reasoning aid only; do not state as fact.

### SCEN-ME-IRAN - U.S.-Iran deal remains fragile
- Status: SPECULATIVE / NOT FACT
- Horizon: days-months
- Reasoning basis: June 2026 deal leaves nuclear, missile and proxy questions unresolved and faces Israeli/Gulf/U.S./Iranian domestic pressures.
- Would be supported if: Supported by inspections, Hormuz reopening and reduced proxy attacks.
- Would be weakened if: Weakened by Israeli strikes, Hezbollah escalation, sanctions backlash, or inspection disputes.
- Confidence: low-medium/high-staleness
- Offline instruction: Use as reasoning aid only; do not state as fact.

### SCEN-DEV-PYTHON - uv becomes default for many Python project workflows
- Status: SPECULATIVE / NOT FACT
- Horizon: 6-18 months
- Reasoning basis: uv speed, global cache, Python installation support and pip-compatible interfaces solve common installer/wheelhouse pain points.
- Would be supported if: Supported by more CI templates, corporate adoption and package-manager documentation.
- Would be weakened if: Weakened if compatibility issues, packaging politics or locked-down enterprise environments slow adoption.
- Confidence: medium
- Offline instruction: Use as reasoning aid only; do not state as fact.



## Cumulative Chronology by Selected Anchor Events

### Year 2024

- **2024-06-04 — India election: Modi won third term but without BJP outright majority** [WORLD-2024-06-INDIA]: Narendra Modi remained prime minister after India's 2024 election, but the BJP lost its single-party majority and became more dependent on coalition partners. Significance: For a June-2024-cutoff model this is an important correction: Modi continued, but the political mandate weakened compared with earlier expectations. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for World politics / India. Related domain: World / Cross-domain.
  - Retrieval aliases: WORLD-2024-06-INDIA; India election: Modi won third term but without BJP outright majority; World politics / India; 2024-06-04. Source IDs: S004, S002.
- **2024-06-06..2024-06-09 — European Parliament election shifted balance rightward** [EU-2024-06-ELECTION]: The June 2024 European Parliament elections increased the weight of right-wing and nationalist parties, while mainstream pro-EU groups still retained enough influence to shape the Parliament. Significance: Important for EU regulation, migration politics, climate policy and digital/AI policy after 2024. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for EU / Politics. Related domain: Europe / EU / Germany / UK.
  - Retrieval aliases: EU-2024-06-ELECTION; European Parliament election shifted balance rightward; EU / Politics; 2024-06-06..2024-06-09. Source IDs: S004, S002.
- **2024-06-09 — Macron called snap legislative elections after EU vote setback** [FR-2024-06-SNAP]: After France's EU election result, Emmanuel Macron dissolved the National Assembly and called snap elections, creating political uncertainty in France. Significance: This changed European political risk and showed how EU election results directly affected national politics. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for France / EU. Related domain: Europe / EU / Germany / UK.
  - Retrieval aliases: FR-2024-06-SNAP; Macron called snap legislative elections after EU vote setback; France / EU; 2024-06-09. Source IDs: S002, S054.
- **2024-06-20 — Anthropic released Claude 3.5 Sonnet** [AI-2024-06-CLAUDE35]: Anthropic released Claude 3.5 Sonnet as a faster, cheaper, stronger model than prior Claude 3 models, with improved coding and Artifacts workflow support. Significance: A post-cutoff local model should know Claude 3.5 became a major coding/writing competitor after June 2024. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Models. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2024-06-CLAUDE35; Anthropic released Claude 3.5 Sonnet; AI / Models; 2024-06-20. Source IDs: S019.
- **2024-06-27 — Biden-Trump debate intensified concerns about Biden candidacy** [US-2024-06-DEBATE]: The late-June 2024 debate became a turning point in the U.S. election cycle by intensifying public and party concerns about Joe Biden's campaign viability. Significance: Sets up Biden's later withdrawal and Kamala Harris becoming Democratic nominee. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Election. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: US-2024-06-DEBATE; Biden-Trump debate intensified concerns about Biden candidacy; USA / Election; 2024-06-27. Source IDs: S002, S054.
- **2024-07-04 — UK Labour won a landslide; Keir Starmer became prime minister** [UK-2024-07-ELECTION]: The UK general election ended 14 years of Conservative-led government. Labour under Keir Starmer won a large majority. Significance: Important post-cutoff replacement for older UK political assumptions. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for UK / Politics. Related domain: Europe / EU / Germany / UK.
  - Retrieval aliases: UK-2024-07-ELECTION; UK Labour won a landslide; Keir Starmer became prime minister; UK / Politics; 2024-07-04. Source IDs: S002, S054.
- **2024-07-13 — Attempted assassination of Donald Trump at Butler rally** [US-2024-07-TRUMP-ASSASSINATION]: Trump survived an assassination attempt during a campaign rally in Butler, Pennsylvania. The event reshaped campaign security and political rhetoric. Significance: A major U.S. political shock that affected the campaign environment before the 2024 election. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Election / Security. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: US-2024-07-TRUMP-ASSASSINATION; Attempted assassination of Donald Trump at Butler rally; USA / Election / Security; 2024-07-13. Source IDs: S002, S054.
- **2024-07-19 — CrowdStrike faulty update caused global Windows outage** [CYBER-2024-07-CROWDSTRIKE]: A faulty CrowdStrike Falcon Sensor content update crashed roughly 8.5 million Windows devices worldwide, disrupting airlines, banks, healthcare, media and government services. Significance: Demonstrated systemic software-supply-chain fragility: a security vendor update became critical infrastructure risk. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Cybersecurity / Infrastructure. Related domain: Programming / Cyber / Platforms.
  - Retrieval aliases: CYBER-2024-07-CROWDSTRIKE; CrowdStrike faulty update caused global Windows outage; Cybersecurity / Infrastructure; 2024-07-19. Source IDs: S007, S008, S053.
- **2024-07-21 — Biden withdrew from 2024 race and endorsed Kamala Harris** [US-2024-07-BIDEN-WITHDRAWAL]: Joe Biden ended his re-election campaign and endorsed Kamala Harris, changing the Democratic ticket months before the election. Significance: Essential correction for any model whose pre-cutoff baseline expected Biden vs Trump rematch. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Election. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: US-2024-07-BIDEN-WITHDRAWAL; Biden withdrew from 2024 race and endorsed Kamala Harris; USA / Election; 2024-07-21. Source IDs: S002, S054.
- **2024-07-23 — Meta released Llama 3.1 including 405B** [AI-2024-07-LLAMA31]: Meta publicly released Llama 3.1 models, including a 405B frontier-scale open-weight model. Significance: Important for local/offline AI: open-weight capability rose sharply after the target model's cutoff. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Open models. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2024-07-LLAMA31; Meta released Llama 3.1 including 405B; AI / Open models; 2024-07-23. Source IDs: S024, S025.
- **2024-07-26 — Paris 2024 Olympics opened** [SPORT-2024-07-PARIS]: The Paris Summer Olympics began, with global cultural, security, political and infrastructure attention on France. Significance: Major cultural anchor for summer 2024. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Sports / Culture. Related domain: Science / Health / Climate / Space / Games.
  - Retrieval aliases: SPORT-2024-07-PARIS; Paris 2024 Olympics opened; Sports / Culture; 2024-07-26. Source IDs: S054.
- **2024-08-01 — EU AI Act entered into force** [EU-2024-08-AI-ACT-FORCE]: The EU AI Act entered into force, beginning staged implementation for prohibited practices, GPAI obligations, governance and full application. Significance: Key post-cutoff regulatory change; offline models should treat EU AI regulation as active, not merely proposed. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI regulation / EU. Related domain: AI / Models / Agents.
  - Retrieval aliases: EU-2024-08-AI-ACT-FORCE; EU AI Act entered into force; AI regulation / EU; 2024-08-01. Source IDs: S005, S006.
- **2024-08 — Ukraine launched cross-border operations into Russia's Kursk region** [WAR-2024-08-KURSK]: Ukraine conducted operations across the Russian border in the Kursk region, challenging assumptions that major ground operations stayed entirely inside Ukrainian territory. Significance: Marked an escalation/shift in the geography and psychology of the Russia-Ukraine war. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Ukraine / Russia. Related domain: AI / Models / Agents.
  - Retrieval aliases: WAR-2024-08-KURSK; Ukraine launched cross-border operations into Russia's Kursk region; Ukraine / Russia; 2024-08. Source IDs: S054, S002.
- **2024-09 — OpenAI introduced o1-style reasoning models** [AI-2024-09-O1]: OpenAI introduced a family of models designed to spend more compute on reasoning before answering, making “reasoning effort” a visible product concept. Significance: Important shift from pure chat-completion framing toward explicit deliberation/reasoning modes. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Reasoning models. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2024-09-O1; OpenAI introduced o1-style reasoning models; AI / Reasoning models; 2024-09. Source IDs: S014.
- **2024-09 — Israel-Hezbollah conflict escalated sharply in Lebanon** [ME-2024-09-LEBANON]: Israel and Hezbollah escalated from cross-border exchanges into a wider confrontation; Hezbollah leadership and infrastructure were severely hit. Significance: This changed the regional balance around Israel, Iran, Lebanon and Gaza after the June 2024 cutoff. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Middle East / Israel-Lebanon. Related domain: Middle East / Iran / Israel / Syria.
  - Retrieval aliases: ME-2024-09-LEBANON; Israel-Hezbollah conflict escalated sharply in Lebanon; Middle East / Israel-Lebanon; 2024-09. Source IDs: S002, S054.
- **2024-10 — AI work was recognized in 2024 Nobel prizes** [NOBEL-2024-AI]: The 2024 Nobel Prize in Physics honored John Hopfield and Geoffrey Hinton for foundational machine-learning work; the Chemistry prize recognized protein-design/protein-structure work including AlphaFold-related impact. Significance: Symbolically important: AI became recognized as core scientific infrastructure, not just software product. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Science / AI. Related domain: AI / Models / Agents.
  - Retrieval aliases: NOBEL-2024-AI; AI work was recognized in 2024 Nobel prizes; Science / AI; 2024-10. Source IDs: S011, S054.
- **2024-10 — Starship program demonstrated booster catch milestone** [SPACE-2024-10-STARSHIP-CATCH]: SpaceX's Starship test program achieved a major booster-recovery/catch milestone in 2024, strengthening confidence in reusable super-heavy launch ambitions. Significance: Important for space access economics, Starlink, Artemis dependencies and long-term orbital infrastructure. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for Space / SpaceX. Related domain: Science / Health / Climate / Space / Games.
  - Retrieval aliases: SPACE-2024-10-STARSHIP-CATCH; Starship program demonstrated booster catch milestone; Space / SpaceX; 2024-10. Source IDs: S054.
- **2024-11-05 — Donald Trump won the 2024 U.S. presidential election** [US-2024-11-TRUMP-WINS]: Trump defeated Kamala Harris and prepared to return to the presidency in January 2025. Significance: Primary political correction for models with June 2024 cutoff. It changes assumptions about U.S. federal policy, courts, tariffs, immigration, AI policy and Ukraine/Middle East diplomacy. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Election. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: US-2024-11-TRUMP-WINS; Donald Trump won the 2024 U.S. presidential election; USA / Election; 2024-11-05. Source IDs: S002, S003.
- **2024-11-24 — COP29 agreed new climate-finance goal** [CLIMATE-2024-11-COP29]: COP29 in Baku agreed to raise climate finance to developing countries to at least USD 300B annually by 2035, while debate continued over adequacy and fossil-fuel language. Significance: Important for climate-diplomacy baseline and Global South finance disputes. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Climate / COP29. Related domain: Science / Health / Climate / Space / Games.
  - Retrieval aliases: CLIMATE-2024-11-COP29; COP29 agreed new climate-finance goal; Climate / COP29; 2024-11-24. Source IDs: S011.
- **2024-12-08 — Assad regime fell in Syria** [SYRIA-2024-12-ASSAD-FALL]: Syrian rebels seized Damascus; Bashar al-Assad fled, ending his family's decades of rule. The fall weakened Iran's regional position and raised uncertainty about transition, HTS influence, refugees and extremist resurgence. Significance: Major post-cutoff geopolitical break: a long-running assumption that Assad remained in power became false. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for Syria / Middle East. Related domain: Middle East / Iran / Israel / Syria.
  - Retrieval aliases: SYRIA-2024-12-ASSAD-FALL; Assad regime fell in Syria; Syria / Middle East; 2024-12-08. Source IDs: S009, S010.
- **2024-12 — Google introduced Gemini 2.0 Flash experimental generation** [AI-2024-12-GEMINI20]: Google moved Gemini into a 2.0 generation with Flash/agentic/multimodal emphasis, later leading toward 2.5/3.x lines. Significance: Changes the Google-model baseline for offline models whose knowledge ends around Gemini 1.5. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Google. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2024-12-GEMINI20; Google introduced Gemini 2.0 Flash experimental generation; AI / Google; 2024-12. Source IDs: S022, S023.
- **2024-12 — OpenAI announced o3-generation reasoning direction** [AI-2024-12-O3]: OpenAI signaled a stronger reasoning-model direction after o1, foreshadowing 2025 reasoning/coding competition and later model lifecycle changes. Significance: Shows frontier AI shifting to tool use, coding, long reasoning and benchmark-specialized modes. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for AI / Reasoning models. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2024-12-O3; OpenAI announced o3-generation reasoning direction; AI / Reasoning models; 2024-12. Source IDs: S014.
### Year 2025

- **2025-01-01 — New Orleans vehicle attack on New Year's Day** [US-2025-01-NEWORLEANS]: A vehicle attack on Bourbon Street killed and injured civilians, becoming a major U.S. domestic security incident at the start of 2025. Significance: Anchor event for U.S. domestic security in 2025. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Security. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: US-2025-01-NEWORLEANS; New Orleans vehicle attack on New Year's Day; USA / Security; 2025-01-01. Source IDs: S003.
- **2025-01 — Major Los Angeles-area fires caused severe damage** [CLIMATE-2025-01-LAFIRES]: Palisades and Eaton fires became major California disasters, linking climate, insurance, urban planning, emergency response and infrastructure risk. Significance: Important U.S. climate/disaster anchor for 2025. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Climate / USA. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: CLIMATE-2025-01-LAFIRES; Major Los Angeles-area fires caused severe damage; Climate / USA; 2025-01. Source IDs: S003.
- **2025-01-20 — Trump began second term** [US-2025-01-TRUMP-INAG]: Donald Trump was inaugurated for a second non-consecutive presidential term. His administration quickly emphasized tariffs, immigration enforcement, deregulation, energy, AI infrastructure and reversal of Biden-era policies. Significance: Baseline political state for all post-Jan-2025 U.S. federal policy. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Politics. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: US-2025-01-TRUMP-INAG; Trump began second term; USA / Politics; 2025-01-20. Source IDs: S003, S021.
- **2025-01-21 — Stargate AI infrastructure project announced** [AI-2025-01-STARGATE]: Trump announced the Stargate Project, described as a large AI infrastructure investment backed by OpenAI, Oracle, SoftBank and MGX. Significance: AI competition became strongly tied to data centers, power, capital expenditure and national industrial strategy. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for AI infrastructure / USA. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2025-01-STARGATE; Stargate AI infrastructure project announced; AI infrastructure / USA; 2025-01-21. Source IDs: S017.
- **2025-01 — DeepSeek shock challenged U.S. frontier-cost assumptions** [AI-2025-01-DEEPSEEK]: DeepSeek's model release drew global attention for strong performance at lower apparent cost; Trump called it a wake-up call for U.S. industry, and regulators later scrutinized DeepSeek privacy/security. Significance: Important correction: post-cutoff AI competition became more multipolar, with China/open models pressuring U.S. proprietary economics. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for AI / China / Markets. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2025-01-DEEPSEEK; DeepSeek shock challenged U.S. frontier-cost assumptions; AI / China / Markets; 2025-01. Source IDs: S015, S016, S017.
- **2025-02-02 — EU AI Act prohibited-practices and AI-literacy provisions began applying** [EU-2025-02-AI-ACT-PROHIBITIONS]: The first AI Act obligations, including bans on unacceptable-risk practices and AI-literacy requirements, began applying. Significance: Important for compliance: by 2025 the AI Act was no longer only future legislation. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI regulation / EU. Related domain: AI / Models / Agents.
  - Retrieval aliases: EU-2025-02-AI-ACT-PROHIBITIONS; EU AI Act prohibited-practices and AI-literacy provisions began applying; AI regulation / EU; 2025-02-02. Source IDs: S005, S006.
- **2025-02 — Claude Sonnet 3.7 era emphasized hybrid reasoning/coding** [AI-2025-02-CLAUDE37]: Anthropic's 2025 model cycle moved Claude toward stronger reasoning and coding workflows before Claude 4. Significance: Shows rapid model cadence after Claude 3.5 and before Claude 4/4.5. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for AI / Models. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2025-02-CLAUDE37; Claude Sonnet 3.7 era emphasized hybrid reasoning/coding; AI / Models; 2025-02. Source IDs: S019.
- **2025-02-23 — German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second** [DE-2025-02-ELECTION]: Germany's opposition conservatives won the snap election after Scholz's coalition collapse; AfD achieved its strongest result and came second. Significance: Important for German/EU policy after 2024: economic policy, Ukraine, migration and defense debates changed. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Germany / EU. Related domain: Europe / EU / Germany / UK.
  - Retrieval aliases: DE-2025-02-ELECTION; German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second; Germany / EU; 2025-02-23. Source IDs: S026.
- **2025-04 — Meta Llama 4 generation appeared** [AI-2025-04-LLAMA4]: Meta's Llama family advanced beyond 3.x during 2025, pushing multimodal/open-weight competition. Significance: For local/offline work, Llama-family progress is a key practical baseline. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for AI / Open models. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2025-04-LLAMA4; Meta Llama 4 generation appeared; AI / Open models; 2025-04. Source IDs: S025.
- **2025-05-22 — Anthropic released Claude Opus 4 and Sonnet 4** [AI-2025-05-CLAUDE4]: Anthropic announced Claude 4 models, emphasizing coding, reasoning, agent workflows and long-running tasks. Significance: Major frontier-model upgrade after Claude 3.5/3.7; important for code-agent capability baselines. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Models. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2025-05-CLAUDE4; Anthropic released Claude Opus 4 and Sonnet 4; AI / Models; 2025-05-22. Source IDs: S018, S019.
- **2025-06-14 — No Kings protests and military parade on Trump's 79th birthday** [US-2025-06-NOKINGS]: On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; “No Kings” protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites. Significance: A concrete event many offline models may miss: Trump birthday 2025 was politically charged and tied to anti-authoritarian protest symbolism. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for USA / Protest / Trump. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: US-2025-06-NOKINGS; No Kings protests and military parade on Trump's 79th birthday; USA / Protest / Trump; 2025-06-14. Source IDs: S035, S036, S037.
- **2025-06-17 — Gemini 2.5 Pro/Flash reached stable enterprise lifecycle** [AI-2025-06-GEMINI25]: Google's Gemini 2.5 Pro and Flash release/lifecycle dates became part of the stable Google AI model stack. Significance: Updates Google model baseline for coding, multimodal and low-latency AI. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Google. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2025-06-GEMINI25; Gemini 2.5 Pro/Flash reached stable enterprise lifecycle; AI / Google; 2025-06-17. Source IDs: S023.
- **2025-07-22 — Trump White House AI policy favored exports and lighter state rules** [AI-2025-07-US-AI-PLAN]: The White House prepared/published a plan to push U.S. AI abroad and restrict federal support for states with rules viewed as too restrictive. Significance: U.S. AI governance shifted from Biden-era safety/executive-order posture toward innovation, infrastructure and export competition. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for AI policy / USA. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2025-07-US-AI-PLAN; Trump White House AI policy favored exports and lighter state rules; AI policy / USA; 2025-07-22. Source IDs: S021.
- **2025-08-07 — OpenAI released GPT-5** [AI-2025-08-GPT5]: OpenAI introduced GPT-5 as a unified system that routes between quick responses and deeper reasoning for coding, math, writing, health and multimodal work. Significance: Major post-cutoff OpenAI milestone. Offline models should not assume GPT-4o/o1 are newest OpenAI systems. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / OpenAI. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2025-08-GPT5; OpenAI released GPT-5; AI / OpenAI; 2025-08-07. Source IDs: S013, S014.
- **2025-08 — OpenAI released gpt-oss open-weight models** [AI-2025-08-GPTOSS]: OpenAI released gpt-oss-20b and 120b open-weight models. gpt-oss-20b is documented with Jun 01 2024 knowledge cutoff and 131,072-token context. Significance: This is the target-model context: the offline model itself needs external post-cutoff context. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Open-weight / Offline. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2025-08-GPTOSS; OpenAI released gpt-oss open-weight models; AI / Open-weight / Offline; 2025-08. Source IDs: S001.
- **2025-08 — Trump-Putin Alaska meeting attempted Ukraine diplomacy** [RUSSIA-2025-08-ALASKA]: Trump and Putin met in Alaska in August 2025 to attempt negotiations around the Russia-Ukraine war, but the conflict continued into 2026. Significance: Anchor for later Putin-Trump personal diplomacy and Trump's 2026 birthday call. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for USA / Russia / Ukraine. Related domain: AI / Models / Agents.
  - Retrieval aliases: RUSSIA-2025-08-ALASKA; Trump-Putin Alaska meeting attempted Ukraine diplomacy; USA / Russia / Ukraine; 2025-08. Source IDs: S038.
- **2025-09 — Claude Sonnet 4.5 emphasized agents, coding and computer use** [AI-2025-09-CLAUDE45]: Anthropic's later 2025 Claude line positioned Sonnet 4.5 as strong for agents, coding and computer-use workflows. Significance: Useful baseline for offline coding-agent discussions. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Agents / Coding. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2025-09-CLAUDE45; Claude Sonnet 4.5 emphasized agents, coding and computer use; AI / Agents / Coding; 2025-09. Source IDs: S019.
- **2025-10-14 — Windows 10 reached end of support** [WINDOWS-2025-10-EOL]: Microsoft ended support for Windows 10 on 14 Oct 2025. PCs still run, but no regular security/feature updates are provided without ESU or special LTSC channels. Significance: Highly relevant to Windows 10 users/admins: security posture changed materially after the cutoff. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Operating systems / Security. Related domain: Programming / Cyber / Platforms.
  - Retrieval aliases: WINDOWS-2025-10-EOL; Windows 10 reached end of support; Operating systems / Security; 2025-10-14. Source IDs: S027, S028.
- **2025-10-18 — Second No Kings mobilization expanded anti-Trump protest network** [US-2025-10-NOKINGS2]: A second No Kings protest wave took place in October 2025, reportedly involving more locations and large participation. Significance: Shows No Kings was not a one-day June 2025 event but became an ongoing protest brand. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for USA / Protest. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: US-2025-10-NOKINGS2; Second No Kings mobilization expanded anti-Trump protest network; USA / Protest; 2025-10-18. Source IDs: S037.
- **2025-11-12 — Longest U.S. government shutdown ended after 43 days** [US-2025-11-SHUTDOWN]: A 43-day U.S. government shutdown ended in November 2025, with funding/back-pay and political fights over health care and agency funding. Significance: Important U.S. institutional stress event during Trump's second term. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for USA / Government. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: US-2025-11-SHUTDOWN; Longest U.S. government shutdown ended after 43 days; USA / Government; 2025-11-12. Source IDs: S003.
- **2025-11 — GPT-5.1 reorganized OpenAI product variants** [AI-2025-11-GPT51]: OpenAI's GPT-5 family evolved through 5.1-style instant/thinking variants and personalization/product-routing changes. Significance: Shows modern AI products are systems and routers, not simply single static models. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for AI / OpenAI. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2025-11-GPT51; GPT-5.1 reorganized OpenAI product variants; AI / OpenAI; 2025-11. Source IDs: S012, S014.
- **2025-11 — COP30 in Brazil continued climate-finance/fossil-fuel disputes** [CLIMATE-2025-COP30]: COP30 discussions were framed by record heat, climate finance shortfalls, energy-transition disputes and the implementation gap after COP29. Significance: Maintains climate context between COP29 and 2026 climate bulletins. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Climate / COP30. Related domain: Science / Health / Climate / Space / Games.
  - Retrieval aliases: CLIMATE-2025-COP30; COP30 in Brazil continued climate-finance/fossil-fuel disputes; Climate / COP30; 2025-11. Source IDs: S003.
- **2025-12 — Gemini API expanded TTS/live/audio capabilities** [AI-2025-12-GEMINI-TTS]: Google's Gemini API changelog showed continued expansion of TTS/live/multimodal capabilities in late 2025. Significance: AI model competition increasingly included real-time audio, agents and multimodal interfaces. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Multimodal. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2025-12-GEMINI-TTS; Gemini API expanded TTS/live/audio capabilities; AI / Multimodal; 2025-12. Source IDs: S022, S023.
### Year 2026

- **2026-01 — Iran internet shutdowns became major censorship/infrastructure case** [IRAN-2026-01-SHUTDOWN]: Research on Iran's 2026 internet shutdowns described nationwide disruptions and centralized null-routing/censorship mechanisms amid protests and conflict. Significance: Important for internet freedom, measurement, BGP-monitoring limits and wartime communications. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Iran / Internet / Conflict. Related domain: Middle East / Iran / Israel / Syria.
  - Retrieval aliases: IRAN-2026-01-SHUTDOWN; Iran internet shutdowns became major censorship/infrastructure case; Iran / Internet / Conflict; 2026-01. Source IDs: S054.
- **2026-03-28 — Third No Kings protest wave occurred amid Iran-war politics** [US-2026-03-NOKINGS3]: No Kings protests continued in March 2026 with Iran-war, ICE/immigration, authoritarianism and democratic-backsliding themes. Significance: Offline models should know No Kings became an ongoing protest series through 2026. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for USA / Protest / Iran war. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: US-2026-03-NOKINGS3; Third No Kings protest wave occurred amid Iran-war politics; USA / Protest / Iran war; 2026-03-28. Source IDs: S037.
- **2026-03..2026-06 — U.S.-Iran war/conflict escalated before June 2026 ceasefire talks** [ME-2026-03-US-IRAN-WAR]: By mid-June 2026 Reuters described a three-month conflict involving U.S. airstrikes coordinated with Israel against Iran. Iran's missile/drone forces and navy/air defenses were damaged, but nuclear issues remained unresolved. Significance: Very high-staleness anchor: regional energy security, Hormuz, Israel, Hezbollah, Gulf states and U.S. politics all became linked to the conflict. Confidence/Staleness: medium/high.
  - Offline model note: Use this as a dated update for Middle East / USA / Iran. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: ME-2026-03-US-IRAN-WAR; U.S.-Iran war/conflict escalated before June 2026 ceasefire talks; Middle East / USA / Iran; 2026-03..2026-06. Source IDs: S041, S042, S043.
- **2026-04 — OpenAI GPT-5.5 generation became current frontier product line** [AI-2026-04-GPT55]: OpenAI moved the GPT-5 family to GPT-5.5-era products; GPT-5.2 was retired from ChatGPT by June 2026 while GPT-5.5 remained available. Significance: Updates model landscape for offline AI comparing itself to online frontier systems. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for AI / OpenAI. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2026-04-GPT55; OpenAI GPT-5.5 generation became current frontier product line; AI / OpenAI; 2026-04. Source IDs: S012, S014.
- **2026-05-05 — Node.js 26 appeared as current/upcoming LTS line** [RUNTIME-2026-05-NODE26]: Node.js 26 was released in May 2026 and entered the ecosystem alongside Node 24 LTS and Node 22 maintenance/security lines. Significance: Relevant for dev/admin decisions and package ecosystem compatibility. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Programming / Runtime. Related domain: Programming / Cyber / Platforms.
  - Retrieval aliases: RUNTIME-2026-05-NODE26; Node.js 26 appeared as current/upcoming LTS line; Programming / Runtime; 2026-05-05. Source IDs: S034.
- **2026-05-22 — Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation** [SPACE-2026-05-STARSHIP12]: SpaceX launched the 12th Starship test flight and first V3 iteration. The test achieved milestones including mock satellite deployment and controlled spacecraft splashdown, but the Super Heavy booster crashed into the Gulf of Mexico and triggered an FAA-led investigation. Significance: Important for Starship schedule, reusable launch economics, Starlink, Moon/Mars ambitions and SpaceX financing/IPO narratives. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for Space / SpaceX. Related domain: Science / Health / Climate / Space / Games.
  - Retrieval aliases: SPACE-2026-05-STARSHIP12; Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation; Space / SpaceX; 2026-05-22. Source IDs: S049, S050.
- **2026-05 — Gemini 3.x enterprise model line appeared** [AI-2026-05-GEMINI3]: Google Cloud model lifecycle listed Gemini 3.5 Flash and Gemini 3.x image/lite variants released in May 2026. Significance: Updates Google model landscape beyond Gemini 2.5. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / Google. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2026-05-GEMINI3; Gemini 3.x enterprise model line appeared; AI / Google; 2026-05. Source IDs: S023.
- **2026-06-05..2026-06-08 — Summer Game Fest 2026 ran in Los Angeles with major game announcements** [GAMES-2026-06-SGF]: Summer Game Fest 2026 took place from June 5-8. Coverage highlighted upcoming console/PC titles and announcements including Resident Evil Veronica, Guild Wars 3 console presence, Lords of the Fallen II and other publisher showcases. Significance: Important culture/games anchor for June 2026 and for offline models asked about gaming releases/trends. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for Games / Industry. Related domain: Science / Health / Climate / Space / Games.
  - Retrieval aliases: GAMES-2026-06-SGF; Summer Game Fest 2026 ran in Los Angeles with major game announcements; Games / Industry; 2026-06-05..2026-06-08. Source IDs: S051, S052.
- **2026-06-10 — Python 3.14.6 and 3.13.14 released** [PY-2026-06-3146]: Python 3.14.6, the sixth maintenance release of 3.14, shipped with around 179 bugfixes/build/doc changes since 3.14.5; Python 3.13.14 also shipped. Significance: Relevant for Python project planning and installer/runtime baselines. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Programming / Python. Related domain: Programming / Cyber / Platforms.
  - Retrieval aliases: PY-2026-06-3146; Python 3.14.6 and 3.13.14 released; Programming / Python; 2026-06-10. Source IDs: S030, S029.
- **2026-06-11 — uv 0.11.21 added CPython 3.13.14 and 3.14.6 support** [UV-2026-06-01121]: Astral's uv changelog notes 0.11.21 release with CPython 3.13.14 and 3.14.6 additions. Significance: Important for Python offline/wheelhouse/venv workflows. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Programming / Packaging. Related domain: Programming / Cyber / Platforms.
  - Retrieval aliases: UV-2026-06-01121; uv 0.11.21 added CPython 3.13.14 and 3.14.6 support; Programming / Packaging; 2026-06-11. Source IDs: S031, S032.
- **2026-06-13 — Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order** [AI-2026-06-ANTHROPIC-EXPORT]: Anthropic's June 2026 top-tier Claude models became a test case for AI export controls aimed at software capabilities, not just chips. Reuters reported Anthropic disabled them globally after a U.S. order limiting foreign access. Significance: Major AI-governance shift: model access itself became a national-security/export-control object. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for AI policy / Export controls. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2026-06-ANTHROPIC-EXPORT; Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order; AI policy / Export controls; 2026-06-13. Source IDs: S020, S021.
- **2026-06-14 — Trump's 80th birthday featured Putin call and controversial White House UFC event** [TRUMP-2026-06-BDAY]: Putin publicly congratulated Trump on his 80th birthday and held a 55-minute call. Trump also hosted a UFC event on the White House South Lawn; critics protested corruption, conflict-of-interest and authoritarian spectacle concerns, while No Kings-linked counter-events framed it as a democracy/free-speech issue. Significance: Concrete event query anchor: if asked “what happened at Trump's 2026 birthday,” answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for USA / Trump / Culture war. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: TRUMP-2026-06-BDAY; Trump's 80th birthday featured Putin call and controversial White House UFC event; USA / Trump / Culture war; 2026-06-14. Source IDs: S038, S039.
- **2026-06-17..2026-06-18 — G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power** [G7-2026-06-EVIAN]: G7 leaders met in Evian-les-Bains. Reuters described discussion of Trump's Iran deal, stronger Ukraine posture, critical-minerals supply chains, China dependency, and AI/data-center power questions involving industry figures. Significance: Connects geopolitics, AI infrastructure, energy, minerals and U.S. alliance management in one summit. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for G7 / Geopolitics / AI. Related domain: AI / Models / Agents.
  - Retrieval aliases: G7-2026-06-EVIAN; G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power; G7 / Geopolitics / AI; 2026-06-17..2026-06-18. Source IDs: S040.
- **2026-06-18 — U.S.-Iran interim agreement aimed at ceasefire and negotiations** [ME-2026-06-USIRANDEAL]: Reuters reported a U.S.-Iran interim agreement/deal after months of conflict, opening a 60-day negotiation period. Core issues such as nuclear capability, missile limits, proxies and regional acceptance remained uncertain. Significance: High-staleness but critical: affects oil/Hormuz risk, Israel/Gulf security, Lebanon/Hezbollah and U.S. domestic politics. Confidence/Staleness: medium/high.
  - Offline model note: Use this as a dated update for Middle East / USA / Iran. Related domain: USA / Trump / U.S. politics.
  - Retrieval aliases: ME-2026-06-USIRANDEAL; U.S.-Iran interim agreement aimed at ceasefire and negotiations; Middle East / USA / Iran; 2026-06-18. Source IDs: S041, S042, S043.
- **2026-06-18 — Ukrainian drone strikes hit Moscow refinery infrastructure** [UA-2026-06-MOSCOWREFINERY]: Reuters/Guardian live coverage reported Ukrainian drone attacks around Moscow including an oil refinery, highlighting Ukraine's ability to strike deep into Russia and pressure Moscow's air defenses. Significance: Concrete war-development anchor for June 2026; very high staleness because battlefield dynamics change rapidly. Confidence/Staleness: medium/high.
  - Offline model note: Use this as a dated update for Ukraine / Russia / War. Related domain: AI / Models / Agents.
  - Retrieval aliases: UA-2026-06-MOSCOWREFINERY; Ukrainian drone strikes hit Moscow refinery infrastructure; Ukraine / Russia / War; 2026-06-18. Source IDs: S044.
- **2026-06-18 — DRC/Uganda Bundibugyo Ebola outbreak worsened** [HEALTH-2026-06-EBOLA]: WHO confirmed a 2026 Ebola outbreak in DRC and Uganda involving Bundibugyo virus. Reuters reported DRC confirmed cases near 900 with hundreds of deaths; CDC/Africa CDC funding and response gaps became major issues. Significance: High-staleness public-health anchor: requires current verification before operational decisions. Confidence/Staleness: high/high.
  - Offline model note: Use this as a dated update for Health / Africa / Ebola. Related domain: Science / Health / Climate / Space / Games.
  - Retrieval aliases: HEALTH-2026-06-EBOLA; DRC/Uganda Bundibugyo Ebola outbreak worsened; Health / Africa / Ebola; 2026-06-18. Source IDs: S045, S046, S047, S048.
- **2026-06-18 — Node.js security releases updated 26.x, 24.x and 22.x lines** [NODE-2026-06-SECURITY]: Node.js shipped security releases for 26.x, 24.x and 22.x, updating dependencies including llhttp, nghttp2, OpenSSL and undici. Significance: Useful concrete admin/dev action: update Node runtimes in supported lines. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Security / Programming. Related domain: Programming / Cyber / Platforms.
  - Retrieval aliases: NODE-2026-06-SECURITY; Node.js security releases updated 26.x, 24.x and 22.x lines; Security / Programming; 2026-06-18. Source IDs: S033, S034.
### Year 2024

- **2024 — 2024 election supercycle continued** [WORLD-2024-ELECTION-SUPERCYCLE]: Elections in countries representing nearly half of humanity made 2024 a global political reset year, including India, EU, UK, France and U.S. Significance: Useful background: many post-cutoff political assumptions changed in a short period. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for World politics. Related domain: World / Cross-domain.
  - Retrieval aliases: WORLD-2024-ELECTION-SUPERCYCLE; 2024 election supercycle continued; World politics; 2024. Source IDs: S004.
### Year 2025

- **2025-01 — Gaza ceasefire/hostage diplomacy remained fragile** [ME-2025-GAZA-CEASEFIRE]: Early 2025 saw renewed Gaza ceasefire/hostage-release diplomacy, but stability remained fragile and later regional conflicts kept evolving. Significance: Do not assume Gaza/Israel war state from June 2024 remained unchanged. Confidence/Staleness: medium/high.
  - Offline model note: Use this as a dated update for Middle East / Gaza. Related domain: Middle East / Iran / Israel / Syria.
  - Retrieval aliases: ME-2025-GAZA-CEASEFIRE; Gaza ceasefire/hostage diplomacy remained fragile; Middle East / Gaza; 2025-01. Source IDs: S003, S054.
- **2025 — Trump tariff policy reshaped global trade risk** [TRADE-2025-TARIFFS]: The second Trump administration pushed aggressive tariff/trade policies, raising inflation, supply-chain and ally-tension questions. Significance: Important for economics and geopolitics; live verification needed for exact tariff rates. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Economy / Trade. Related domain: World / Cross-domain.
  - Retrieval aliases: TRADE-2025-TARIFFS; Trump tariff policy reshaped global trade risk; Economy / Trade; 2025. Source IDs: S003.
- **2025-08-02 — EU AI Act GPAI/governance obligations entered staged application** [AI-2025-AI-ACT-GPAI]: General-purpose AI obligations and governance/enforcement provisions entered their next staged application period, affecting model providers serving the EU. Significance: Important for frontier AI model providers and open/closed model transparency debates. Confidence/Staleness: high/medium.
  - Offline model note: Use this as a dated update for AI regulation / EU. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2025-AI-ACT-GPAI; EU AI Act GPAI/governance obligations entered staged application; AI regulation / EU; 2025-08-02. Source IDs: S005, S006.
- **2025-06 — Digital news trust/platform shifts continued** [MEDIA-2025-DIGITALNEWS]: Reuters Institute's 2025 Digital News Report framed journalism against uncertainty, platform fragmentation, AI and climate/conflict pressures. Significance: Useful for understanding media ecosystem and information trust. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Media / AI / Society. Related domain: AI / Models / Agents.
  - Retrieval aliases: MEDIA-2025-DIGITALNEWS; Digital news trust/platform shifts continued; Media / AI / Society; 2025-06. Source IDs: S054.
- **2025 — Nintendo Switch successor era began** [GAMES-2025-SWITCH2]: The games industry moved into a new hardware/platform cycle around Nintendo's Switch successor and publisher showcase resets. Significance: Useful as gaming-market context, but exact launch details should be verified in current sources. Confidence/Staleness: medium/medium.
  - Offline model note: Use this as a dated update for Games / Hardware. Related domain: War / Ukraine / Russia.
  - Retrieval aliases: GAMES-2025-SWITCH2; Nintendo Switch successor era began; Games / Hardware; 2025. Source IDs: S054.
- **2025 — AI-in-science moved from novelty to infrastructure** [SCI-2025-AI-SCIENCE]: After AlphaFold/Nobel recognition, 2025 research and industry increasingly treated AI as an accelerator for biology, chemistry, coding and data analysis. Significance: Good reasoning context, not a single event. Confidence/Staleness: medium/low.
  - Offline model note: Use this as a dated update for Science / AI. Related domain: AI / Models / Agents.
  - Retrieval aliases: SCI-2025-AI-SCIENCE; AI-in-science moved from novelty to infrastructure; Science / AI; 2025. Source IDs: S003, S019.
### Year 2026

- **2026-06-12 — OpenAI retired GPT-5.2 ChatGPT variants; GPT-5.5 remained** [AI-2026-OPENAI-RETIREMENTS]: OpenAI release notes say GPT-5.2 Instant/Thinking/Pro were no longer available in ChatGPT as of 12 Jun 2026 and conversations moved to GPT-5.5 counterparts. Significance: Important model lifecycle detail for users comparing ChatGPT behavior. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for AI / OpenAI lifecycle. Related domain: AI / Models / Agents.
  - Retrieval aliases: AI-2026-OPENAI-RETIREMENTS; OpenAI retired GPT-5.2 ChatGPT variants; GPT-5.5 remained; AI / OpenAI lifecycle; 2026-06-12. Source IDs: S012.
- **2026-06-15 — U.S. closed Delta probe from 2024 CrowdStrike meltdown** [CROWDSTRIKE-2026-DELTA-PROBE]: USDOT closed its investigation into Delta's 2024 CrowdStrike-triggered operational meltdown, noting passenger support and no penalties. Significance: Shows long-tail regulatory/business effects of the 2024 outage. Confidence/Staleness: high/low.
  - Offline model note: Use this as a dated update for Cyber / Aviation / Regulation. Related domain: Programming / Cyber / Platforms.
  - Retrieval aliases: CROWDSTRIKE-2026-DELTA-PROBE; U.S. closed Delta probe from 2024 CrowdStrike meltdown; Cyber / Aviation / Regulation; 2026-06-15. Source IDs: S053.



## Expanded Retrieval Dossier Round 1

This round adds model-facing retrieval, chronology and answer-boundary notes. It is intentionally context content, not source-link filler.

### DOSSIER WORLD-2024-06-INDIA - India election: Modi won third term but without BJP outright majority

**Anchor date/period:** 2024-06-04  
**Domain:** World / Cross-domain  
**Category:** World politics / India  
**Confidence/Staleness:** high / medium

#### What happened
Narendra Modi remained prime minister after India's 2024 election, but the BJP lost its single-party majority and became more dependent on coalition partners.

#### Why this changed the offline baseline
For a June-2024-cutoff model this is an important correction: Modi continued, but the political mandate weakened compared with earlier expectations. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: WORLD-2024-06-INDIA
- Main title: India election: Modi won third term but without BJP outright majority
- Category path: World politics / India
- Date key: 2024-06-04
- Related domain: World / Cross-domain
- Related cards in same domain: WORLD-2024-ELECTION-SUPERCYCLE, TRADE-2025-TARIFFS

#### Source context, not links
- S004: Reuters: 2024 global elections graphic — 2024 had elections in countries home to almost half the world population; used as election-supercycle context.
- S002: CFR: Ten Most Significant World Events in 2024 — High-level synthesis of 2024 world events, including Trump win, conflicts, elections, climate and AI/security context.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Narendra Modi remained prime minister after India's 2024 election, but the BJP lost its single-party majority and became more dependent on coalition partners. This mattered because For a June-2024-cutoff model this is an important correction: Modi continued, but the political mandate weakened compared with earlier expectations.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Narendra Modi remained prime minister after India's 2024 election, but the BJP lost its single-party majority and became more dependent on coalition partners. Wichtig daran ist: For a June-2024-cutoff model this is an important correction: Modi continued, but the political mandate weakened compared with earlier expectations.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for World / Cross-domain and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-06-04 in World politics / India?
2. Why does India election: Modi won third term but without BJP outright majority matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Narendra Modi remained prime minister after India's 2024 election, but the BJP lost its single-party majority and became more dependent on coalition partners. The important point is that For a June-2024-cutoff model this is an important correction: Modi continued, but the political mandate weakened compared with earlier expectations. Confidence is high; staleness is medium."

### DOSSIER EU-2024-06-ELECTION - European Parliament election shifted balance rightward

**Anchor date/period:** 2024-06-06..2024-06-09  
**Domain:** Europe / EU / Germany / UK  
**Category:** EU / Politics  
**Confidence/Staleness:** high / low

#### What happened
The June 2024 European Parliament elections increased the weight of right-wing and nationalist parties, while mainstream pro-EU groups still retained enough influence to shape the Parliament.

#### Why this changed the offline baseline
Important for EU regulation, migration politics, climate policy and digital/AI policy after 2024. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: EU-2024-06-ELECTION
- Main title: European Parliament election shifted balance rightward
- Category path: EU / Politics
- Date key: 2024-06-06..2024-06-09
- Related domain: Europe / EU / Germany / UK
- Related cards in same domain: FR-2024-06-SNAP, UK-2024-07-ELECTION, DE-2025-02-ELECTION

#### Source context, not links
- S004: Reuters: 2024 global elections graphic — 2024 had elections in countries home to almost half the world population; used as election-supercycle context.
- S002: CFR: Ten Most Significant World Events in 2024 — High-level synthesis of 2024 world events, including Trump win, conflicts, elections, climate and AI/security context.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, The June 2024 European Parliament elections increased the weight of right-wing and nationalist parties, while mainstream pro-EU groups still retained enough influence to shape the Parliament. This mattered because Important for EU regulation, migration politics, climate policy and digital/AI policy after 2024.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: The June 2024 European Parliament elections increased the weight of right-wing and nationalist parties, while mainstream pro-EU groups still retained enough influence to shape the Parliament. Wichtig daran ist: Important for EU regulation, migration politics, climate policy and digital/AI policy after 2024.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Europe / EU / Germany / UK and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-06-06..2024-06-09 in EU / Politics?
2. Why does European Parliament election shifted balance rightward matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, The June 2024 European Parliament elections increased the weight of right-wing and nationalist parties, while mainstream pro-EU groups still retained enough influence to shape the Parliament. The important point is that Important for EU regulation, migration politics, climate policy and digital/AI policy after 2024. Confidence is high; staleness is low."

### DOSSIER FR-2024-06-SNAP - Macron called snap legislative elections after EU vote setback

**Anchor date/period:** 2024-06-09  
**Domain:** Europe / EU / Germany / UK  
**Category:** France / EU  
**Confidence/Staleness:** high / low

#### What happened
After France's EU election result, Emmanuel Macron dissolved the National Assembly and called snap elections, creating political uncertainty in France.

#### Why this changed the offline baseline
This changed European political risk and showed how EU election results directly affected national politics. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: FR-2024-06-SNAP
- Main title: Macron called snap legislative elections after EU vote setback
- Category path: France / EU
- Date key: 2024-06-09
- Related domain: Europe / EU / Germany / UK
- Related cards in same domain: EU-2024-06-ELECTION, UK-2024-07-ELECTION, DE-2025-02-ELECTION

#### Source context, not links
- S002: CFR: Ten Most Significant World Events in 2024 — High-level synthesis of 2024 world events, including Trump win, conflicts, elections, climate and AI/security context.
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, After France's EU election result, Emmanuel Macron dissolved the National Assembly and called snap elections, creating political uncertainty in France. This mattered because This changed European political risk and showed how EU election results directly affected national politics.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: After France's EU election result, Emmanuel Macron dissolved the National Assembly and called snap elections, creating political uncertainty in France. Wichtig daran ist: This changed European political risk and showed how EU election results directly affected national politics.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Europe / EU / Germany / UK and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-06-09 in France / EU?
2. Why does Macron called snap legislative elections after EU vote setback matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, After France's EU election result, Emmanuel Macron dissolved the National Assembly and called snap elections, creating political uncertainty in France. The important point is that This changed European political risk and showed how EU election results directly affected national politics. Confidence is high; staleness is low."

### DOSSIER AI-2024-06-CLAUDE35 - Anthropic released Claude 3.5 Sonnet

**Anchor date/period:** 2024-06-20  
**Domain:** AI / Models / Agents  
**Category:** AI / Models  
**Confidence/Staleness:** high / low

#### What happened
Anthropic released Claude 3.5 Sonnet as a faster, cheaper, stronger model than prior Claude 3 models, with improved coding and Artifacts workflow support.

#### Why this changed the offline baseline
A post-cutoff local model should know Claude 3.5 became a major coding/writing competitor after June 2024. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2024-06-CLAUDE35
- Main title: Anthropic released Claude 3.5 Sonnet
- Category path: AI / Models
- Date key: 2024-06-20
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK, EU-2025-02-AI-ACT-PROHIBITIONS

#### Source context, not links
- S019: Anthropic system cards — Anthropic system-card timeline for Claude 3.5/3.7/4/4.1/4.5 families.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Anthropic released Claude 3.5 Sonnet as a faster, cheaper, stronger model than prior Claude 3 models, with improved coding and Artifacts workflow support. This mattered because A post-cutoff local model should know Claude 3.5 became a major coding/writing competitor after June 2024.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Anthropic released Claude 3.5 Sonnet as a faster, cheaper, stronger model than prior Claude 3 models, with improved coding and Artifacts workflow support. Wichtig daran ist: A post-cutoff local model should know Claude 3.5 became a major coding/writing competitor after June 2024.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-06-20 in AI / Models?
2. Why does Anthropic released Claude 3.5 Sonnet matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Anthropic released Claude 3.5 Sonnet as a faster, cheaper, stronger model than prior Claude 3 models, with improved coding and Artifacts workflow support. The important point is that A post-cutoff local model should know Claude 3.5 became a major coding/writing competitor after June 2024. Confidence is high; staleness is low."

### DOSSIER US-2024-06-DEBATE - Biden-Trump debate intensified concerns about Biden candidacy

**Anchor date/period:** 2024-06-27  
**Domain:** USA / Trump / U.S. politics  
**Category:** USA / Election  
**Confidence/Staleness:** high / low

#### What happened
The late-June 2024 debate became a turning point in the U.S. election cycle by intensifying public and party concerns about Joe Biden's campaign viability.

#### Why this changed the offline baseline
Sets up Biden's later withdrawal and Kamala Harris becoming Democratic nominee. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: US-2024-06-DEBATE
- Main title: Biden-Trump debate intensified concerns about Biden candidacy
- Category path: USA / Election
- Date key: 2024-06-27
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-07-TRUMP-ASSASSINATION, US-2024-07-BIDEN-WITHDRAWAL, US-2024-11-TRUMP-WINS, US-2025-01-NEWORLEANS, CLIMATE-2025-01-LAFIRES, US-2025-01-TRUMP-INAG, US-2025-06-NOKINGS, US-2025-10-NOKINGS2, US-2025-11-SHUTDOWN, US-2026-03-NOKINGS3

#### Source context, not links
- S002: CFR: Ten Most Significant World Events in 2024 — High-level synthesis of 2024 world events, including Trump win, conflicts, elections, climate and AI/security context.
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, The late-June 2024 debate became a turning point in the U.S. election cycle by intensifying public and party concerns about Joe Biden's campaign viability. This mattered because Sets up Biden's later withdrawal and Kamala Harris becoming Democratic nominee.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: The late-June 2024 debate became a turning point in the U.S. election cycle by intensifying public and party concerns about Joe Biden's campaign viability. Wichtig daran ist: Sets up Biden's later withdrawal and Kamala Harris becoming Democratic nominee.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-06-27 in USA / Election?
2. Why does Biden-Trump debate intensified concerns about Biden candidacy matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, The late-June 2024 debate became a turning point in the U.S. election cycle by intensifying public and party concerns about Joe Biden's campaign viability. The important point is that Sets up Biden's later withdrawal and Kamala Harris becoming Democratic nominee. Confidence is high; staleness is low."

### DOSSIER UK-2024-07-ELECTION - UK Labour won a landslide; Keir Starmer became prime minister

**Anchor date/period:** 2024-07-04  
**Domain:** Europe / EU / Germany / UK  
**Category:** UK / Politics  
**Confidence/Staleness:** high / low

#### What happened
The UK general election ended 14 years of Conservative-led government. Labour under Keir Starmer won a large majority.

#### Why this changed the offline baseline
Important post-cutoff replacement for older UK political assumptions. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: UK-2024-07-ELECTION
- Main title: UK Labour won a landslide; Keir Starmer became prime minister
- Category path: UK / Politics
- Date key: 2024-07-04
- Related domain: Europe / EU / Germany / UK
- Related cards in same domain: EU-2024-06-ELECTION, FR-2024-06-SNAP, DE-2025-02-ELECTION

#### Source context, not links
- S002: CFR: Ten Most Significant World Events in 2024 — High-level synthesis of 2024 world events, including Trump win, conflicts, elections, climate and AI/security context.
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, The UK general election ended 14 years of Conservative-led government. Labour under Keir Starmer won a large majority. This mattered because Important post-cutoff replacement for older UK political assumptions.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: The UK general election ended 14 years of Conservative-led government. Labour under Keir Starmer won a large majority. Wichtig daran ist: Important post-cutoff replacement for older UK political assumptions.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Europe / EU / Germany / UK and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-07-04 in UK / Politics?
2. Why does UK Labour won a landslide; Keir Starmer became prime minister matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, The UK general election ended 14 years of Conservative-led government. Labour under Keir Starmer won a large majority. The important point is that Important post-cutoff replacement for older UK political assumptions. Confidence is high; staleness is low."

### DOSSIER US-2024-07-TRUMP-ASSASSINATION - Attempted assassination of Donald Trump at Butler rally

**Anchor date/period:** 2024-07-13  
**Domain:** USA / Trump / U.S. politics  
**Category:** USA / Election / Security  
**Confidence/Staleness:** high / low

#### What happened
Trump survived an assassination attempt during a campaign rally in Butler, Pennsylvania. The event reshaped campaign security and political rhetoric.

#### Why this changed the offline baseline
A major U.S. political shock that affected the campaign environment before the 2024 election. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: US-2024-07-TRUMP-ASSASSINATION
- Main title: Attempted assassination of Donald Trump at Butler rally
- Category path: USA / Election / Security
- Date key: 2024-07-13
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-06-DEBATE, US-2024-07-BIDEN-WITHDRAWAL, US-2024-11-TRUMP-WINS, US-2025-01-NEWORLEANS, CLIMATE-2025-01-LAFIRES, US-2025-01-TRUMP-INAG, US-2025-06-NOKINGS, US-2025-10-NOKINGS2, US-2025-11-SHUTDOWN, US-2026-03-NOKINGS3

#### Source context, not links
- S002: CFR: Ten Most Significant World Events in 2024 — High-level synthesis of 2024 world events, including Trump win, conflicts, elections, climate and AI/security context.
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Trump survived an assassination attempt during a campaign rally in Butler, Pennsylvania. The event reshaped campaign security and political rhetoric. This mattered because A major U.S. political shock that affected the campaign environment before the 2024 election.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Trump survived an assassination attempt during a campaign rally in Butler, Pennsylvania. The event reshaped campaign security and political rhetoric. Wichtig daran ist: A major U.S. political shock that affected the campaign environment before the 2024 election.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-07-13 in USA / Election / Security?
2. Why does Attempted assassination of Donald Trump at Butler rally matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Trump survived an assassination attempt during a campaign rally in Butler, Pennsylvania. The event reshaped campaign security and political rhetoric. The important point is that A major U.S. political shock that affected the campaign environment before the 2024 election. Confidence is high; staleness is low."

### DOSSIER CYBER-2024-07-CROWDSTRIKE - CrowdStrike faulty update caused global Windows outage

**Anchor date/period:** 2024-07-19  
**Domain:** Programming / Cyber / Platforms  
**Category:** Cybersecurity / Infrastructure  
**Confidence/Staleness:** high / low

#### What happened
A faulty CrowdStrike Falcon Sensor content update crashed roughly 8.5 million Windows devices worldwide, disrupting airlines, banks, healthcare, media and government services.

#### Why this changed the offline baseline
Demonstrated systemic software-supply-chain fragility: a security vendor update became critical infrastructure risk. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: CYBER-2024-07-CROWDSTRIKE
- Main title: CrowdStrike faulty update caused global Windows outage
- Category path: Cybersecurity / Infrastructure
- Date key: 2024-07-19
- Related domain: Programming / Cyber / Platforms
- Related cards in same domain: WINDOWS-2025-10-EOL, RUNTIME-2026-05-NODE26, PY-2026-06-3146, UV-2026-06-01121, NODE-2026-06-SECURITY, CROWDSTRIKE-2026-DELTA-PROBE

#### Source context, not links
- S007: Reuters: CrowdStrike global outage — Faulty CrowdStrike update caused global Windows outages affecting airlines, banks, healthcare and more.
- S008: Reuters: Microsoft estimates CrowdStrike device impact — Microsoft said about 8.5 million Windows devices were affected.
- S053: Reuters: US closes Delta CrowdStrike probe 2026 — USDOT closed probe into Delta 2024 CrowdStrike meltdown; impact review.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, A faulty CrowdStrike Falcon Sensor content update crashed roughly 8.5 million Windows devices worldwide, disrupting airlines, banks, healthcare, media and government services. This mattered because Demonstrated systemic software-supply-chain fragility: a security vendor update became critical infrastructure risk.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: A faulty CrowdStrike Falcon Sensor content update crashed roughly 8.5 million Windows devices worldwide, disrupting airlines, banks, healthcare, media and government services. Wichtig daran ist: Demonstrated systemic software-supply-chain fragility: a security vendor update became critical infrastructure risk.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Programming / Cyber / Platforms and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-07-19 in Cybersecurity / Infrastructure?
2. Why does CrowdStrike faulty update caused global Windows outage matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, A faulty CrowdStrike Falcon Sensor content update crashed roughly 8.5 million Windows devices worldwide, disrupting airlines, banks, healthcare, media and government services. The important point is that Demonstrated systemic software-supply-chain fragility: a security vendor update became critical infrastructure risk. Confidence is high; staleness is low."

### DOSSIER US-2024-07-BIDEN-WITHDRAWAL - Biden withdrew from 2024 race and endorsed Kamala Harris

**Anchor date/period:** 2024-07-21  
**Domain:** USA / Trump / U.S. politics  
**Category:** USA / Election  
**Confidence/Staleness:** high / low

#### What happened
Joe Biden ended his re-election campaign and endorsed Kamala Harris, changing the Democratic ticket months before the election.

#### Why this changed the offline baseline
Essential correction for any model whose pre-cutoff baseline expected Biden vs Trump rematch. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: US-2024-07-BIDEN-WITHDRAWAL
- Main title: Biden withdrew from 2024 race and endorsed Kamala Harris
- Category path: USA / Election
- Date key: 2024-07-21
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-06-DEBATE, US-2024-07-TRUMP-ASSASSINATION, US-2024-11-TRUMP-WINS, US-2025-01-NEWORLEANS, CLIMATE-2025-01-LAFIRES, US-2025-01-TRUMP-INAG, US-2025-06-NOKINGS, US-2025-10-NOKINGS2, US-2025-11-SHUTDOWN, US-2026-03-NOKINGS3

#### Source context, not links
- S002: CFR: Ten Most Significant World Events in 2024 — High-level synthesis of 2024 world events, including Trump win, conflicts, elections, climate and AI/security context.
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Joe Biden ended his re-election campaign and endorsed Kamala Harris, changing the Democratic ticket months before the election. This mattered because Essential correction for any model whose pre-cutoff baseline expected Biden vs Trump rematch.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Joe Biden ended his re-election campaign and endorsed Kamala Harris, changing the Democratic ticket months before the election. Wichtig daran ist: Essential correction for any model whose pre-cutoff baseline expected Biden vs Trump rematch.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-07-21 in USA / Election?
2. Why does Biden withdrew from 2024 race and endorsed Kamala Harris matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Joe Biden ended his re-election campaign and endorsed Kamala Harris, changing the Democratic ticket months before the election. The important point is that Essential correction for any model whose pre-cutoff baseline expected Biden vs Trump rematch. Confidence is high; staleness is low."

### DOSSIER AI-2024-07-LLAMA31 - Meta released Llama 3.1 including 405B

**Anchor date/period:** 2024-07-23  
**Domain:** AI / Models / Agents  
**Category:** AI / Open models  
**Confidence/Staleness:** high / low

#### What happened
Meta publicly released Llama 3.1 models, including a 405B frontier-scale open-weight model.

#### Why this changed the offline baseline
Important for local/offline AI: open-weight capability rose sharply after the target model's cutoff. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2024-07-LLAMA31
- Main title: Meta released Llama 3.1 including 405B
- Category path: AI / Open models
- Date key: 2024-07-23
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK, EU-2025-02-AI-ACT-PROHIBITIONS

#### Source context, not links
- S024: Meta: Llama 3.1 — Meta announced Llama 3.1 405B on 23 Jul 2024.
- S025: Meta Llama official model hub — Official Llama family hub for Llama, Llama Guard and Prompt Guard.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Meta publicly released Llama 3.1 models, including a 405B frontier-scale open-weight model. This mattered because Important for local/offline AI: open-weight capability rose sharply after the target model's cutoff.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Meta publicly released Llama 3.1 models, including a 405B frontier-scale open-weight model. Wichtig daran ist: Important for local/offline AI: open-weight capability rose sharply after the target model's cutoff.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-07-23 in AI / Open models?
2. Why does Meta released Llama 3.1 including 405B matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Meta publicly released Llama 3.1 models, including a 405B frontier-scale open-weight model. The important point is that Important for local/offline AI: open-weight capability rose sharply after the target model's cutoff. Confidence is high; staleness is low."

### DOSSIER SPORT-2024-07-PARIS - Paris 2024 Olympics opened

**Anchor date/period:** 2024-07-26  
**Domain:** Science / Health / Climate / Space / Games  
**Category:** Sports / Culture  
**Confidence/Staleness:** high / low

#### What happened
The Paris Summer Olympics began, with global cultural, security, political and infrastructure attention on France.

#### Why this changed the offline baseline
Major cultural anchor for summer 2024. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: SPORT-2024-07-PARIS
- Main title: Paris 2024 Olympics opened
- Category path: Sports / Culture
- Date key: 2024-07-26
- Related domain: Science / Health / Climate / Space / Games
- Related cards in same domain: SPACE-2024-10-STARSHIP-CATCH, CLIMATE-2024-11-COP29, CLIMATE-2025-COP30, SPACE-2026-05-STARSHIP12, GAMES-2026-06-SGF, HEALTH-2026-06-EBOLA

#### Source context, not links
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, The Paris Summer Olympics began, with global cultural, security, political and infrastructure attention on France. This mattered because Major cultural anchor for summer 2024.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: The Paris Summer Olympics began, with global cultural, security, political and infrastructure attention on France. Wichtig daran ist: Major cultural anchor for summer 2024.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Science / Health / Climate / Space / Games and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-07-26 in Sports / Culture?
2. Why does Paris 2024 Olympics opened matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, The Paris Summer Olympics began, with global cultural, security, political and infrastructure attention on France. The important point is that Major cultural anchor for summer 2024. Confidence is high; staleness is low."

### DOSSIER EU-2024-08-AI-ACT-FORCE - EU AI Act entered into force

**Anchor date/period:** 2024-08-01  
**Domain:** AI / Models / Agents  
**Category:** AI regulation / EU  
**Confidence/Staleness:** high / low

#### What happened
The EU AI Act entered into force, beginning staged implementation for prohibited practices, GPAI obligations, governance and full application.

#### Why this changed the offline baseline
Key post-cutoff regulatory change; offline models should treat EU AI regulation as active, not merely proposed. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: EU-2024-08-AI-ACT-FORCE
- Main title: EU AI Act entered into force
- Category path: AI regulation / EU
- Date key: 2024-08-01
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK, EU-2025-02-AI-ACT-PROHIBITIONS

#### Source context, not links
- S005: EU Commission: AI Act timeline — AI Act entered force 1 Aug 2024; full application 2 Aug 2026 with staged exceptions.
- S006: EU AI Act implementation timeline — Supplemental staged dates for prohibited practices, GPAI and governance obligations.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, The EU AI Act entered into force, beginning staged implementation for prohibited practices, GPAI obligations, governance and full application. This mattered because Key post-cutoff regulatory change; offline models should treat EU AI regulation as active, not merely proposed.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: The EU AI Act entered into force, beginning staged implementation for prohibited practices, GPAI obligations, governance and full application. Wichtig daran ist: Key post-cutoff regulatory change; offline models should treat EU AI regulation as active, not merely proposed.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-08-01 in AI regulation / EU?
2. Why does EU AI Act entered into force matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, The EU AI Act entered into force, beginning staged implementation for prohibited practices, GPAI obligations, governance and full application. The important point is that Key post-cutoff regulatory change; offline models should treat EU AI regulation as active, not merely proposed. Confidence is high; staleness is low."

### DOSSIER WAR-2024-08-KURSK - Ukraine launched cross-border operations into Russia's Kursk region

**Anchor date/period:** 2024-08  
**Domain:** AI / Models / Agents  
**Category:** Ukraine / Russia  
**Confidence/Staleness:** medium / medium

#### What happened
Ukraine conducted operations across the Russian border in the Kursk region, challenging assumptions that major ground operations stayed entirely inside Ukrainian territory.

#### Why this changed the offline baseline
Marked an escalation/shift in the geography and psychology of the Russia-Ukraine war. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: WAR-2024-08-KURSK
- Main title: Ukraine launched cross-border operations into Russia's Kursk region
- Category path: Ukraine / Russia
- Date key: 2024-08
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK, EU-2025-02-AI-ACT-PROHIBITIONS

#### Source context, not links
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.
- S002: CFR: Ten Most Significant World Events in 2024 — High-level synthesis of 2024 world events, including Trump win, conflicts, elections, climate and AI/security context.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Ukraine conducted operations across the Russian border in the Kursk region, challenging assumptions that major ground operations stayed entirely inside Ukrainian territory. This mattered because Marked an escalation/shift in the geography and psychology of the Russia-Ukraine war.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Ukraine conducted operations across the Russian border in the Kursk region, challenging assumptions that major ground operations stayed entirely inside Ukrainian territory. Wichtig daran ist: Marked an escalation/shift in the geography and psychology of the Russia-Ukraine war.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-08 in Ukraine / Russia?
2. Why does Ukraine launched cross-border operations into Russia's Kursk region matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Ukraine conducted operations across the Russian border in the Kursk region, challenging assumptions that major ground operations stayed entirely inside Ukrainian territory. The important point is that Marked an escalation/shift in the geography and psychology of the Russia-Ukraine war. Confidence is medium; staleness is medium."

### DOSSIER AI-2024-09-O1 - OpenAI introduced o1-style reasoning models

**Anchor date/period:** 2024-09  
**Domain:** AI / Models / Agents  
**Category:** AI / Reasoning models  
**Confidence/Staleness:** high / low

#### What happened
OpenAI introduced a family of models designed to spend more compute on reasoning before answering, making “reasoning effort” a visible product concept.

#### Why this changed the offline baseline
Important shift from pure chat-completion framing toward explicit deliberation/reasoning modes. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2024-09-O1
- Main title: OpenAI introduced o1-style reasoning models
- Category path: AI / Reasoning models
- Date key: 2024-09
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK, EU-2025-02-AI-ACT-PROHIBITIONS

#### Source context, not links
- S014: OpenAI model release notes — Official OpenAI model lifecycle notes including GPT-4o updates and o3 retirement timing.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, OpenAI introduced a family of models designed to spend more compute on reasoning before answering, making “reasoning effort” a visible product concept. This mattered because Important shift from pure chat-completion framing toward explicit deliberation/reasoning modes.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: OpenAI introduced a family of models designed to spend more compute on reasoning before answering, making “reasoning effort” a visible product concept. Wichtig daran ist: Important shift from pure chat-completion framing toward explicit deliberation/reasoning modes.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-09 in AI / Reasoning models?
2. Why does OpenAI introduced o1-style reasoning models matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, OpenAI introduced a family of models designed to spend more compute on reasoning before answering, making “reasoning effort” a visible product concept. The important point is that Important shift from pure chat-completion framing toward explicit deliberation/reasoning modes. Confidence is high; staleness is low."

### DOSSIER ME-2024-09-LEBANON - Israel-Hezbollah conflict escalated sharply in Lebanon

**Anchor date/period:** 2024-09  
**Domain:** Middle East / Iran / Israel / Syria  
**Category:** Middle East / Israel-Lebanon  
**Confidence/Staleness:** medium / medium

#### What happened
Israel and Hezbollah escalated from cross-border exchanges into a wider confrontation; Hezbollah leadership and infrastructure were severely hit.

#### Why this changed the offline baseline
This changed the regional balance around Israel, Iran, Lebanon and Gaza after the June 2024 cutoff. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: ME-2024-09-LEBANON
- Main title: Israel-Hezbollah conflict escalated sharply in Lebanon
- Category path: Middle East / Israel-Lebanon
- Date key: 2024-09
- Related domain: Middle East / Iran / Israel / Syria
- Related cards in same domain: SYRIA-2024-12-ASSAD-FALL, IRAN-2026-01-SHUTDOWN, ME-2025-GAZA-CEASEFIRE

#### Source context, not links
- S002: CFR: Ten Most Significant World Events in 2024 — High-level synthesis of 2024 world events, including Trump win, conflicts, elections, climate and AI/security context.
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Israel and Hezbollah escalated from cross-border exchanges into a wider confrontation; Hezbollah leadership and infrastructure were severely hit. This mattered because This changed the regional balance around Israel, Iran, Lebanon and Gaza after the June 2024 cutoff.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Israel and Hezbollah escalated from cross-border exchanges into a wider confrontation; Hezbollah leadership and infrastructure were severely hit. Wichtig daran ist: This changed the regional balance around Israel, Iran, Lebanon and Gaza after the June 2024 cutoff.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Middle East / Iran / Israel / Syria and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-09 in Middle East / Israel-Lebanon?
2. Why does Israel-Hezbollah conflict escalated sharply in Lebanon matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Israel and Hezbollah escalated from cross-border exchanges into a wider confrontation; Hezbollah leadership and infrastructure were severely hit. The important point is that This changed the regional balance around Israel, Iran, Lebanon and Gaza after the June 2024 cutoff. Confidence is medium; staleness is medium."

### DOSSIER NOBEL-2024-AI - AI work was recognized in 2024 Nobel prizes

**Anchor date/period:** 2024-10  
**Domain:** AI / Models / Agents  
**Category:** Science / AI  
**Confidence/Staleness:** high / low

#### What happened
The 2024 Nobel Prize in Physics honored John Hopfield and Geoffrey Hinton for foundational machine-learning work; the Chemistry prize recognized protein-design/protein-structure work including AlphaFold-related impact.

#### Why this changed the offline baseline
Symbolically important: AI became recognized as core scientific infrastructure, not just software product. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: NOBEL-2024-AI
- Main title: AI work was recognized in 2024 Nobel prizes
- Category path: Science / AI
- Date key: 2024-10
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK, EU-2025-02-AI-ACT-PROHIBITIONS

#### Source context, not links
- S011: UNFCCC COP29 outcome — COP29 agreed to triple climate finance to developing countries to USD 300B annually by 2035; broader USD 1.3T effort by 2035.
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, The 2024 Nobel Prize in Physics honored John Hopfield and Geoffrey Hinton for foundational machine-learning work; the Chemistry prize recognized protein-design/protein-structure work including AlphaFold-related impact. This mattered because Symbolically important: AI became recognized as core scientific infrastructure, not just software product.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: The 2024 Nobel Prize in Physics honored John Hopfield and Geoffrey Hinton for foundational machine-learning work; the Chemistry prize recognized protein-design/protein-structure work including AlphaFold-related impact. Wichtig daran ist: Symbolically important: AI became recognized as core scientific infrastructure, not just software product.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-10 in Science / AI?
2. Why does AI work was recognized in 2024 Nobel prizes matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, The 2024 Nobel Prize in Physics honored John Hopfield and Geoffrey Hinton for foundational machine-learning work; the Chemistry prize recognized protein-design/protein-structure work including AlphaFold-related impact. The important point is that Symbolically important: AI became recognized as core scientific infrastructure, not just software product. Confidence is high; staleness is low."

### DOSSIER SPACE-2024-10-STARSHIP-CATCH - Starship program demonstrated booster catch milestone

**Anchor date/period:** 2024-10  
**Domain:** Science / Health / Climate / Space / Games  
**Category:** Space / SpaceX  
**Confidence/Staleness:** medium / low

#### What happened
SpaceX's Starship test program achieved a major booster-recovery/catch milestone in 2024, strengthening confidence in reusable super-heavy launch ambitions.

#### Why this changed the offline baseline
Important for space access economics, Starlink, Artemis dependencies and long-term orbital infrastructure. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: SPACE-2024-10-STARSHIP-CATCH
- Main title: Starship program demonstrated booster catch milestone
- Category path: Space / SpaceX
- Date key: 2024-10
- Related domain: Science / Health / Climate / Space / Games
- Related cards in same domain: SPORT-2024-07-PARIS, CLIMATE-2024-11-COP29, CLIMATE-2025-COP30, SPACE-2026-05-STARSHIP12, GAMES-2026-06-SGF, HEALTH-2026-06-EBOLA

#### Source context, not links
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, SpaceX's Starship test program achieved a major booster-recovery/catch milestone in 2024, strengthening confidence in reusable super-heavy launch ambitions. This mattered because Important for space access economics, Starlink, Artemis dependencies and long-term orbital infrastructure.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: SpaceX's Starship test program achieved a major booster-recovery/catch milestone in 2024, strengthening confidence in reusable super-heavy launch ambitions. Wichtig daran ist: Important for space access economics, Starlink, Artemis dependencies and long-term orbital infrastructure.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Science / Health / Climate / Space / Games and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-10 in Space / SpaceX?
2. Why does Starship program demonstrated booster catch milestone matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, SpaceX's Starship test program achieved a major booster-recovery/catch milestone in 2024, strengthening confidence in reusable super-heavy launch ambitions. The important point is that Important for space access economics, Starlink, Artemis dependencies and long-term orbital infrastructure. Confidence is medium; staleness is low."

### DOSSIER US-2024-11-TRUMP-WINS - Donald Trump won the 2024 U.S. presidential election

**Anchor date/period:** 2024-11-05  
**Domain:** USA / Trump / U.S. politics  
**Category:** USA / Election  
**Confidence/Staleness:** high / low

#### What happened
Trump defeated Kamala Harris and prepared to return to the presidency in January 2025.

#### Why this changed the offline baseline
Primary political correction for models with June 2024 cutoff. It changes assumptions about U.S. federal policy, courts, tariffs, immigration, AI policy and Ukraine/Middle East diplomacy. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: US-2024-11-TRUMP-WINS
- Main title: Donald Trump won the 2024 U.S. presidential election
- Category path: USA / Election
- Date key: 2024-11-05
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-06-DEBATE, US-2024-07-TRUMP-ASSASSINATION, US-2024-07-BIDEN-WITHDRAWAL, US-2025-01-NEWORLEANS, CLIMATE-2025-01-LAFIRES, US-2025-01-TRUMP-INAG, US-2025-06-NOKINGS, US-2025-10-NOKINGS2, US-2025-11-SHUTDOWN, US-2026-03-NOKINGS3

#### Source context, not links
- S002: CFR: Ten Most Significant World Events in 2024 — High-level synthesis of 2024 world events, including Trump win, conflicts, elections, climate and AI/security context.
- S003: CFR: Ten Most Significant World Events in 2025 — High-level synthesis of 2025 world events including Trump return, AI race, trade/geopolitics.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Trump defeated Kamala Harris and prepared to return to the presidency in January 2025. This mattered because Primary political correction for models with June 2024 cutoff. It changes assumptions about U.S. federal policy, courts, tariffs, immigration, AI policy and Ukraine/Middle East diplomacy.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Trump defeated Kamala Harris and prepared to return to the presidency in January 2025. Wichtig daran ist: Primary political correction for models with June 2024 cutoff. It changes assumptions about U.S. federal policy, courts, tariffs, immigration, AI policy and Ukraine/Middle East diplomacy.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-11-05 in USA / Election?
2. Why does Donald Trump won the 2024 U.S. presidential election matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Trump defeated Kamala Harris and prepared to return to the presidency in January 2025. The important point is that Primary political correction for models with June 2024 cutoff. It changes assumptions about U.S. federal policy, courts, tariffs, immigration, AI policy and Ukraine/Middle East diplomacy. Confidence is high; staleness is low."

### DOSSIER CLIMATE-2024-11-COP29 - COP29 agreed new climate-finance goal

**Anchor date/period:** 2024-11-24  
**Domain:** Science / Health / Climate / Space / Games  
**Category:** Climate / COP29  
**Confidence/Staleness:** high / low

#### What happened
COP29 in Baku agreed to raise climate finance to developing countries to at least USD 300B annually by 2035, while debate continued over adequacy and fossil-fuel language.

#### Why this changed the offline baseline
Important for climate-diplomacy baseline and Global South finance disputes. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: CLIMATE-2024-11-COP29
- Main title: COP29 agreed new climate-finance goal
- Category path: Climate / COP29
- Date key: 2024-11-24
- Related domain: Science / Health / Climate / Space / Games
- Related cards in same domain: SPORT-2024-07-PARIS, SPACE-2024-10-STARSHIP-CATCH, CLIMATE-2025-COP30, SPACE-2026-05-STARSHIP12, GAMES-2026-06-SGF, HEALTH-2026-06-EBOLA

#### Source context, not links
- S011: UNFCCC COP29 outcome — COP29 agreed to triple climate finance to developing countries to USD 300B annually by 2035; broader USD 1.3T effort by 2035.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, COP29 in Baku agreed to raise climate finance to developing countries to at least USD 300B annually by 2035, while debate continued over adequacy and fossil-fuel language. This mattered because Important for climate-diplomacy baseline and Global South finance disputes.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: COP29 in Baku agreed to raise climate finance to developing countries to at least USD 300B annually by 2035, while debate continued over adequacy and fossil-fuel language. Wichtig daran ist: Important for climate-diplomacy baseline and Global South finance disputes.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Science / Health / Climate / Space / Games and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-11-24 in Climate / COP29?
2. Why does COP29 agreed new climate-finance goal matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, COP29 in Baku agreed to raise climate finance to developing countries to at least USD 300B annually by 2035, while debate continued over adequacy and fossil-fuel language. The important point is that Important for climate-diplomacy baseline and Global South finance disputes. Confidence is high; staleness is low."

### DOSSIER SYRIA-2024-12-ASSAD-FALL - Assad regime fell in Syria

**Anchor date/period:** 2024-12-08  
**Domain:** Middle East / Iran / Israel / Syria  
**Category:** Syria / Middle East  
**Confidence/Staleness:** high / medium

#### What happened
Syrian rebels seized Damascus; Bashar al-Assad fled, ending his family's decades of rule. The fall weakened Iran's regional position and raised uncertainty about transition, HTS influence, refugees and extremist resurgence.

#### Why this changed the offline baseline
Major post-cutoff geopolitical break: a long-running assumption that Assad remained in power became false. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: SYRIA-2024-12-ASSAD-FALL
- Main title: Assad regime fell in Syria
- Category path: Syria / Middle East
- Date key: 2024-12-08
- Related domain: Middle East / Iran / Israel / Syria
- Related cards in same domain: ME-2024-09-LEBANON, IRAN-2026-01-SHUTDOWN, ME-2025-GAZA-CEASEFIRE

#### Source context, not links
- S009: Reuters: Syria Assad rule ends — Syrian rebels seized Damascus and ended Bashar al-Assad rule on 8 Dec 2024.
- S010: Reuters: Assad exit implications — Assad exit shattered Iran influence but raised risks of instability/extremism.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Syrian rebels seized Damascus; Bashar al-Assad fled, ending his family's decades of rule. The fall weakened Iran's regional position and raised uncertainty about transition, HTS influence, refugees and extremist resurgence. This mattered because Major post-cutoff geopolitical break: a long-running assumption that Assad remained in power became false.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Syrian rebels seized Damascus; Bashar al-Assad fled, ending his family's decades of rule. The fall weakened Iran's regional position and raised uncertainty about transition, HTS influence, refugees and extremist resurgence. Wichtig daran ist: Major post-cutoff geopolitical break: a long-running assumption that Assad remained in power became false.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Middle East / Iran / Israel / Syria and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-12-08 in Syria / Middle East?
2. Why does Assad regime fell in Syria matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Syrian rebels seized Damascus; Bashar al-Assad fled, ending his family's decades of rule. The fall weakened Iran's regional position and raised uncertainty about transition, HTS influence, refugees and extremist resurgence. The important point is that Major post-cutoff geopolitical break: a long-running assumption that Assad remained in power became false. Confidence is high; staleness is medium."

### DOSSIER AI-2024-12-GEMINI20 - Google introduced Gemini 2.0 Flash experimental generation

**Anchor date/period:** 2024-12  
**Domain:** AI / Models / Agents  
**Category:** AI / Google  
**Confidence/Staleness:** high / low

#### What happened
Google moved Gemini into a 2.0 generation with Flash/agentic/multimodal emphasis, later leading toward 2.5/3.x lines.

#### Why this changed the offline baseline
Changes the Google-model baseline for offline models whose knowledge ends around Gemini 1.5. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2024-12-GEMINI20
- Main title: Google introduced Gemini 2.0 Flash experimental generation
- Category path: AI / Google
- Date key: 2024-12
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK, EU-2025-02-AI-ACT-PROHIBITIONS

#### Source context, not links
- S022: Google Gemini API changelog — Gemini API model/product release notes.
- S023: Google Cloud Gemini model lifecycle — Gemini model version/lifecycle dates including Gemini 2.5 and 3.x releases.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Google moved Gemini into a 2.0 generation with Flash/agentic/multimodal emphasis, later leading toward 2.5/3.x lines. This mattered because Changes the Google-model baseline for offline models whose knowledge ends around Gemini 1.5.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Google moved Gemini into a 2.0 generation with Flash/agentic/multimodal emphasis, later leading toward 2.5/3.x lines. Wichtig daran ist: Changes the Google-model baseline for offline models whose knowledge ends around Gemini 1.5.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-12 in AI / Google?
2. Why does Google introduced Gemini 2.0 Flash experimental generation matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Google moved Gemini into a 2.0 generation with Flash/agentic/multimodal emphasis, later leading toward 2.5/3.x lines. The important point is that Changes the Google-model baseline for offline models whose knowledge ends around Gemini 1.5. Confidence is high; staleness is low."

### DOSSIER AI-2024-12-O3 - OpenAI announced o3-generation reasoning direction

**Anchor date/period:** 2024-12  
**Domain:** AI / Models / Agents  
**Category:** AI / Reasoning models  
**Confidence/Staleness:** medium / low

#### What happened
OpenAI signaled a stronger reasoning-model direction after o1, foreshadowing 2025 reasoning/coding competition and later model lifecycle changes.

#### Why this changed the offline baseline
Shows frontier AI shifting to tool use, coding, long reasoning and benchmark-specialized modes. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2024-12-O3
- Main title: OpenAI announced o3-generation reasoning direction
- Category path: AI / Reasoning models
- Date key: 2024-12
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK, EU-2025-02-AI-ACT-PROHIBITIONS

#### Source context, not links
- S014: OpenAI model release notes — Official OpenAI model lifecycle notes including GPT-4o updates and o3 retirement timing.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, OpenAI signaled a stronger reasoning-model direction after o1, foreshadowing 2025 reasoning/coding competition and later model lifecycle changes. This mattered because Shows frontier AI shifting to tool use, coding, long reasoning and benchmark-specialized modes.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: OpenAI signaled a stronger reasoning-model direction after o1, foreshadowing 2025 reasoning/coding competition and later model lifecycle changes. Wichtig daran ist: Shows frontier AI shifting to tool use, coding, long reasoning and benchmark-specialized modes.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024-12 in AI / Reasoning models?
2. Why does OpenAI announced o3-generation reasoning direction matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, OpenAI signaled a stronger reasoning-model direction after o1, foreshadowing 2025 reasoning/coding competition and later model lifecycle changes. The important point is that Shows frontier AI shifting to tool use, coding, long reasoning and benchmark-specialized modes. Confidence is medium; staleness is low."

### DOSSIER US-2025-01-NEWORLEANS - New Orleans vehicle attack on New Year's Day

**Anchor date/period:** 2025-01-01  
**Domain:** USA / Trump / U.S. politics  
**Category:** USA / Security  
**Confidence/Staleness:** high / low

#### What happened
A vehicle attack on Bourbon Street killed and injured civilians, becoming a major U.S. domestic security incident at the start of 2025.

#### Why this changed the offline baseline
Anchor event for U.S. domestic security in 2025. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: US-2025-01-NEWORLEANS
- Main title: New Orleans vehicle attack on New Year's Day
- Category path: USA / Security
- Date key: 2025-01-01
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-06-DEBATE, US-2024-07-TRUMP-ASSASSINATION, US-2024-07-BIDEN-WITHDRAWAL, US-2024-11-TRUMP-WINS, CLIMATE-2025-01-LAFIRES, US-2025-01-TRUMP-INAG, US-2025-06-NOKINGS, US-2025-10-NOKINGS2, US-2025-11-SHUTDOWN, US-2026-03-NOKINGS3

#### Source context, not links
- S003: CFR: Ten Most Significant World Events in 2025 — High-level synthesis of 2025 world events including Trump return, AI race, trade/geopolitics.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, A vehicle attack on Bourbon Street killed and injured civilians, becoming a major U.S. domestic security incident at the start of 2025. This mattered because Anchor event for U.S. domestic security in 2025.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: A vehicle attack on Bourbon Street killed and injured civilians, becoming a major U.S. domestic security incident at the start of 2025. Wichtig daran ist: Anchor event for U.S. domestic security in 2025.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-01-01 in USA / Security?
2. Why does New Orleans vehicle attack on New Year's Day matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, A vehicle attack on Bourbon Street killed and injured civilians, becoming a major U.S. domestic security incident at the start of 2025. The important point is that Anchor event for U.S. domestic security in 2025. Confidence is high; staleness is low."

### DOSSIER CLIMATE-2025-01-LAFIRES - Major Los Angeles-area fires caused severe damage

**Anchor date/period:** 2025-01  
**Domain:** USA / Trump / U.S. politics  
**Category:** Climate / USA  
**Confidence/Staleness:** high / low

#### What happened
Palisades and Eaton fires became major California disasters, linking climate, insurance, urban planning, emergency response and infrastructure risk.

#### Why this changed the offline baseline
Important U.S. climate/disaster anchor for 2025. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: CLIMATE-2025-01-LAFIRES
- Main title: Major Los Angeles-area fires caused severe damage
- Category path: Climate / USA
- Date key: 2025-01
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-06-DEBATE, US-2024-07-TRUMP-ASSASSINATION, US-2024-07-BIDEN-WITHDRAWAL, US-2024-11-TRUMP-WINS, US-2025-01-NEWORLEANS, US-2025-01-TRUMP-INAG, US-2025-06-NOKINGS, US-2025-10-NOKINGS2, US-2025-11-SHUTDOWN, US-2026-03-NOKINGS3

#### Source context, not links
- S003: CFR: Ten Most Significant World Events in 2025 — High-level synthesis of 2025 world events including Trump return, AI race, trade/geopolitics.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Palisades and Eaton fires became major California disasters, linking climate, insurance, urban planning, emergency response and infrastructure risk. This mattered because Important U.S. climate/disaster anchor for 2025.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Palisades and Eaton fires became major California disasters, linking climate, insurance, urban planning, emergency response and infrastructure risk. Wichtig daran ist: Important U.S. climate/disaster anchor for 2025.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-01 in Climate / USA?
2. Why does Major Los Angeles-area fires caused severe damage matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Palisades and Eaton fires became major California disasters, linking climate, insurance, urban planning, emergency response and infrastructure risk. The important point is that Important U.S. climate/disaster anchor for 2025. Confidence is high; staleness is low."

### DOSSIER US-2025-01-TRUMP-INAG - Trump began second term

**Anchor date/period:** 2025-01-20  
**Domain:** USA / Trump / U.S. politics  
**Category:** USA / Politics  
**Confidence/Staleness:** high / low

#### What happened
Donald Trump was inaugurated for a second non-consecutive presidential term. His administration quickly emphasized tariffs, immigration enforcement, deregulation, energy, AI infrastructure and reversal of Biden-era policies.

#### Why this changed the offline baseline
Baseline political state for all post-Jan-2025 U.S. federal policy. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: US-2025-01-TRUMP-INAG
- Main title: Trump began second term
- Category path: USA / Politics
- Date key: 2025-01-20
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-06-DEBATE, US-2024-07-TRUMP-ASSASSINATION, US-2024-07-BIDEN-WITHDRAWAL, US-2024-11-TRUMP-WINS, US-2025-01-NEWORLEANS, CLIMATE-2025-01-LAFIRES, US-2025-06-NOKINGS, US-2025-10-NOKINGS2, US-2025-11-SHUTDOWN, US-2026-03-NOKINGS3

#### Source context, not links
- S003: CFR: Ten Most Significant World Events in 2025 — High-level synthesis of 2025 world events including Trump return, AI race, trade/geopolitics.
- S021: Reuters: Anthropic disables top-tier models — U.S. order/foreign-access restriction led Anthropic to disable Fable 5/Mythos 5 for all users, according to Reuters.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Donald Trump was inaugurated for a second non-consecutive presidential term. His administration quickly emphasized tariffs, immigration enforcement, deregulation, energy, AI infrastructure and reversal of Biden-era policies. This mattered because Baseline political state for all post-Jan-2025 U.S. federal policy.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Donald Trump was inaugurated for a second non-consecutive presidential term. His administration quickly emphasized tariffs, immigration enforcement, deregulation, energy, AI infrastructure and reversal of Biden-era policies. Wichtig daran ist: Baseline political state for all post-Jan-2025 U.S. federal policy.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-01-20 in USA / Politics?
2. Why does Trump began second term matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Donald Trump was inaugurated for a second non-consecutive presidential term. His administration quickly emphasized tariffs, immigration enforcement, deregulation, energy, AI infrastructure and reversal of Biden-era policies. The important point is that Baseline political state for all post-Jan-2025 U.S. federal policy. Confidence is high; staleness is low."

### DOSSIER AI-2025-01-STARGATE - Stargate AI infrastructure project announced

**Anchor date/period:** 2025-01-21  
**Domain:** AI / Models / Agents  
**Category:** AI infrastructure / USA  
**Confidence/Staleness:** high / medium

#### What happened
Trump announced the Stargate Project, described as a large AI infrastructure investment backed by OpenAI, Oracle, SoftBank and MGX.

#### Why this changed the offline baseline
AI competition became strongly tied to data centers, power, capital expenditure and national industrial strategy. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2025-01-STARGATE
- Main title: Stargate AI infrastructure project announced
- Category path: AI infrastructure / USA
- Date key: 2025-01-21
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-DEEPSEEK, EU-2025-02-AI-ACT-PROHIBITIONS

#### Source context, not links
- S017: Chatham House: Trump, Stargate, DeepSeek — Summary of early-2025 AI infrastructure/geopolitics shock around Stargate and DeepSeek.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Trump announced the Stargate Project, described as a large AI infrastructure investment backed by OpenAI, Oracle, SoftBank and MGX. This mattered because AI competition became strongly tied to data centers, power, capital expenditure and national industrial strategy.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Trump announced the Stargate Project, described as a large AI infrastructure investment backed by OpenAI, Oracle, SoftBank and MGX. Wichtig daran ist: AI competition became strongly tied to data centers, power, capital expenditure and national industrial strategy.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-01-21 in AI infrastructure / USA?
2. Why does Stargate AI infrastructure project announced matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Trump announced the Stargate Project, described as a large AI infrastructure investment backed by OpenAI, Oracle, SoftBank and MGX. The important point is that AI competition became strongly tied to data centers, power, capital expenditure and national industrial strategy. Confidence is high; staleness is medium."

### DOSSIER AI-2025-01-DEEPSEEK - DeepSeek shock challenged U.S. frontier-cost assumptions

**Anchor date/period:** 2025-01  
**Domain:** AI / Models / Agents  
**Category:** AI / China / Markets  
**Confidence/Staleness:** high / medium

#### What happened
DeepSeek's model release drew global attention for strong performance at lower apparent cost; Trump called it a wake-up call for U.S. industry, and regulators later scrutinized DeepSeek privacy/security.

#### Why this changed the offline baseline
Important correction: post-cutoff AI competition became more multipolar, with China/open models pressuring U.S. proprietary economics. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2025-01-DEEPSEEK
- Main title: DeepSeek shock challenged U.S. frontier-cost assumptions
- Category path: AI / China / Markets
- Date key: 2025-01
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, EU-2025-02-AI-ACT-PROHIBITIONS

#### Source context, not links
- S015: Reuters: DeepSeek wake-up call — Trump called DeepSeek a wake-up call for US industry; used for DeepSeek disruption context.
- S016: Reuters: DeepSeek regulatory scrutiny — Governments increased scrutiny of DeepSeek over privacy/security and data storage concerns.
- S017: Chatham House: Trump, Stargate, DeepSeek — Summary of early-2025 AI infrastructure/geopolitics shock around Stargate and DeepSeek.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, DeepSeek's model release drew global attention for strong performance at lower apparent cost; Trump called it a wake-up call for U.S. industry, and regulators later scrutinized DeepSeek privacy/security. This mattered because Important correction: post-cutoff AI competition became more multipolar, with China/open models pressuring U.S. proprietary economics.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: DeepSeek's model release drew global attention for strong performance at lower apparent cost; Trump called it a wake-up call for U.S. industry, and regulators later scrutinized DeepSeek privacy/security. Wichtig daran ist: Important correction: post-cutoff AI competition became more multipolar, with China/open models pressuring U.S. proprietary economics.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-01 in AI / China / Markets?
2. Why does DeepSeek shock challenged U.S. frontier-cost assumptions matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, DeepSeek's model release drew global attention for strong performance at lower apparent cost; Trump called it a wake-up call for U.S. industry, and regulators later scrutinized DeepSeek privacy/security. The important point is that Important correction: post-cutoff AI competition became more multipolar, with China/open models pressuring U.S. proprietary economics. Confidence is high; staleness is medium."

### DOSSIER EU-2025-02-AI-ACT-PROHIBITIONS - EU AI Act prohibited-practices and AI-literacy provisions began applying

**Anchor date/period:** 2025-02-02  
**Domain:** AI / Models / Agents  
**Category:** AI regulation / EU  
**Confidence/Staleness:** high / low

#### What happened
The first AI Act obligations, including bans on unacceptable-risk practices and AI-literacy requirements, began applying.

#### Why this changed the offline baseline
Important for compliance: by 2025 the AI Act was no longer only future legislation. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: EU-2025-02-AI-ACT-PROHIBITIONS
- Main title: EU AI Act prohibited-practices and AI-literacy provisions began applying
- Category path: AI regulation / EU
- Date key: 2025-02-02
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S005: EU Commission: AI Act timeline — AI Act entered force 1 Aug 2024; full application 2 Aug 2026 with staged exceptions.
- S006: EU AI Act implementation timeline — Supplemental staged dates for prohibited practices, GPAI and governance obligations.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, The first AI Act obligations, including bans on unacceptable-risk practices and AI-literacy requirements, began applying. This mattered because Important for compliance: by 2025 the AI Act was no longer only future legislation.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: The first AI Act obligations, including bans on unacceptable-risk practices and AI-literacy requirements, began applying. Wichtig daran ist: Important for compliance: by 2025 the AI Act was no longer only future legislation.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-02-02 in AI regulation / EU?
2. Why does EU AI Act prohibited-practices and AI-literacy provisions began applying matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, The first AI Act obligations, including bans on unacceptable-risk practices and AI-literacy requirements, began applying. The important point is that Important for compliance: by 2025 the AI Act was no longer only future legislation. Confidence is high; staleness is low."

### DOSSIER AI-2025-02-CLAUDE37 - Claude Sonnet 3.7 era emphasized hybrid reasoning/coding

**Anchor date/period:** 2025-02  
**Domain:** AI / Models / Agents  
**Category:** AI / Models  
**Confidence/Staleness:** medium / low

#### What happened
Anthropic's 2025 model cycle moved Claude toward stronger reasoning and coding workflows before Claude 4.

#### Why this changed the offline baseline
Shows rapid model cadence after Claude 3.5 and before Claude 4/4.5. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2025-02-CLAUDE37
- Main title: Claude Sonnet 3.7 era emphasized hybrid reasoning/coding
- Category path: AI / Models
- Date key: 2025-02
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S019: Anthropic system cards — Anthropic system-card timeline for Claude 3.5/3.7/4/4.1/4.5 families.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Anthropic's 2025 model cycle moved Claude toward stronger reasoning and coding workflows before Claude 4. This mattered because Shows rapid model cadence after Claude 3.5 and before Claude 4/4.5.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Anthropic's 2025 model cycle moved Claude toward stronger reasoning and coding workflows before Claude 4. Wichtig daran ist: Shows rapid model cadence after Claude 3.5 and before Claude 4/4.5.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-02 in AI / Models?
2. Why does Claude Sonnet 3.7 era emphasized hybrid reasoning/coding matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Anthropic's 2025 model cycle moved Claude toward stronger reasoning and coding workflows before Claude 4. The important point is that Shows rapid model cadence after Claude 3.5 and before Claude 4/4.5. Confidence is medium; staleness is low."

### DOSSIER DE-2025-02-ELECTION - German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second

**Anchor date/period:** 2025-02-23  
**Domain:** Europe / EU / Germany / UK  
**Category:** Germany / EU  
**Confidence/Staleness:** high / low

#### What happened
Germany's opposition conservatives won the snap election after Scholz's coalition collapse; AfD achieved its strongest result and came second.

#### Why this changed the offline baseline
Important for German/EU policy after 2024: economic policy, Ukraine, migration and defense debates changed. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: DE-2025-02-ELECTION
- Main title: German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second
- Category path: Germany / EU
- Date key: 2025-02-23
- Related domain: Europe / EU / Germany / UK
- Related cards in same domain: EU-2024-06-ELECTION, FR-2024-06-SNAP, UK-2024-07-ELECTION

#### Source context, not links
- S026: Reuters: Germany election 2025 — Germany conservatives won 2025 election; Friedrich Merz positioned for chancellor; AfD second.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Germany's opposition conservatives won the snap election after Scholz's coalition collapse; AfD achieved its strongest result and came second. This mattered because Important for German/EU policy after 2024: economic policy, Ukraine, migration and defense debates changed.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Germany's opposition conservatives won the snap election after Scholz's coalition collapse; AfD achieved its strongest result and came second. Wichtig daran ist: Important for German/EU policy after 2024: economic policy, Ukraine, migration and defense debates changed.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Europe / EU / Germany / UK and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-02-23 in Germany / EU?
2. Why does German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Germany's opposition conservatives won the snap election after Scholz's coalition collapse; AfD achieved its strongest result and came second. The important point is that Important for German/EU policy after 2024: economic policy, Ukraine, migration and defense debates changed. Confidence is high; staleness is low."

### DOSSIER AI-2025-04-LLAMA4 - Meta Llama 4 generation appeared

**Anchor date/period:** 2025-04  
**Domain:** AI / Models / Agents  
**Category:** AI / Open models  
**Confidence/Staleness:** medium / low

#### What happened
Meta's Llama family advanced beyond 3.x during 2025, pushing multimodal/open-weight competition.

#### Why this changed the offline baseline
For local/offline work, Llama-family progress is a key practical baseline. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2025-04-LLAMA4
- Main title: Meta Llama 4 generation appeared
- Category path: AI / Open models
- Date key: 2025-04
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S025: Meta Llama official model hub — Official Llama family hub for Llama, Llama Guard and Prompt Guard.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Meta's Llama family advanced beyond 3.x during 2025, pushing multimodal/open-weight competition. This mattered because For local/offline work, Llama-family progress is a key practical baseline.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Meta's Llama family advanced beyond 3.x during 2025, pushing multimodal/open-weight competition. Wichtig daran ist: For local/offline work, Llama-family progress is a key practical baseline.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-04 in AI / Open models?
2. Why does Meta Llama 4 generation appeared matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Meta's Llama family advanced beyond 3.x during 2025, pushing multimodal/open-weight competition. The important point is that For local/offline work, Llama-family progress is a key practical baseline. Confidence is medium; staleness is low."

### DOSSIER AI-2025-05-CLAUDE4 - Anthropic released Claude Opus 4 and Sonnet 4

**Anchor date/period:** 2025-05-22  
**Domain:** AI / Models / Agents  
**Category:** AI / Models  
**Confidence/Staleness:** high / low

#### What happened
Anthropic announced Claude 4 models, emphasizing coding, reasoning, agent workflows and long-running tasks.

#### Why this changed the offline baseline
Major frontier-model upgrade after Claude 3.5/3.7; important for code-agent capability baselines. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2025-05-CLAUDE4
- Main title: Anthropic released Claude Opus 4 and Sonnet 4
- Category path: AI / Models
- Date key: 2025-05-22
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S018: Anthropic: Claude 4 — Official Claude Opus 4 and Sonnet 4 announcement, May 2025.
- S019: Anthropic system cards — Anthropic system-card timeline for Claude 3.5/3.7/4/4.1/4.5 families.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Anthropic announced Claude 4 models, emphasizing coding, reasoning, agent workflows and long-running tasks. This mattered because Major frontier-model upgrade after Claude 3.5/3.7; important for code-agent capability baselines.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Anthropic announced Claude 4 models, emphasizing coding, reasoning, agent workflows and long-running tasks. Wichtig daran ist: Major frontier-model upgrade after Claude 3.5/3.7; important for code-agent capability baselines.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-05-22 in AI / Models?
2. Why does Anthropic released Claude Opus 4 and Sonnet 4 matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Anthropic announced Claude 4 models, emphasizing coding, reasoning, agent workflows and long-running tasks. The important point is that Major frontier-model upgrade after Claude 3.5/3.7; important for code-agent capability baselines. Confidence is high; staleness is low."

### DOSSIER US-2025-06-NOKINGS - No Kings protests and military parade on Trump's 79th birthday

**Anchor date/period:** 2025-06-14  
**Domain:** USA / Trump / U.S. politics  
**Category:** USA / Protest / Trump  
**Confidence/Staleness:** high / low

#### What happened
On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; “No Kings” protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites.

#### Why this changed the offline baseline
A concrete event many offline models may miss: Trump birthday 2025 was politically charged and tied to anti-authoritarian protest symbolism. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: US-2025-06-NOKINGS
- Main title: No Kings protests and military parade on Trump's 79th birthday
- Category path: USA / Protest / Trump
- Date key: 2025-06-14
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-06-DEBATE, US-2024-07-TRUMP-ASSASSINATION, US-2024-07-BIDEN-WITHDRAWAL, US-2024-11-TRUMP-WINS, US-2025-01-NEWORLEANS, CLIMATE-2025-01-LAFIRES, US-2025-01-TRUMP-INAG, US-2025-10-NOKINGS2, US-2025-11-SHUTDOWN, US-2026-03-NOKINGS3

#### Source context, not links
- S035: Reuters: 2025 Trump military parade/No Kings — 2025 U.S. Army 250th parade fell on Trump birthday; nationwide No Kings protests occurred.
- S036: Reuters: Trump warns protest at parade — Trump warned protesters ahead of 2025 military parade.
- S037: Reuters: No Kings March 2026 — First No Kings event on Trump birthday 2025 drew estimated 4m-6m people; later mobilizations continued.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; “No Kings” protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites. This mattered because A concrete event many offline models may miss: Trump birthday 2025 was politically charged and tied to anti-authoritarian protest symbolism.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; “No Kings” protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites. Wichtig daran ist: A concrete event many offline models may miss: Trump birthday 2025 was politically charged and tied to anti-authoritarian protest symbolism.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-06-14 in USA / Protest / Trump?
2. Why does No Kings protests and military parade on Trump's 79th birthday matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; “No Kings” protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites. The important point is that A concrete event many offline models may miss: Trump birthday 2025 was politically charged and tied to anti-authoritarian protest symbolism. Confidence is high; staleness is low."

### DOSSIER AI-2025-06-GEMINI25 - Gemini 2.5 Pro/Flash reached stable enterprise lifecycle

**Anchor date/period:** 2025-06-17  
**Domain:** AI / Models / Agents  
**Category:** AI / Google  
**Confidence/Staleness:** high / low

#### What happened
Google's Gemini 2.5 Pro and Flash release/lifecycle dates became part of the stable Google AI model stack.

#### Why this changed the offline baseline
Updates Google model baseline for coding, multimodal and low-latency AI. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2025-06-GEMINI25
- Main title: Gemini 2.5 Pro/Flash reached stable enterprise lifecycle
- Category path: AI / Google
- Date key: 2025-06-17
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S023: Google Cloud Gemini model lifecycle — Gemini model version/lifecycle dates including Gemini 2.5 and 3.x releases.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Google's Gemini 2.5 Pro and Flash release/lifecycle dates became part of the stable Google AI model stack. This mattered because Updates Google model baseline for coding, multimodal and low-latency AI.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Google's Gemini 2.5 Pro and Flash release/lifecycle dates became part of the stable Google AI model stack. Wichtig daran ist: Updates Google model baseline for coding, multimodal and low-latency AI.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-06-17 in AI / Google?
2. Why does Gemini 2.5 Pro/Flash reached stable enterprise lifecycle matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Google's Gemini 2.5 Pro and Flash release/lifecycle dates became part of the stable Google AI model stack. The important point is that Updates Google model baseline for coding, multimodal and low-latency AI. Confidence is high; staleness is low."

### DOSSIER AI-2025-07-US-AI-PLAN - Trump White House AI policy favored exports and lighter state rules

**Anchor date/period:** 2025-07-22  
**Domain:** AI / Models / Agents  
**Category:** AI policy / USA  
**Confidence/Staleness:** high / medium

#### What happened
The White House prepared/published a plan to push U.S. AI abroad and restrict federal support for states with rules viewed as too restrictive.

#### Why this changed the offline baseline
U.S. AI governance shifted from Biden-era safety/executive-order posture toward innovation, infrastructure and export competition. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2025-07-US-AI-PLAN
- Main title: Trump White House AI policy favored exports and lighter state rules
- Category path: AI policy / USA
- Date key: 2025-07-22
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S021: Reuters: Anthropic disables top-tier models — U.S. order/foreign-access restriction led Anthropic to disable Fable 5/Mythos 5 for all users, according to Reuters.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, The White House prepared/published a plan to push U.S. AI abroad and restrict federal support for states with rules viewed as too restrictive. This mattered because U.S. AI governance shifted from Biden-era safety/executive-order posture toward innovation, infrastructure and export competition.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: The White House prepared/published a plan to push U.S. AI abroad and restrict federal support for states with rules viewed as too restrictive. Wichtig daran ist: U.S. AI governance shifted from Biden-era safety/executive-order posture toward innovation, infrastructure and export competition.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-07-22 in AI policy / USA?
2. Why does Trump White House AI policy favored exports and lighter state rules matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, The White House prepared/published a plan to push U.S. AI abroad and restrict federal support for states with rules viewed as too restrictive. The important point is that U.S. AI governance shifted from Biden-era safety/executive-order posture toward innovation, infrastructure and export competition. Confidence is high; staleness is medium."

### DOSSIER AI-2025-08-GPT5 - OpenAI released GPT-5

**Anchor date/period:** 2025-08-07  
**Domain:** AI / Models / Agents  
**Category:** AI / OpenAI  
**Confidence/Staleness:** high / low

#### What happened
OpenAI introduced GPT-5 as a unified system that routes between quick responses and deeper reasoning for coding, math, writing, health and multimodal work.

#### Why this changed the offline baseline
Major post-cutoff OpenAI milestone. Offline models should not assume GPT-4o/o1 are newest OpenAI systems. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2025-08-GPT5
- Main title: OpenAI released GPT-5
- Category path: AI / OpenAI
- Date key: 2025-08-07
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S013: OpenAI: Introducing GPT-5 — Official announcement for GPT-5 in Aug 2025.
- S014: OpenAI model release notes — Official OpenAI model lifecycle notes including GPT-4o updates and o3 retirement timing.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, OpenAI introduced GPT-5 as a unified system that routes between quick responses and deeper reasoning for coding, math, writing, health and multimodal work. This mattered because Major post-cutoff OpenAI milestone. Offline models should not assume GPT-4o/o1 are newest OpenAI systems.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: OpenAI introduced GPT-5 as a unified system that routes between quick responses and deeper reasoning for coding, math, writing, health and multimodal work. Wichtig daran ist: Major post-cutoff OpenAI milestone. Offline models should not assume GPT-4o/o1 are newest OpenAI systems.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-08-07 in AI / OpenAI?
2. Why does OpenAI released GPT-5 matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, OpenAI introduced GPT-5 as a unified system that routes between quick responses and deeper reasoning for coding, math, writing, health and multimodal work. The important point is that Major post-cutoff OpenAI milestone. Offline models should not assume GPT-4o/o1 are newest OpenAI systems. Confidence is high; staleness is low."

### DOSSIER AI-2025-08-GPTOSS - OpenAI released gpt-oss open-weight models

**Anchor date/period:** 2025-08  
**Domain:** AI / Models / Agents  
**Category:** AI / Open-weight / Offline  
**Confidence/Staleness:** high / low

#### What happened
OpenAI released gpt-oss-20b and 120b open-weight models. gpt-oss-20b is documented with Jun 01 2024 knowledge cutoff and 131,072-token context.

#### Why this changed the offline baseline
This is the target-model context: the offline model itself needs external post-cutoff context. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2025-08-GPTOSS
- Main title: OpenAI released gpt-oss open-weight models
- Category path: AI / Open-weight / Offline
- Date key: 2025-08
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S001: OpenAI gpt-oss-20b model docs — gpt-oss-20b has knowledge cutoff Jun 01 2024 and 131,072 context window.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, OpenAI released gpt-oss-20b and 120b open-weight models. gpt-oss-20b is documented with Jun 01 2024 knowledge cutoff and 131,072-token context. This mattered because This is the target-model context: the offline model itself needs external post-cutoff context.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: OpenAI released gpt-oss-20b and 120b open-weight models. gpt-oss-20b is documented with Jun 01 2024 knowledge cutoff and 131,072-token context. Wichtig daran ist: This is the target-model context: the offline model itself needs external post-cutoff context.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-08 in AI / Open-weight / Offline?
2. Why does OpenAI released gpt-oss open-weight models matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, OpenAI released gpt-oss-20b and 120b open-weight models. gpt-oss-20b is documented with Jun 01 2024 knowledge cutoff and 131,072-token context. The important point is that This is the target-model context: the offline model itself needs external post-cutoff context. Confidence is high; staleness is low."

### DOSSIER RUSSIA-2025-08-ALASKA - Trump-Putin Alaska meeting attempted Ukraine diplomacy

**Anchor date/period:** 2025-08  
**Domain:** AI / Models / Agents  
**Category:** USA / Russia / Ukraine  
**Confidence/Staleness:** medium / medium

#### What happened
Trump and Putin met in Alaska in August 2025 to attempt negotiations around the Russia-Ukraine war, but the conflict continued into 2026.

#### Why this changed the offline baseline
Anchor for later Putin-Trump personal diplomacy and Trump's 2026 birthday call. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: RUSSIA-2025-08-ALASKA
- Main title: Trump-Putin Alaska meeting attempted Ukraine diplomacy
- Category path: USA / Russia / Ukraine
- Date key: 2025-08
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S038: Reuters: Putin birthday greeting to Trump 2026 — Putin congratulated Trump on his 80th birthday and the two spoke for 55 minutes.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Trump and Putin met in Alaska in August 2025 to attempt negotiations around the Russia-Ukraine war, but the conflict continued into 2026. This mattered because Anchor for later Putin-Trump personal diplomacy and Trump's 2026 birthday call.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Trump and Putin met in Alaska in August 2025 to attempt negotiations around the Russia-Ukraine war, but the conflict continued into 2026. Wichtig daran ist: Anchor for later Putin-Trump personal diplomacy and Trump's 2026 birthday call.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-08 in USA / Russia / Ukraine?
2. Why does Trump-Putin Alaska meeting attempted Ukraine diplomacy matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Trump and Putin met in Alaska in August 2025 to attempt negotiations around the Russia-Ukraine war, but the conflict continued into 2026. The important point is that Anchor for later Putin-Trump personal diplomacy and Trump's 2026 birthday call. Confidence is medium; staleness is medium."

### DOSSIER AI-2025-09-CLAUDE45 - Claude Sonnet 4.5 emphasized agents, coding and computer use

**Anchor date/period:** 2025-09  
**Domain:** AI / Models / Agents  
**Category:** AI / Agents / Coding  
**Confidence/Staleness:** high / low

#### What happened
Anthropic's later 2025 Claude line positioned Sonnet 4.5 as strong for agents, coding and computer-use workflows.

#### Why this changed the offline baseline
Useful baseline for offline coding-agent discussions. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2025-09-CLAUDE45
- Main title: Claude Sonnet 4.5 emphasized agents, coding and computer use
- Category path: AI / Agents / Coding
- Date key: 2025-09
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S019: Anthropic system cards — Anthropic system-card timeline for Claude 3.5/3.7/4/4.1/4.5 families.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Anthropic's later 2025 Claude line positioned Sonnet 4.5 as strong for agents, coding and computer-use workflows. This mattered because Useful baseline for offline coding-agent discussions.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Anthropic's later 2025 Claude line positioned Sonnet 4.5 as strong for agents, coding and computer-use workflows. Wichtig daran ist: Useful baseline for offline coding-agent discussions.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-09 in AI / Agents / Coding?
2. Why does Claude Sonnet 4.5 emphasized agents, coding and computer use matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Anthropic's later 2025 Claude line positioned Sonnet 4.5 as strong for agents, coding and computer-use workflows. The important point is that Useful baseline for offline coding-agent discussions. Confidence is high; staleness is low."

### DOSSIER WINDOWS-2025-10-EOL - Windows 10 reached end of support

**Anchor date/period:** 2025-10-14  
**Domain:** Programming / Cyber / Platforms  
**Category:** Operating systems / Security  
**Confidence/Staleness:** high / low

#### What happened
Microsoft ended support for Windows 10 on 14 Oct 2025. PCs still run, but no regular security/feature updates are provided without ESU or special LTSC channels.

#### Why this changed the offline baseline
Highly relevant to Windows 10 users/admins: security posture changed materially after the cutoff. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: WINDOWS-2025-10-EOL
- Main title: Windows 10 reached end of support
- Category path: Operating systems / Security
- Date key: 2025-10-14
- Related domain: Programming / Cyber / Platforms
- Related cards in same domain: CYBER-2024-07-CROWDSTRIKE, RUNTIME-2026-05-NODE26, PY-2026-06-3146, UV-2026-06-01121, NODE-2026-06-SECURITY, CROWDSTRIKE-2026-DELTA-PROBE

#### Source context, not links
- S027: Microsoft: Windows 10 support ended — Windows 10 support ended 14 Oct 2025; no more feature/security updates without ESU.
- S028: Microsoft Windows 10 ESU — Consumer Extended Security Updates for eligible Windows 10 22H2 devices.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Microsoft ended support for Windows 10 on 14 Oct 2025. PCs still run, but no regular security/feature updates are provided without ESU or special LTSC channels. This mattered because Highly relevant to Windows 10 users/admins: security posture changed materially after the cutoff.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Microsoft ended support for Windows 10 on 14 Oct 2025. PCs still run, but no regular security/feature updates are provided without ESU or special LTSC channels. Wichtig daran ist: Highly relevant to Windows 10 users/admins: security posture changed materially after the cutoff.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Programming / Cyber / Platforms and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-10-14 in Operating systems / Security?
2. Why does Windows 10 reached end of support matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Microsoft ended support for Windows 10 on 14 Oct 2025. PCs still run, but no regular security/feature updates are provided without ESU or special LTSC channels. The important point is that Highly relevant to Windows 10 users/admins: security posture changed materially after the cutoff. Confidence is high; staleness is low."

### DOSSIER US-2025-10-NOKINGS2 - Second No Kings mobilization expanded anti-Trump protest network

**Anchor date/period:** 2025-10-18  
**Domain:** USA / Trump / U.S. politics  
**Category:** USA / Protest  
**Confidence/Staleness:** medium / medium

#### What happened
A second No Kings protest wave took place in October 2025, reportedly involving more locations and large participation.

#### Why this changed the offline baseline
Shows No Kings was not a one-day June 2025 event but became an ongoing protest brand. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: US-2025-10-NOKINGS2
- Main title: Second No Kings mobilization expanded anti-Trump protest network
- Category path: USA / Protest
- Date key: 2025-10-18
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-06-DEBATE, US-2024-07-TRUMP-ASSASSINATION, US-2024-07-BIDEN-WITHDRAWAL, US-2024-11-TRUMP-WINS, US-2025-01-NEWORLEANS, CLIMATE-2025-01-LAFIRES, US-2025-01-TRUMP-INAG, US-2025-06-NOKINGS, US-2025-11-SHUTDOWN, US-2026-03-NOKINGS3

#### Source context, not links
- S037: Reuters: No Kings March 2026 — First No Kings event on Trump birthday 2025 drew estimated 4m-6m people; later mobilizations continued.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, A second No Kings protest wave took place in October 2025, reportedly involving more locations and large participation. This mattered because Shows No Kings was not a one-day June 2025 event but became an ongoing protest brand.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: A second No Kings protest wave took place in October 2025, reportedly involving more locations and large participation. Wichtig daran ist: Shows No Kings was not a one-day June 2025 event but became an ongoing protest brand.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-10-18 in USA / Protest?
2. Why does Second No Kings mobilization expanded anti-Trump protest network matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, A second No Kings protest wave took place in October 2025, reportedly involving more locations and large participation. The important point is that Shows No Kings was not a one-day June 2025 event but became an ongoing protest brand. Confidence is medium; staleness is medium."

### DOSSIER US-2025-11-SHUTDOWN - Longest U.S. government shutdown ended after 43 days

**Anchor date/period:** 2025-11-12  
**Domain:** USA / Trump / U.S. politics  
**Category:** USA / Government  
**Confidence/Staleness:** medium / low

#### What happened
A 43-day U.S. government shutdown ended in November 2025, with funding/back-pay and political fights over health care and agency funding.

#### Why this changed the offline baseline
Important U.S. institutional stress event during Trump's second term. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: US-2025-11-SHUTDOWN
- Main title: Longest U.S. government shutdown ended after 43 days
- Category path: USA / Government
- Date key: 2025-11-12
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-06-DEBATE, US-2024-07-TRUMP-ASSASSINATION, US-2024-07-BIDEN-WITHDRAWAL, US-2024-11-TRUMP-WINS, US-2025-01-NEWORLEANS, CLIMATE-2025-01-LAFIRES, US-2025-01-TRUMP-INAG, US-2025-06-NOKINGS, US-2025-10-NOKINGS2, US-2026-03-NOKINGS3

#### Source context, not links
- S003: CFR: Ten Most Significant World Events in 2025 — High-level synthesis of 2025 world events including Trump return, AI race, trade/geopolitics.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, A 43-day U.S. government shutdown ended in November 2025, with funding/back-pay and political fights over health care and agency funding. This mattered because Important U.S. institutional stress event during Trump's second term.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: A 43-day U.S. government shutdown ended in November 2025, with funding/back-pay and political fights over health care and agency funding. Wichtig daran ist: Important U.S. institutional stress event during Trump's second term.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-11-12 in USA / Government?
2. Why does Longest U.S. government shutdown ended after 43 days matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, A 43-day U.S. government shutdown ended in November 2025, with funding/back-pay and political fights over health care and agency funding. The important point is that Important U.S. institutional stress event during Trump's second term. Confidence is medium; staleness is low."

### DOSSIER AI-2025-11-GPT51 - GPT-5.1 reorganized OpenAI product variants

**Anchor date/period:** 2025-11  
**Domain:** AI / Models / Agents  
**Category:** AI / OpenAI  
**Confidence/Staleness:** medium / low

#### What happened
OpenAI's GPT-5 family evolved through 5.1-style instant/thinking variants and personalization/product-routing changes.

#### Why this changed the offline baseline
Shows modern AI products are systems and routers, not simply single static models. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2025-11-GPT51
- Main title: GPT-5.1 reorganized OpenAI product variants
- Category path: AI / OpenAI
- Date key: 2025-11
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S012: OpenAI ChatGPT/model release notes — Official OpenAI release/lifecycle notes for GPT-4o, GPT-5.x, GPT-5.5 availability/retirements.
- S014: OpenAI model release notes — Official OpenAI model lifecycle notes including GPT-4o updates and o3 retirement timing.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, OpenAI's GPT-5 family evolved through 5.1-style instant/thinking variants and personalization/product-routing changes. This mattered because Shows modern AI products are systems and routers, not simply single static models.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: OpenAI's GPT-5 family evolved through 5.1-style instant/thinking variants and personalization/product-routing changes. Wichtig daran ist: Shows modern AI products are systems and routers, not simply single static models.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-11 in AI / OpenAI?
2. Why does GPT-5.1 reorganized OpenAI product variants matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, OpenAI's GPT-5 family evolved through 5.1-style instant/thinking variants and personalization/product-routing changes. The important point is that Shows modern AI products are systems and routers, not simply single static models. Confidence is medium; staleness is low."

### DOSSIER CLIMATE-2025-COP30 - COP30 in Brazil continued climate-finance/fossil-fuel disputes

**Anchor date/period:** 2025-11  
**Domain:** Science / Health / Climate / Space / Games  
**Category:** Climate / COP30  
**Confidence/Staleness:** medium / medium

#### What happened
COP30 discussions were framed by record heat, climate finance shortfalls, energy-transition disputes and the implementation gap after COP29.

#### Why this changed the offline baseline
Maintains climate context between COP29 and 2026 climate bulletins. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: CLIMATE-2025-COP30
- Main title: COP30 in Brazil continued climate-finance/fossil-fuel disputes
- Category path: Climate / COP30
- Date key: 2025-11
- Related domain: Science / Health / Climate / Space / Games
- Related cards in same domain: SPORT-2024-07-PARIS, SPACE-2024-10-STARSHIP-CATCH, CLIMATE-2024-11-COP29, SPACE-2026-05-STARSHIP12, GAMES-2026-06-SGF, HEALTH-2026-06-EBOLA

#### Source context, not links
- S003: CFR: Ten Most Significant World Events in 2025 — High-level synthesis of 2025 world events including Trump return, AI race, trade/geopolitics.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, COP30 discussions were framed by record heat, climate finance shortfalls, energy-transition disputes and the implementation gap after COP29. This mattered because Maintains climate context between COP29 and 2026 climate bulletins.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: COP30 discussions were framed by record heat, climate finance shortfalls, energy-transition disputes and the implementation gap after COP29. Wichtig daran ist: Maintains climate context between COP29 and 2026 climate bulletins.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Science / Health / Climate / Space / Games and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-11 in Climate / COP30?
2. Why does COP30 in Brazil continued climate-finance/fossil-fuel disputes matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, COP30 discussions were framed by record heat, climate finance shortfalls, energy-transition disputes and the implementation gap after COP29. The important point is that Maintains climate context between COP29 and 2026 climate bulletins. Confidence is medium; staleness is medium."

### DOSSIER AI-2025-12-GEMINI-TTS - Gemini API expanded TTS/live/audio capabilities

**Anchor date/period:** 2025-12  
**Domain:** AI / Models / Agents  
**Category:** AI / Multimodal  
**Confidence/Staleness:** high / low

#### What happened
Google's Gemini API changelog showed continued expansion of TTS/live/multimodal capabilities in late 2025.

#### Why this changed the offline baseline
AI model competition increasingly included real-time audio, agents and multimodal interfaces. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2025-12-GEMINI-TTS
- Main title: Gemini API expanded TTS/live/audio capabilities
- Category path: AI / Multimodal
- Date key: 2025-12
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S022: Google Gemini API changelog — Gemini API model/product release notes.
- S023: Google Cloud Gemini model lifecycle — Gemini model version/lifecycle dates including Gemini 2.5 and 3.x releases.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Google's Gemini API changelog showed continued expansion of TTS/live/multimodal capabilities in late 2025. This mattered because AI model competition increasingly included real-time audio, agents and multimodal interfaces.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Google's Gemini API changelog showed continued expansion of TTS/live/multimodal capabilities in late 2025. Wichtig daran ist: AI model competition increasingly included real-time audio, agents and multimodal interfaces.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-12 in AI / Multimodal?
2. Why does Gemini API expanded TTS/live/audio capabilities matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Google's Gemini API changelog showed continued expansion of TTS/live/multimodal capabilities in late 2025. The important point is that AI model competition increasingly included real-time audio, agents and multimodal interfaces. Confidence is high; staleness is low."

### DOSSIER IRAN-2026-01-SHUTDOWN - Iran internet shutdowns became major censorship/infrastructure case

**Anchor date/period:** 2026-01  
**Domain:** Middle East / Iran / Israel / Syria  
**Category:** Iran / Internet / Conflict  
**Confidence/Staleness:** medium / medium

#### What happened
Research on Iran's 2026 internet shutdowns described nationwide disruptions and centralized null-routing/censorship mechanisms amid protests and conflict.

#### Why this changed the offline baseline
Important for internet freedom, measurement, BGP-monitoring limits and wartime communications. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: IRAN-2026-01-SHUTDOWN
- Main title: Iran internet shutdowns became major censorship/infrastructure case
- Category path: Iran / Internet / Conflict
- Date key: 2026-01
- Related domain: Middle East / Iran / Israel / Syria
- Related cards in same domain: ME-2024-09-LEBANON, SYRIA-2024-12-ASSAD-FALL, ME-2025-GAZA-CEASEFIRE

#### Source context, not links
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Research on Iran's 2026 internet shutdowns described nationwide disruptions and centralized null-routing/censorship mechanisms amid protests and conflict. This mattered because Important for internet freedom, measurement, BGP-monitoring limits and wartime communications.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Research on Iran's 2026 internet shutdowns described nationwide disruptions and centralized null-routing/censorship mechanisms amid protests and conflict. Wichtig daran ist: Important for internet freedom, measurement, BGP-monitoring limits and wartime communications.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Middle East / Iran / Israel / Syria and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-01 in Iran / Internet / Conflict?
2. Why does Iran internet shutdowns became major censorship/infrastructure case matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Research on Iran's 2026 internet shutdowns described nationwide disruptions and centralized null-routing/censorship mechanisms amid protests and conflict. The important point is that Important for internet freedom, measurement, BGP-monitoring limits and wartime communications. Confidence is medium; staleness is medium."

### DOSSIER US-2026-03-NOKINGS3 - Third No Kings protest wave occurred amid Iran-war politics

**Anchor date/period:** 2026-03-28  
**Domain:** USA / Trump / U.S. politics  
**Category:** USA / Protest / Iran war  
**Confidence/Staleness:** high / medium

#### What happened
No Kings protests continued in March 2026 with Iran-war, ICE/immigration, authoritarianism and democratic-backsliding themes.

#### Why this changed the offline baseline
Offline models should know No Kings became an ongoing protest series through 2026. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: US-2026-03-NOKINGS3
- Main title: Third No Kings protest wave occurred amid Iran-war politics
- Category path: USA / Protest / Iran war
- Date key: 2026-03-28
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-06-DEBATE, US-2024-07-TRUMP-ASSASSINATION, US-2024-07-BIDEN-WITHDRAWAL, US-2024-11-TRUMP-WINS, US-2025-01-NEWORLEANS, CLIMATE-2025-01-LAFIRES, US-2025-01-TRUMP-INAG, US-2025-06-NOKINGS, US-2025-10-NOKINGS2, US-2025-11-SHUTDOWN

#### Source context, not links
- S037: Reuters: No Kings March 2026 — First No Kings event on Trump birthday 2025 drew estimated 4m-6m people; later mobilizations continued.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, No Kings protests continued in March 2026 with Iran-war, ICE/immigration, authoritarianism and democratic-backsliding themes. This mattered because Offline models should know No Kings became an ongoing protest series through 2026.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: No Kings protests continued in March 2026 with Iran-war, ICE/immigration, authoritarianism and democratic-backsliding themes. Wichtig daran ist: Offline models should know No Kings became an ongoing protest series through 2026.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-03-28 in USA / Protest / Iran war?
2. Why does Third No Kings protest wave occurred amid Iran-war politics matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, No Kings protests continued in March 2026 with Iran-war, ICE/immigration, authoritarianism and democratic-backsliding themes. The important point is that Offline models should know No Kings became an ongoing protest series through 2026. Confidence is high; staleness is medium."

### DOSSIER ME-2026-03-US-IRAN-WAR - U.S.-Iran war/conflict escalated before June 2026 ceasefire talks

**Anchor date/period:** 2026-03..2026-06  
**Domain:** USA / Trump / U.S. politics  
**Category:** Middle East / USA / Iran  
**Confidence/Staleness:** medium / high

#### What happened
By mid-June 2026 Reuters described a three-month conflict involving U.S. airstrikes coordinated with Israel against Iran. Iran's missile/drone forces and navy/air defenses were damaged, but nuclear issues remained unresolved.

#### Why this changed the offline baseline
Very high-staleness anchor: regional energy security, Hormuz, Israel, Hezbollah, Gulf states and U.S. politics all became linked to the conflict. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: ME-2026-03-US-IRAN-WAR
- Main title: U.S.-Iran war/conflict escalated before June 2026 ceasefire talks
- Category path: Middle East / USA / Iran
- Date key: 2026-03..2026-06
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-06-DEBATE, US-2024-07-TRUMP-ASSASSINATION, US-2024-07-BIDEN-WITHDRAWAL, US-2024-11-TRUMP-WINS, US-2025-01-NEWORLEANS, CLIMATE-2025-01-LAFIRES, US-2025-01-TRUMP-INAG, US-2025-06-NOKINGS, US-2025-10-NOKINGS2, US-2025-11-SHUTDOWN

#### Source context, not links
- S041: Reuters: U.S.-Iran interim deal 2026 — U.S.-Iran interim agreement/ceasefire and 60-day negotiation period.
- S042: Reuters: Trump goals in Iran war — Reuters analysis: Iran war outcomes partial; missile/drone damage, navy/air defense degradation, nuclear unresolved.
- S043: AP: Iran nuclear watchdog inspection — AP report on Iran inviting watchdog inspection and enriched uranium handling under agreement.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, By mid-June 2026 Reuters described a three-month conflict involving U.S. airstrikes coordinated with Israel against Iran. Iran's missile/drone forces and navy/air defenses were damaged, but nuclear issues remained unresolved. This mattered because Very high-staleness anchor: regional energy security, Hormuz, Israel, Hezbollah, Gulf states and U.S. politics all became linked to the conflict.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: By mid-June 2026 Reuters described a three-month conflict involving U.S. airstrikes coordinated with Israel against Iran. Iran's missile/drone forces and navy/air defenses were damaged, but nuclear issues remained unresolved. Wichtig daran ist: Very high-staleness anchor: regional energy security, Hormuz, Israel, Hezbollah, Gulf states and U.S. politics all became linked to the conflict.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-03..2026-06 in Middle East / USA / Iran?
2. Why does U.S.-Iran war/conflict escalated before June 2026 ceasefire talks matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, By mid-June 2026 Reuters described a three-month conflict involving U.S. airstrikes coordinated with Israel against Iran. Iran's missile/drone forces and navy/air defenses were damaged, but nuclear issues remained unresolved. The important point is that Very high-staleness anchor: regional energy security, Hormuz, Israel, Hezbollah, Gulf states and U.S. politics all became linked to the conflict. Confidence is medium; staleness is high."

### DOSSIER AI-2026-04-GPT55 - OpenAI GPT-5.5 generation became current frontier product line

**Anchor date/period:** 2026-04  
**Domain:** AI / Models / Agents  
**Category:** AI / OpenAI  
**Confidence/Staleness:** medium / low

#### What happened
OpenAI moved the GPT-5 family to GPT-5.5-era products; GPT-5.2 was retired from ChatGPT by June 2026 while GPT-5.5 remained available.

#### Why this changed the offline baseline
Updates model landscape for offline AI comparing itself to online frontier systems. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2026-04-GPT55
- Main title: OpenAI GPT-5.5 generation became current frontier product line
- Category path: AI / OpenAI
- Date key: 2026-04
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S012: OpenAI ChatGPT/model release notes — Official OpenAI release/lifecycle notes for GPT-4o, GPT-5.x, GPT-5.5 availability/retirements.
- S014: OpenAI model release notes — Official OpenAI model lifecycle notes including GPT-4o updates and o3 retirement timing.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, OpenAI moved the GPT-5 family to GPT-5.5-era products; GPT-5.2 was retired from ChatGPT by June 2026 while GPT-5.5 remained available. This mattered because Updates model landscape for offline AI comparing itself to online frontier systems.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: OpenAI moved the GPT-5 family to GPT-5.5-era products; GPT-5.2 was retired from ChatGPT by June 2026 while GPT-5.5 remained available. Wichtig daran ist: Updates model landscape for offline AI comparing itself to online frontier systems.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-04 in AI / OpenAI?
2. Why does OpenAI GPT-5.5 generation became current frontier product line matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, OpenAI moved the GPT-5 family to GPT-5.5-era products; GPT-5.2 was retired from ChatGPT by June 2026 while GPT-5.5 remained available. The important point is that Updates model landscape for offline AI comparing itself to online frontier systems. Confidence is medium; staleness is low."

### DOSSIER RUNTIME-2026-05-NODE26 - Node.js 26 appeared as current/upcoming LTS line

**Anchor date/period:** 2026-05-05  
**Domain:** Programming / Cyber / Platforms  
**Category:** Programming / Runtime  
**Confidence/Staleness:** high / low

#### What happened
Node.js 26 was released in May 2026 and entered the ecosystem alongside Node 24 LTS and Node 22 maintenance/security lines.

#### Why this changed the offline baseline
Relevant for dev/admin decisions and package ecosystem compatibility. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: RUNTIME-2026-05-NODE26
- Main title: Node.js 26 appeared as current/upcoming LTS line
- Category path: Programming / Runtime
- Date key: 2026-05-05
- Related domain: Programming / Cyber / Platforms
- Related cards in same domain: CYBER-2024-07-CROWDSTRIKE, WINDOWS-2025-10-EOL, PY-2026-06-3146, UV-2026-06-01121, NODE-2026-06-SECURITY, CROWDSTRIKE-2026-DELTA-PROBE

#### Source context, not links
- S034: endoflife.date Node.js — Node 26 released May 2026; Node 24 LTS, Node 22 maintenance context.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Node.js 26 was released in May 2026 and entered the ecosystem alongside Node 24 LTS and Node 22 maintenance/security lines. This mattered because Relevant for dev/admin decisions and package ecosystem compatibility.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Node.js 26 was released in May 2026 and entered the ecosystem alongside Node 24 LTS and Node 22 maintenance/security lines. Wichtig daran ist: Relevant for dev/admin decisions and package ecosystem compatibility.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Programming / Cyber / Platforms and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-05-05 in Programming / Runtime?
2. Why does Node.js 26 appeared as current/upcoming LTS line matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Node.js 26 was released in May 2026 and entered the ecosystem alongside Node 24 LTS and Node 22 maintenance/security lines. The important point is that Relevant for dev/admin decisions and package ecosystem compatibility. Confidence is high; staleness is low."

### DOSSIER SPACE-2026-05-STARSHIP12 - Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation

**Anchor date/period:** 2026-05-22  
**Domain:** Science / Health / Climate / Space / Games  
**Category:** Space / SpaceX  
**Confidence/Staleness:** high / medium

#### What happened
SpaceX launched the 12th Starship test flight and first V3 iteration. The test achieved milestones including mock satellite deployment and controlled spacecraft splashdown, but the Super Heavy booster crashed into the Gulf of Mexico and triggered an FAA-led investigation.

#### Why this changed the offline baseline
Important for Starship schedule, reusable launch economics, Starlink, Moon/Mars ambitions and SpaceX financing/IPO narratives. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: SPACE-2026-05-STARSHIP12
- Main title: Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation
- Category path: Space / SpaceX
- Date key: 2026-05-22
- Related domain: Science / Health / Climate / Space / Games
- Related cards in same domain: SPORT-2024-07-PARIS, SPACE-2024-10-STARSHIP-CATCH, CLIMATE-2024-11-COP29, CLIMATE-2025-COP30, GAMES-2026-06-SGF, HEALTH-2026-06-EBOLA

#### Source context, not links
- S049: Reuters: Starship Flight 12/V3 — SpaceX Starship 12th test flight and V3 debut in May 2026.
- S050: Reuters: FAA Starship investigation — FAA ordered SpaceX to investigate booster mishap after Flight 12.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, SpaceX launched the 12th Starship test flight and first V3 iteration. The test achieved milestones including mock satellite deployment and controlled spacecraft splashdown, but the Super Heavy booster crashed into the Gulf of Mexico and triggered an FAA-led investigation. This mattered because Important for Starship schedule, reusable launch economics, Starlink, Moon/Mars ambitions and SpaceX financing/IPO narratives.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: SpaceX launched the 12th Starship test flight and first V3 iteration. The test achieved milestones including mock satellite deployment and controlled spacecraft splashdown, but the Super Heavy booster crashed into the Gulf of Mexico and triggered an FAA-led investigation. Wichtig daran ist: Important for Starship schedule, reusable launch economics, Starlink, Moon/Mars ambitions and SpaceX financing/IPO narratives.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Science / Health / Climate / Space / Games and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-05-22 in Space / SpaceX?
2. Why does Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, SpaceX launched the 12th Starship test flight and first V3 iteration. The test achieved milestones including mock satellite deployment and controlled spacecraft splashdown, but the Super Heavy booster crashed into the Gulf of Mexico and triggered an FAA-led investigation. The important point is that Important for Starship schedule, reusable launch economics, Starlink, Moon/Mars ambitions and SpaceX financing/IPO narratives. Confidence is high; staleness is medium."

### DOSSIER AI-2026-05-GEMINI3 - Gemini 3.x enterprise model line appeared

**Anchor date/period:** 2026-05  
**Domain:** AI / Models / Agents  
**Category:** AI / Google  
**Confidence/Staleness:** high / low

#### What happened
Google Cloud model lifecycle listed Gemini 3.5 Flash and Gemini 3.x image/lite variants released in May 2026.

#### Why this changed the offline baseline
Updates Google model landscape beyond Gemini 2.5. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2026-05-GEMINI3
- Main title: Gemini 3.x enterprise model line appeared
- Category path: AI / Google
- Date key: 2026-05
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S023: Google Cloud Gemini model lifecycle — Gemini model version/lifecycle dates including Gemini 2.5 and 3.x releases.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Google Cloud model lifecycle listed Gemini 3.5 Flash and Gemini 3.x image/lite variants released in May 2026. This mattered because Updates Google model landscape beyond Gemini 2.5.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Google Cloud model lifecycle listed Gemini 3.5 Flash and Gemini 3.x image/lite variants released in May 2026. Wichtig daran ist: Updates Google model landscape beyond Gemini 2.5.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-05 in AI / Google?
2. Why does Gemini 3.x enterprise model line appeared matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Google Cloud model lifecycle listed Gemini 3.5 Flash and Gemini 3.x image/lite variants released in May 2026. The important point is that Updates Google model landscape beyond Gemini 2.5. Confidence is high; staleness is low."

### DOSSIER GAMES-2026-06-SGF - Summer Game Fest 2026 ran in Los Angeles with major game announcements

**Anchor date/period:** 2026-06-05..2026-06-08  
**Domain:** Science / Health / Climate / Space / Games  
**Category:** Games / Industry  
**Confidence/Staleness:** medium / low

#### What happened
Summer Game Fest 2026 took place from June 5-8. Coverage highlighted upcoming console/PC titles and announcements including Resident Evil Veronica, Guild Wars 3 console presence, Lords of the Fallen II and other publisher showcases.

#### Why this changed the offline baseline
Important culture/games anchor for June 2026 and for offline models asked about gaming releases/trends. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: GAMES-2026-06-SGF
- Main title: Summer Game Fest 2026 ran in Los Angeles with major game announcements
- Category path: Games / Industry
- Date key: 2026-06-05..2026-06-08
- Related domain: Science / Health / Climate / Space / Games
- Related cards in same domain: SPORT-2024-07-PARIS, SPACE-2024-10-STARSHIP-CATCH, CLIMATE-2024-11-COP29, CLIMATE-2025-COP30, SPACE-2026-05-STARSHIP12, HEALTH-2026-06-EBOLA

#### Source context, not links
- S051: Summer Game Fest official — Summer Game Fest 2026 main show date/venue.
- S052: PlayStation Blog SGF 2026 — Sony/PlayStation summary of selected SGF 2026 announcements.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Summer Game Fest 2026 took place from June 5-8. Coverage highlighted upcoming console/PC titles and announcements including Resident Evil Veronica, Guild Wars 3 console presence, Lords of the Fallen II and other publisher showcases. This mattered because Important culture/games anchor for June 2026 and for offline models asked about gaming releases/trends.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Summer Game Fest 2026 took place from June 5-8. Coverage highlighted upcoming console/PC titles and announcements including Resident Evil Veronica, Guild Wars 3 console presence, Lords of the Fallen II and other publisher showcases. Wichtig daran ist: Important culture/games anchor for June 2026 and for offline models asked about gaming releases/trends.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Science / Health / Climate / Space / Games and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-06-05..2026-06-08 in Games / Industry?
2. Why does Summer Game Fest 2026 ran in Los Angeles with major game announcements matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Summer Game Fest 2026 took place from June 5-8. Coverage highlighted upcoming console/PC titles and announcements including Resident Evil Veronica, Guild Wars 3 console presence, Lords of the Fallen II and other publisher showcases. The important point is that Important culture/games anchor for June 2026 and for offline models asked about gaming releases/trends. Confidence is medium; staleness is low."

### DOSSIER PY-2026-06-3146 - Python 3.14.6 and 3.13.14 released

**Anchor date/period:** 2026-06-10  
**Domain:** Programming / Cyber / Platforms  
**Category:** Programming / Python  
**Confidence/Staleness:** high / low

#### What happened
Python 3.14.6, the sixth maintenance release of 3.14, shipped with around 179 bugfixes/build/doc changes since 3.14.5; Python 3.13.14 also shipped.

#### Why this changed the offline baseline
Relevant for Python project planning and installer/runtime baselines. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: PY-2026-06-3146
- Main title: Python 3.14.6 and 3.13.14 released
- Category path: Programming / Python
- Date key: 2026-06-10
- Related domain: Programming / Cyber / Platforms
- Related cards in same domain: CYBER-2024-07-CROWDSTRIKE, WINDOWS-2025-10-EOL, RUNTIME-2026-05-NODE26, UV-2026-06-01121, NODE-2026-06-SECURITY, CROWDSTRIKE-2026-DELTA-PROBE

#### Source context, not links
- S030: Python Insider: Python 3.14.6 — Python 3.14.6 and 3.13.14 released 10 Jun 2026; 3.14.6 has ~179 fixes.
- S029: Python PEP 745 — Python 3.14 release schedule.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Python 3.14.6, the sixth maintenance release of 3.14, shipped with around 179 bugfixes/build/doc changes since 3.14.5; Python 3.13.14 also shipped. This mattered because Relevant for Python project planning and installer/runtime baselines.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Python 3.14.6, the sixth maintenance release of 3.14, shipped with around 179 bugfixes/build/doc changes since 3.14.5; Python 3.13.14 also shipped. Wichtig daran ist: Relevant for Python project planning and installer/runtime baselines.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Programming / Cyber / Platforms and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-06-10 in Programming / Python?
2. Why does Python 3.14.6 and 3.13.14 released matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Python 3.14.6, the sixth maintenance release of 3.14, shipped with around 179 bugfixes/build/doc changes since 3.14.5; Python 3.13.14 also shipped. The important point is that Relevant for Python project planning and installer/runtime baselines. Confidence is high; staleness is low."

### DOSSIER UV-2026-06-01121 - uv 0.11.21 added CPython 3.13.14 and 3.14.6 support

**Anchor date/period:** 2026-06-11  
**Domain:** Programming / Cyber / Platforms  
**Category:** Programming / Packaging  
**Confidence/Staleness:** high / low

#### What happened
Astral's uv changelog notes 0.11.21 release with CPython 3.13.14 and 3.14.6 additions.

#### Why this changed the offline baseline
Important for Python offline/wheelhouse/venv workflows. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: UV-2026-06-01121
- Main title: uv 0.11.21 added CPython 3.13.14 and 3.14.6 support
- Category path: Programming / Packaging
- Date key: 2026-06-11
- Related domain: Programming / Cyber / Platforms
- Related cards in same domain: CYBER-2024-07-CROWDSTRIKE, WINDOWS-2025-10-EOL, RUNTIME-2026-05-NODE26, PY-2026-06-3146, NODE-2026-06-SECURITY, CROWDSTRIKE-2026-DELTA-PROBE

#### Source context, not links
- S031: uv changelog — uv 0.11.21 released 2026-06-11; added CPython 3.13.14 and 3.14.6.
- S032: uv PyPI/project docs — uv supports pip-compatible workflows, global cache, Windows/macOS/Linux.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Astral's uv changelog notes 0.11.21 release with CPython 3.13.14 and 3.14.6 additions. This mattered because Important for Python offline/wheelhouse/venv workflows.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Astral's uv changelog notes 0.11.21 release with CPython 3.13.14 and 3.14.6 additions. Wichtig daran ist: Important for Python offline/wheelhouse/venv workflows.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Programming / Cyber / Platforms and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-06-11 in Programming / Packaging?
2. Why does uv 0.11.21 added CPython 3.13.14 and 3.14.6 support matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Astral's uv changelog notes 0.11.21 release with CPython 3.13.14 and 3.14.6 additions. The important point is that Important for Python offline/wheelhouse/venv workflows. Confidence is high; staleness is low."

### DOSSIER AI-2026-06-ANTHROPIC-EXPORT - Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order

**Anchor date/period:** 2026-06-13  
**Domain:** AI / Models / Agents  
**Category:** AI policy / Export controls  
**Confidence/Staleness:** high / medium

#### What happened
Anthropic's June 2026 top-tier Claude models became a test case for AI export controls aimed at software capabilities, not just chips. Reuters reported Anthropic disabled them globally after a U.S. order limiting foreign access.

#### Why this changed the offline baseline
Major AI-governance shift: model access itself became a national-security/export-control object. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2026-06-ANTHROPIC-EXPORT
- Main title: Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order
- Category path: AI policy / Export controls
- Date key: 2026-06-13
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S020: Anthropic Claude models overview — Claude Fable 5 generally available June 9 2026; Mythos 5 limited availability.
- S021: Reuters: Anthropic disables top-tier models — U.S. order/foreign-access restriction led Anthropic to disable Fable 5/Mythos 5 for all users, according to Reuters.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Anthropic's June 2026 top-tier Claude models became a test case for AI export controls aimed at software capabilities, not just chips. Reuters reported Anthropic disabled them globally after a U.S. order limiting foreign access. This mattered because Major AI-governance shift: model access itself became a national-security/export-control object.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Anthropic's June 2026 top-tier Claude models became a test case for AI export controls aimed at software capabilities, not just chips. Reuters reported Anthropic disabled them globally after a U.S. order limiting foreign access. Wichtig daran ist: Major AI-governance shift: model access itself became a national-security/export-control object.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-06-13 in AI policy / Export controls?
2. Why does Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Anthropic's June 2026 top-tier Claude models became a test case for AI export controls aimed at software capabilities, not just chips. Reuters reported Anthropic disabled them globally after a U.S. order limiting foreign access. The important point is that Major AI-governance shift: model access itself became a national-security/export-control object. Confidence is high; staleness is medium."

### DOSSIER TRUMP-2026-06-BDAY - Trump's 80th birthday featured Putin call and controversial White House UFC event

**Anchor date/period:** 2026-06-14  
**Domain:** USA / Trump / U.S. politics  
**Category:** USA / Trump / Culture war  
**Confidence/Staleness:** high / medium

#### What happened
Putin publicly congratulated Trump on his 80th birthday and held a 55-minute call. Trump also hosted a UFC event on the White House South Lawn; critics protested corruption, conflict-of-interest and authoritarian spectacle concerns, while No Kings-linked counter-events framed it as a democracy/free-speech issue.

#### Why this changed the offline baseline
Concrete event query anchor: if asked “what happened at Trump's 2026 birthday,” answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: TRUMP-2026-06-BDAY
- Main title: Trump's 80th birthday featured Putin call and controversial White House UFC event
- Category path: USA / Trump / Culture war
- Date key: 2026-06-14
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-06-DEBATE, US-2024-07-TRUMP-ASSASSINATION, US-2024-07-BIDEN-WITHDRAWAL, US-2024-11-TRUMP-WINS, US-2025-01-NEWORLEANS, CLIMATE-2025-01-LAFIRES, US-2025-01-TRUMP-INAG, US-2025-06-NOKINGS, US-2025-10-NOKINGS2, US-2025-11-SHUTDOWN

#### Source context, not links
- S038: Reuters: Putin birthday greeting to Trump 2026 — Putin congratulated Trump on his 80th birthday and the two spoke for 55 minutes.
- S039: Guardian: Trump UFC birthday event 2026 — Trump hosted a UFC event on the White House South Lawn; protests criticized ethics/conflicts.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Putin publicly congratulated Trump on his 80th birthday and held a 55-minute call. Trump also hosted a UFC event on the White House South Lawn; critics protested corruption, conflict-of-interest and authoritarian spectacle concerns, while No Kings-linked counter-events framed it as a democracy/free-speech issue. This mattered because Concrete event query anchor: if asked “what happened at Trump's 2026 birthday,” answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Putin publicly congratulated Trump on his 80th birthday and held a 55-minute call. Trump also hosted a UFC event on the White House South Lawn; critics protested corruption, conflict-of-interest and authoritarian spectacle concerns, while No Kings-linked counter-events framed it as a democracy/free-speech issue. Wichtig daran ist: Concrete event query anchor: if asked “what happened at Trump's 2026 birthday,” answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-06-14 in USA / Trump / Culture war?
2. Why does Trump's 80th birthday featured Putin call and controversial White House UFC event matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Putin publicly congratulated Trump on his 80th birthday and held a 55-minute call. Trump also hosted a UFC event on the White House South Lawn; critics protested corruption, conflict-of-interest and authoritarian spectacle concerns, while No Kings-linked counter-events framed it as a democracy/free-speech issue. The important point is that Concrete event query anchor: if asked “what happened at Trump's 2026 birthday,” answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism. Confidence is high; staleness is medium."

### DOSSIER G7-2026-06-EVIAN - G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power

**Anchor date/period:** 2026-06-17..2026-06-18  
**Domain:** AI / Models / Agents  
**Category:** G7 / Geopolitics / AI  
**Confidence/Staleness:** high / medium

#### What happened
G7 leaders met in Evian-les-Bains. Reuters described discussion of Trump's Iran deal, stronger Ukraine posture, critical-minerals supply chains, China dependency, and AI/data-center power questions involving industry figures.

#### Why this changed the offline baseline
Connects geopolitics, AI infrastructure, energy, minerals and U.S. alliance management in one summit. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: G7-2026-06-EVIAN
- Main title: G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power
- Category path: G7 / Geopolitics / AI
- Date key: 2026-06-17..2026-06-18
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S040: Reuters: G7 2026 summit — G7 discussed Iran deal, Ukraine, critical minerals and AI/data-center power at Evian-les-Bains.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, G7 leaders met in Evian-les-Bains. Reuters described discussion of Trump's Iran deal, stronger Ukraine posture, critical-minerals supply chains, China dependency, and AI/data-center power questions involving industry figures. This mattered because Connects geopolitics, AI infrastructure, energy, minerals and U.S. alliance management in one summit.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: G7 leaders met in Evian-les-Bains. Reuters described discussion of Trump's Iran deal, stronger Ukraine posture, critical-minerals supply chains, China dependency, and AI/data-center power questions involving industry figures. Wichtig daran ist: Connects geopolitics, AI infrastructure, energy, minerals and U.S. alliance management in one summit.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-06-17..2026-06-18 in G7 / Geopolitics / AI?
2. Why does G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, G7 leaders met in Evian-les-Bains. Reuters described discussion of Trump's Iran deal, stronger Ukraine posture, critical-minerals supply chains, China dependency, and AI/data-center power questions involving industry figures. The important point is that Connects geopolitics, AI infrastructure, energy, minerals and U.S. alliance management in one summit. Confidence is high; staleness is medium."

### DOSSIER ME-2026-06-USIRANDEAL - U.S.-Iran interim agreement aimed at ceasefire and negotiations

**Anchor date/period:** 2026-06-18  
**Domain:** USA / Trump / U.S. politics  
**Category:** Middle East / USA / Iran  
**Confidence/Staleness:** medium / high

#### What happened
Reuters reported a U.S.-Iran interim agreement/deal after months of conflict, opening a 60-day negotiation period. Core issues such as nuclear capability, missile limits, proxies and regional acceptance remained uncertain.

#### Why this changed the offline baseline
High-staleness but critical: affects oil/Hormuz risk, Israel/Gulf security, Lebanon/Hezbollah and U.S. domestic politics. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: ME-2026-06-USIRANDEAL
- Main title: U.S.-Iran interim agreement aimed at ceasefire and negotiations
- Category path: Middle East / USA / Iran
- Date key: 2026-06-18
- Related domain: USA / Trump / U.S. politics
- Related cards in same domain: US-2024-06-DEBATE, US-2024-07-TRUMP-ASSASSINATION, US-2024-07-BIDEN-WITHDRAWAL, US-2024-11-TRUMP-WINS, US-2025-01-NEWORLEANS, CLIMATE-2025-01-LAFIRES, US-2025-01-TRUMP-INAG, US-2025-06-NOKINGS, US-2025-10-NOKINGS2, US-2025-11-SHUTDOWN

#### Source context, not links
- S041: Reuters: U.S.-Iran interim deal 2026 — U.S.-Iran interim agreement/ceasefire and 60-day negotiation period.
- S042: Reuters: Trump goals in Iran war — Reuters analysis: Iran war outcomes partial; missile/drone damage, navy/air defense degradation, nuclear unresolved.
- S043: AP: Iran nuclear watchdog inspection — AP report on Iran inviting watchdog inspection and enriched uranium handling under agreement.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Reuters reported a U.S.-Iran interim agreement/deal after months of conflict, opening a 60-day negotiation period. Core issues such as nuclear capability, missile limits, proxies and regional acceptance remained uncertain. This mattered because High-staleness but critical: affects oil/Hormuz risk, Israel/Gulf security, Lebanon/Hezbollah and U.S. domestic politics.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Reuters reported a U.S.-Iran interim agreement/deal after months of conflict, opening a 60-day negotiation period. Core issues such as nuclear capability, missile limits, proxies and regional acceptance remained uncertain. Wichtig daran ist: High-staleness but critical: affects oil/Hormuz risk, Israel/Gulf security, Lebanon/Hezbollah and U.S. domestic politics.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for USA / Trump / U.S. politics and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-06-18 in Middle East / USA / Iran?
2. Why does U.S.-Iran interim agreement aimed at ceasefire and negotiations matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Reuters reported a U.S.-Iran interim agreement/deal after months of conflict, opening a 60-day negotiation period. Core issues such as nuclear capability, missile limits, proxies and regional acceptance remained uncertain. The important point is that High-staleness but critical: affects oil/Hormuz risk, Israel/Gulf security, Lebanon/Hezbollah and U.S. domestic politics. Confidence is medium; staleness is high."

### DOSSIER UA-2026-06-MOSCOWREFINERY - Ukrainian drone strikes hit Moscow refinery infrastructure

**Anchor date/period:** 2026-06-18  
**Domain:** AI / Models / Agents  
**Category:** Ukraine / Russia / War  
**Confidence/Staleness:** medium / high

#### What happened
Reuters/Guardian live coverage reported Ukrainian drone attacks around Moscow including an oil refinery, highlighting Ukraine's ability to strike deep into Russia and pressure Moscow's air defenses.

#### Why this changed the offline baseline
Concrete war-development anchor for June 2026; very high staleness because battlefield dynamics change rapidly. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: UA-2026-06-MOSCOWREFINERY
- Main title: Ukrainian drone strikes hit Moscow refinery infrastructure
- Category path: Ukraine / Russia / War
- Date key: 2026-06-18
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S044: Reuters: Ukraine Moscow refinery attack — Ukrainian drone attack on Moscow refinery, June 2026.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Reuters/Guardian live coverage reported Ukrainian drone attacks around Moscow including an oil refinery, highlighting Ukraine's ability to strike deep into Russia and pressure Moscow's air defenses. This mattered because Concrete war-development anchor for June 2026; very high staleness because battlefield dynamics change rapidly.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Reuters/Guardian live coverage reported Ukrainian drone attacks around Moscow including an oil refinery, highlighting Ukraine's ability to strike deep into Russia and pressure Moscow's air defenses. Wichtig daran ist: Concrete war-development anchor for June 2026; very high staleness because battlefield dynamics change rapidly.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-06-18 in Ukraine / Russia / War?
2. Why does Ukrainian drone strikes hit Moscow refinery infrastructure matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Reuters/Guardian live coverage reported Ukrainian drone attacks around Moscow including an oil refinery, highlighting Ukraine's ability to strike deep into Russia and pressure Moscow's air defenses. The important point is that Concrete war-development anchor for June 2026; very high staleness because battlefield dynamics change rapidly. Confidence is medium; staleness is high."

### DOSSIER HEALTH-2026-06-EBOLA - DRC/Uganda Bundibugyo Ebola outbreak worsened

**Anchor date/period:** 2026-06-18  
**Domain:** Science / Health / Climate / Space / Games  
**Category:** Health / Africa / Ebola  
**Confidence/Staleness:** high / high

#### What happened
WHO confirmed a 2026 Ebola outbreak in DRC and Uganda involving Bundibugyo virus. Reuters reported DRC confirmed cases near 900 with hundreds of deaths; CDC/Africa CDC funding and response gaps became major issues.

#### Why this changed the offline baseline
High-staleness public-health anchor: requires current verification before operational decisions. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: HEALTH-2026-06-EBOLA
- Main title: DRC/Uganda Bundibugyo Ebola outbreak worsened
- Category path: Health / Africa / Ebola
- Date key: 2026-06-18
- Related domain: Science / Health / Climate / Space / Games
- Related cards in same domain: SPORT-2024-07-PARIS, SPACE-2024-10-STARSHIP-CATCH, CLIMATE-2024-11-COP29, CLIMATE-2025-COP30, SPACE-2026-05-STARSHIP12, GAMES-2026-06-SGF

#### Source context, not links
- S045: WHO: DRC/Uganda Ebola 2026 — Ebola Bundibugyo outbreak confirmed in DRC and Uganda in May 2026.
- S046: Reuters: DRC Ebola cases 18 Jun 2026 — DRC confirmed Ebola case/death update.
- S047: Reuters: CDC Ebola emergency funding — CDC activated emergency Ebola response funding.
- S048: ECDC Ebola DRC/Uganda 2026 — ECDC situation page for DRC/Uganda Ebola outbreak.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, WHO confirmed a 2026 Ebola outbreak in DRC and Uganda involving Bundibugyo virus. Reuters reported DRC confirmed cases near 900 with hundreds of deaths; CDC/Africa CDC funding and response gaps became major issues. This mattered because High-staleness public-health anchor: requires current verification before operational decisions.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: WHO confirmed a 2026 Ebola outbreak in DRC and Uganda involving Bundibugyo virus. Reuters reported DRC confirmed cases near 900 with hundreds of deaths; CDC/Africa CDC funding and response gaps became major issues. Wichtig daran ist: High-staleness public-health anchor: requires current verification before operational decisions.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Science / Health / Climate / Space / Games and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-06-18 in Health / Africa / Ebola?
2. Why does DRC/Uganda Bundibugyo Ebola outbreak worsened matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, WHO confirmed a 2026 Ebola outbreak in DRC and Uganda involving Bundibugyo virus. Reuters reported DRC confirmed cases near 900 with hundreds of deaths; CDC/Africa CDC funding and response gaps became major issues. The important point is that High-staleness public-health anchor: requires current verification before operational decisions. Confidence is high; staleness is high."

### DOSSIER NODE-2026-06-SECURITY - Node.js security releases updated 26.x, 24.x and 22.x lines

**Anchor date/period:** 2026-06-18  
**Domain:** Programming / Cyber / Platforms  
**Category:** Security / Programming  
**Confidence/Staleness:** high / low

#### What happened
Node.js shipped security releases for 26.x, 24.x and 22.x, updating dependencies including llhttp, nghttp2, OpenSSL and undici.

#### Why this changed the offline baseline
Useful concrete admin/dev action: update Node runtimes in supported lines. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: NODE-2026-06-SECURITY
- Main title: Node.js security releases updated 26.x, 24.x and 22.x lines
- Category path: Security / Programming
- Date key: 2026-06-18
- Related domain: Programming / Cyber / Platforms
- Related cards in same domain: CYBER-2024-07-CROWDSTRIKE, WINDOWS-2025-10-EOL, RUNTIME-2026-05-NODE26, PY-2026-06-3146, UV-2026-06-01121, CROWDSTRIKE-2026-DELTA-PROBE

#### Source context, not links
- S033: Node.js June 2026 security release — Security updates for Node 26.x, 24.x and 22.x released 18 Jun 2026.
- S034: endoflife.date Node.js — Node 26 released May 2026; Node 24 LTS, Node 22 maintenance context.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Node.js shipped security releases for 26.x, 24.x and 22.x, updating dependencies including llhttp, nghttp2, OpenSSL and undici. This mattered because Useful concrete admin/dev action: update Node runtimes in supported lines.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Node.js shipped security releases for 26.x, 24.x and 22.x, updating dependencies including llhttp, nghttp2, OpenSSL and undici. Wichtig daran ist: Useful concrete admin/dev action: update Node runtimes in supported lines.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Programming / Cyber / Platforms and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2026-06-18 in Security / Programming?
2. Why does Node.js security releases updated 26.x, 24.x and 22.x lines matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Node.js shipped security releases for 26.x, 24.x and 22.x, updating dependencies including llhttp, nghttp2, OpenSSL and undici. The important point is that Useful concrete admin/dev action: update Node runtimes in supported lines. Confidence is high; staleness is low."

### DOSSIER WORLD-2024-ELECTION-SUPERCYCLE - 2024 election supercycle continued

**Anchor date/period:** 2024  
**Domain:** World / Cross-domain  
**Category:** World politics  
**Confidence/Staleness:** high / medium

#### What happened
Elections in countries representing nearly half of humanity made 2024 a global political reset year, including India, EU, UK, France and U.S.

#### Why this changed the offline baseline
Useful background: many post-cutoff political assumptions changed in a short period. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: WORLD-2024-ELECTION-SUPERCYCLE
- Main title: 2024 election supercycle continued
- Category path: World politics
- Date key: 2024
- Related domain: World / Cross-domain
- Related cards in same domain: WORLD-2024-06-INDIA, TRADE-2025-TARIFFS

#### Source context, not links
- S004: Reuters: 2024 global elections graphic — 2024 had elections in countries home to almost half the world population; used as election-supercycle context.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Elections in countries representing nearly half of humanity made 2024 a global political reset year, including India, EU, UK, France and U.S. This mattered because Useful background: many post-cutoff political assumptions changed in a short period.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Elections in countries representing nearly half of humanity made 2024 a global political reset year, including India, EU, UK, France and U.S. Wichtig daran ist: Useful background: many post-cutoff political assumptions changed in a short period.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for World / Cross-domain and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2024 in World politics?
2. Why does 2024 election supercycle continued matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Elections in countries representing nearly half of humanity made 2024 a global political reset year, including India, EU, UK, France and U.S. The important point is that Useful background: many post-cutoff political assumptions changed in a short period. Confidence is high; staleness is medium."

### DOSSIER ME-2025-GAZA-CEASEFIRE - Gaza ceasefire/hostage diplomacy remained fragile

**Anchor date/period:** 2025-01  
**Domain:** Middle East / Iran / Israel / Syria  
**Category:** Middle East / Gaza  
**Confidence/Staleness:** medium / high

#### What happened
Early 2025 saw renewed Gaza ceasefire/hostage-release diplomacy, but stability remained fragile and later regional conflicts kept evolving.

#### Why this changed the offline baseline
Do not assume Gaza/Israel war state from June 2024 remained unchanged. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: ME-2025-GAZA-CEASEFIRE
- Main title: Gaza ceasefire/hostage diplomacy remained fragile
- Category path: Middle East / Gaza
- Date key: 2025-01
- Related domain: Middle East / Iran / Israel / Syria
- Related cards in same domain: ME-2024-09-LEBANON, SYRIA-2024-12-ASSAD-FALL, IRAN-2026-01-SHUTDOWN

#### Source context, not links
- S003: CFR: Ten Most Significant World Events in 2025 — High-level synthesis of 2025 world events including Trump return, AI race, trade/geopolitics.
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Early 2025 saw renewed Gaza ceasefire/hostage-release diplomacy, but stability remained fragile and later regional conflicts kept evolving. This mattered because Do not assume Gaza/Israel war state from June 2024 remained unchanged.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Early 2025 saw renewed Gaza ceasefire/hostage-release diplomacy, but stability remained fragile and later regional conflicts kept evolving. Wichtig daran ist: Do not assume Gaza/Israel war state from June 2024 remained unchanged.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for Middle East / Iran / Israel / Syria and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-01 in Middle East / Gaza?
2. Why does Gaza ceasefire/hostage diplomacy remained fragile matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Early 2025 saw renewed Gaza ceasefire/hostage-release diplomacy, but stability remained fragile and later regional conflicts kept evolving. The important point is that Do not assume Gaza/Israel war state from June 2024 remained unchanged. Confidence is medium; staleness is high."

### DOSSIER TRADE-2025-TARIFFS - Trump tariff policy reshaped global trade risk

**Anchor date/period:** 2025  
**Domain:** World / Cross-domain  
**Category:** Economy / Trade  
**Confidence/Staleness:** medium / medium

#### What happened
The second Trump administration pushed aggressive tariff/trade policies, raising inflation, supply-chain and ally-tension questions.

#### Why this changed the offline baseline
Important for economics and geopolitics; live verification needed for exact tariff rates. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: TRADE-2025-TARIFFS
- Main title: Trump tariff policy reshaped global trade risk
- Category path: Economy / Trade
- Date key: 2025
- Related domain: World / Cross-domain
- Related cards in same domain: WORLD-2024-06-INDIA, WORLD-2024-ELECTION-SUPERCYCLE

#### Source context, not links
- S003: CFR: Ten Most Significant World Events in 2025 — High-level synthesis of 2025 world events including Trump return, AI race, trade/geopolitics.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, The second Trump administration pushed aggressive tariff/trade policies, raising inflation, supply-chain and ally-tension questions. This mattered because Important for economics and geopolitics; live verification needed for exact tariff rates.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: The second Trump administration pushed aggressive tariff/trade policies, raising inflation, supply-chain and ally-tension questions. Wichtig daran ist: Important for economics and geopolitics; live verification needed for exact tariff rates.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for World / Cross-domain and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025 in Economy / Trade?
2. Why does Trump tariff policy reshaped global trade risk matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, The second Trump administration pushed aggressive tariff/trade policies, raising inflation, supply-chain and ally-tension questions. The important point is that Important for economics and geopolitics; live verification needed for exact tariff rates. Confidence is medium; staleness is medium."

### DOSSIER AI-2025-AI-ACT-GPAI - EU AI Act GPAI/governance obligations entered staged application

**Anchor date/period:** 2025-08-02  
**Domain:** AI / Models / Agents  
**Category:** AI regulation / EU  
**Confidence/Staleness:** high / medium

#### What happened
General-purpose AI obligations and governance/enforcement provisions entered their next staged application period, affecting model providers serving the EU.

#### Why this changed the offline baseline
Important for frontier AI model providers and open/closed model transparency debates. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: AI-2025-AI-ACT-GPAI
- Main title: EU AI Act GPAI/governance obligations entered staged application
- Category path: AI regulation / EU
- Date key: 2025-08-02
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S005: EU Commission: AI Act timeline — AI Act entered force 1 Aug 2024; full application 2 Aug 2026 with staged exceptions.
- S006: EU AI Act implementation timeline — Supplemental staged dates for prohibited practices, GPAI and governance obligations.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, General-purpose AI obligations and governance/enforcement provisions entered their next staged application period, affecting model providers serving the EU. This mattered because Important for frontier AI model providers and open/closed model transparency debates.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: General-purpose AI obligations and governance/enforcement provisions entered their next staged application period, affecting model providers serving the EU. Wichtig daran ist: Important for frontier AI model providers and open/closed model transparency debates.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-08-02 in AI regulation / EU?
2. Why does EU AI Act GPAI/governance obligations entered staged application matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, General-purpose AI obligations and governance/enforcement provisions entered their next staged application period, affecting model providers serving the EU. The important point is that Important for frontier AI model providers and open/closed model transparency debates. Confidence is high; staleness is medium."

### DOSSIER MEDIA-2025-DIGITALNEWS - Digital news trust/platform shifts continued

**Anchor date/period:** 2025-06  
**Domain:** AI / Models / Agents  
**Category:** Media / AI / Society  
**Confidence/Staleness:** medium / medium

#### What happened
Reuters Institute's 2025 Digital News Report framed journalism against uncertainty, platform fragmentation, AI and climate/conflict pressures.

#### Why this changed the offline baseline
Useful for understanding media ecosystem and information trust. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: MEDIA-2025-DIGITALNEWS
- Main title: Digital news trust/platform shifts continued
- Category path: Media / AI / Society
- Date key: 2025-06
- Related domain: AI / Models / Agents
- Related cards in same domain: AI-2024-06-CLAUDE35, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, AI-2024-12-GEMINI20, AI-2024-12-O3, AI-2025-01-STARGATE, AI-2025-01-DEEPSEEK

#### Source context, not links
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, Reuters Institute's 2025 Digital News Report framed journalism against uncertainty, platform fragmentation, AI and climate/conflict pressures. This mattered because Useful for understanding media ecosystem and information trust.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: Reuters Institute's 2025 Digital News Report framed journalism against uncertainty, platform fragmentation, AI and climate/conflict pressures. Wichtig daran ist: Useful for understanding media ecosystem and information trust.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for AI / Models / Agents and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025-06 in Media / AI / Society?
2. Why does Digital news trust/platform shifts continued matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, Reuters Institute's 2025 Digital News Report framed journalism against uncertainty, platform fragmentation, AI and climate/conflict pressures. The important point is that Useful for understanding media ecosystem and information trust. Confidence is medium; staleness is medium."

### DOSSIER GAMES-2025-SWITCH2 - Nintendo Switch successor era began

**Anchor date/period:** 2025  
**Domain:** War / Ukraine / Russia  
**Category:** Games / Hardware  
**Confidence/Staleness:** medium / medium

#### What happened
The games industry moved into a new hardware/platform cycle around Nintendo's Switch successor and publisher showcase resets.

#### Why this changed the offline baseline
Useful as gaming-market context, but exact launch details should be verified in current sources. For a model whose training ended around mid-2024 or earlier, this item should be treated as a post-cutoff correction or extension. It should not be projected backward into dates before it was known. It is a dated context item, not a permanent update.

#### Safe answer boundary
An offline model may state the event, date/period, actors explicitly named in the card, and why it matters. It should avoid adding unverified details, casualties, numbers, quotes, or later outcomes unless those details appear elsewhere in the current update package. If the user asks about the current/live state after 2026-06-19, the model should request a newer update or online verification.

#### Retrieval aliases
- Card ID: GAMES-2025-SWITCH2
- Main title: Nintendo Switch successor era began
- Category path: Games / Hardware
- Date key: 2025
- Related domain: War / Ukraine / Russia
- Related cards in same domain: none selected

#### Source context, not links
- S054: Wikipedia Current events portal — Discovery source for current events by month; use as secondary discovery, not sole authority.

#### Model-facing phrasing
- English: According to the 2026-06-19 offline briefing, The games industry moved into a new hardware/platform cycle around Nintendo's Switch successor and publisher showcase resets. This mattered because Useful as gaming-market context, but exact launch details should be verified in current sources.
- German: Laut dem Offline-Briefing vom 2026-06-19 gilt: The games industry moved into a new hardware/platform cycle around Nintendo's Switch successor and publisher showcase resets. Wichtig daran ist: Useful as gaming-market context, but exact launch details should be verified in current sources.

#### Reasoning implications
- Treat this as a node in a chronological chain, not as timeless truth.
- If this card conflicts with older pre-2024-06-01 model knowledge, prefer this card for the stated date/period.
- If this card has high staleness, reduce assertiveness and state that the situation may have changed after the snapshot.
- If the user asks why the item matters, connect it to the domain summary for War / Ukraine / Russia and the related cards listed above.

#### Do-not-infer rules
- Do not invent hidden motives, exact legal wording, casualty figures, vote totals, model benchmark numbers, or military details unless present in the package.
- Do not treat source IDs as live verification; they are provenance anchors for an offline snapshot.
- Do not use this card as evidence for future developments after 2026-06-19.

#### Possible user questions this card helps answer
1. What happened around 2025 in Games / Hardware?
2. Why does Nintendo Switch successor era began matter for post-2024 context?
3. What old assumption should a local model correct because of this event?

#### Minimal answer template
"As of the 2026-06-19 offline update, The games industry moved into a new hardware/platform cycle around Nintendo's Switch successor and publisher showcase resets. The important point is that Useful as gaming-market context, but exact launch details should be verified in current sources. Confidence is medium; staleness is medium."



## 2026-06-20 Update Cards

### CARD ME-2026-06-SWISSTALKS — U.S. and Iran envoys headed to Switzerland while ceasefire conditions remained fragile
Date: 2026-06-20
Cat: Middle East / USA / Iran / Diplomacy
Meta: conf=medium; stale=high; src=S055,S056
Use: OU-HIGH-STALENESS
Event:
U.S. envoy Steve Witkoff and Iranian foreign minister Abbas Araqchi were reported en route to Switzerland for talks intended to turn a recent interim U.S.-Iran pact into a more durable peace arrangement. The talks sit inside a fragile regional setting: Lebanon/Hezbollah ceasefire implementation, Israeli concerns and military action, Iran nuclear-program issues, and reopening or stabilizing the Strait of Hormuz.
Why it matters:
This is a high-staleness anchor for June 2026 because it connects energy markets, Gulf security, Israel/Lebanon dynamics, U.S. domestic politics, sanctions relief, nuclear verification and regional proxy issues. Offline models should not treat the talks as a completed settlement.
Key details:
- Main actors: Donald Trump administration; Steve Witkoff; Abbas Araqchi; Iran; Israel; Hezbollah; Switzerland as facilitation venue.
- Reported objective: convert an interim pact into a longer-term peace or negotiation framework.
- Open issues: nuclear restrictions/verification, sanctions relief, regional proxies, Lebanon ceasefire compliance, Israeli participation/objections, and Hormuz shipping/security.
- Staleness note: fast-moving diplomacy and military incidents may have superseded this by the time it is read.

### CARD ME-2026-06-LEBANON-CEASEFIRE-FRAGILE — Israel-Hezbollah ceasefire was immediately strained by deadly strikes
Date: 2026-06-19..2026-06-20
Cat: Middle East / Lebanon / Israel / Hezbollah / War
Meta: conf=medium; stale=high; src=S056,S057
Use: OU-HIGH-STALENESS
Event:
Reuters reported that Israel and Hezbollah had agreed to a ceasefire beginning Friday afternoon, but Israeli strikes in Lebanon killed at least 10 people hours after the ceasefire was supposed to take effect. Israel said the strikes responded to Hezbollah projectiles and threats; Lebanese reports included civilian casualties and at least one Lebanese soldier.
Why it matters:
The incident shows that a formal ceasefire can fail operationally even if diplomats announce it. For offline reasoning, this is a strong example of why Middle East cards require high-staleness treatment and why the U.S.-Iran deal cannot be read as automatically ending all linked conflicts.
Key details:
- Ceasefire brokered with U.S. and Qatari involvement and Iranian assistance/support.
- Israel was not a direct party to the U.S.-Iran negotiation framework and continued to assert military-security needs.
- Reported deaths and strikes make the Lebanon front a test case for whether the wider regional de-escalation is real or only declaratory.

### CARD AI-2026-06-JUMPER-ANTHROPIC — AlphaFold co-creator John Jumper left Google DeepMind for Anthropic
Date: 2026-06-19
Cat: AI / Science / Talent / BioAI
Meta: conf=high; stale=medium; src=S058
Event:
John Jumper, a senior Google DeepMind researcher and co-creator of AlphaFold, announced he was leaving DeepMind for Anthropic. Jumper shared the 2024 Nobel Prize in Chemistry with Demis Hassabis and David Baker for protein-structure work. His move became another marker of intense AI talent competition between major labs and startups.
Why it matters:
This connects foundation-model competition with scientific AI and biology. Anthropic's recruitment of a major AlphaFold figure suggests that frontier AI companies continue to treat science tooling, reasoning systems and high-end research talent as strategic assets, not just chat-product inputs.
Key details:
- Main actors: John Jumper; Google DeepMind; Anthropic; Demis Hassabis; AlphaFold.
- Context: AI labs compete for top researchers, with startups offering focused missions and potentially less bureaucracy.
- Offline relation: updates older assumptions that DeepMind retained most marquee AlphaFold leadership.

### CARD DEV-2026-06-NODE-SECURITY-V5 — Node.js June 2026 security releases patched high-severity issues
Date: 2026-06-18..2026-06-20
Cat: Programming / Security / Node.js
Meta: conf=high; stale=low; src=S059,S060
Event:
The Node.js project issued June 2026 security releases for supported release lines including 22.x, 24.x and 26.x. Node.js v26.3.1 notes listed high-severity fixes for TLS hostname normalization/wildcard-depth authentication behavior and a WebCrypto AES integer overflow that could lead to process abort/DoS. Additional medium-severity fixes covered proxy credential redaction, HTTP/2 origin-set memory growth, and SNI context matching.
Why it matters:
For admins and developers, this is a concrete patch-management item. Offline models advising on Node deployments should prefer patched runtime versions rather than generic advice.
Key details:
- Affected release lines: Node.js 22, 24 and 26.
- Example patched current release: Node.js 26.3.1.
- High-severity CVEs named in official notes: CVE-2026-48618 and CVE-2026-48933.
- Action orientation: upgrade supported Node.js runtimes promptly, especially exposed services using TLS/WebCrypto/HTTP2/proxy paths.

### CARD DEV-2026-06-PYTHON-UV — Python 3.14.6 and uv 0.11.23 anchored June 2026 Python tooling state
Date: 2026-06-10..2026-06-19
Cat: Programming / Python / Packaging
Meta: conf=high; stale=low; src=S061,S062
Event:
Python 3.14.6 was released on 2026-06-10 as the sixth maintenance release of Python 3.14, with roughly 179 bugfixes, build improvements and documentation changes since 3.14.5. uv 0.11.23 appeared on PyPI with a 2026-06-19 release date; nearby uv release notes also show continued support for newer CPython patch releases.
Why it matters:
This is useful for offline developer assistance: Python 3.14 is no longer future-facing in this snapshot; it is an established maintenance line. uv remains an important Rust-based Python project/package manager and is relevant for fast, reproducible, cache-friendly local/offline Python workflows.
Key details:
- Python 3.14.6 release date: 2026-06-10.
- uv latest observed PyPI release in this snapshot: 0.11.23 on 2026-06-19.
- Offline install relevance: uv and local caches/wheelhouses remain useful for machines without reliable internet.

### CARD OPENAI-2026-06-TASKS-ADMIN — ChatGPT Scheduled Tasks and admin usage controls matured
Date: 2026-06-17..2026-06-20
Cat: AI Products / OpenAI / Admin / Automation
Meta: conf=high; stale=medium; src=S063,S064
Event:
OpenAI release notes described Scheduled Tasks in ChatGPT as easier to find and manage, with a Scheduled page in the sidebar for active tasks, next-run visibility, pause/resume/edit/delete controls, and reliability improvements. Enterprise/Edu notes described workspace usage-limit tools that let admins set monthly credit limits by workspace, group and user and review increase requests.
Why it matters:
For offline-context reasoning, this shows a broader 2026 product trend: AI systems are moving from passive chat toward scheduled work, monitoring, admin-governed usage and operational automation. It also affects how organizations manage AI cost and governance.
Key details:
- Scheduled Tasks: recurring/one-time work and monitoring-style workflows became more discoverable/manageable.
- Enterprise/Edu: usage limits and billing/analytics controls became a workspace administration layer.
- Offline-model relation: do not assume ChatGPT is only synchronous chat; by this snapshot it has explicit task scheduling/automation surfaces.

### CARD AI-2026-06-G7-TRUSTED-PARTNERS — G7 discussed allied access to restricted frontier AI models
Date: 2026-06-16..2026-06-18
Cat: AI Governance / G7 / Security / Allies
Meta: conf=medium; stale=medium; src=S065,S066
Event:
G7 discussions included the question of whether trusted democratic partners should receive access to cutting-edge U.S. AI models for cybersecurity and safety work, against the backdrop of U.S. restrictions on foreign access to certain advanced models. French President Emmanuel Macron publicly argued for democratic cooperation and warned against overly nationalist restrictions, while AI leaders including Sam Altman and Dario Amodei participated in summit-linked AI discussions.
Why it matters:
This is a key AI-governance tension for 2026: frontier AI is treated simultaneously as commercial infrastructure, national-security capability, allied-defense resource, and safety-governance object. Offline models should recognize that AI regulation and access policy became geopolitical, not merely technical.
Key details:
- Themes: trusted partner access, cybersecurity, democratic AI governance, U.S. export/security controls, EU concerns.
- Actors: G7 leaders; U.S. Commerce officials; Macron; OpenAI/Anthropic/Google DeepMind leadership.
- Interpretation: not a settled treaty; an active negotiation topic.
