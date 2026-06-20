
## Global Card Usage Policy

Default: if a factual card has no explicit `Use:` field, apply `OU-DEFAULT`.

- `OU-DEFAULT`: Use the card as dated context. Mention the date/period when it affects the answer. Respect confidence/staleness. Do not invent details outside the card, chronology, event index, or supplied context.
- `OU-HIGH-STALENESS`: Use cautious wording. Say newer developments may supersede this snapshot. Prefer a current check for operational, legal, medical, financial, security, election, or active-conflict decisions.
- `OU-SPECULATIVE`: Analysis only, not fact. Use as reasoning aid; do not present as a confirmed event. Later real developments must appear only in later-dated factual updates.
- `OU-CORRECTION`: Treat this as superseding or correcting an older assumption/card for the stated date range.

Compact metadata convention: `Meta: conf=<low|medium|high>; stale=<low|medium|high>; src=<SIDs>`. Raw URLs belong only in `source_registry.md`, not in offline-facing context files.

# Event Index - names, topics, dates

Created: 2026-06-21 (Europe/Berlin date)
Coverage: 2024-06-01 to 2026-06-21
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



## 2026-06-20 indexed additions

- `ME-2026-06-SWISSTALKS` - U.S.-Iran talks in Switzerland; Steve Witkoff; Abbas Araqchi; interim pact; Hormuz; nuclear issues; Lebanon ceasefire; high-staleness diplomacy.
- `ME-2026-06-LEBANON-CEASEFIRE-FRAGILE` - Israel-Hezbollah ceasefire strained by deadly Israeli strikes in Lebanon; U.S./Qatar mediation; Iran-linked regional de-escalation; high staleness.
- `AI-2026-06-JUMPER-ANTHROPIC` - John Jumper leaves Google DeepMind for Anthropic; AlphaFold; AI-for-science talent competition; Nobel 2024 context.
- `DEV-2026-06-NODE-SECURITY-V5` - Node.js June 2026 security releases; Node 22/24/26; Node 26.3.1; CVE-2026-48618; CVE-2026-48933.
- `DEV-2026-06-PYTHON-UV` - Python 3.14.6; uv 0.11.23; Python packaging/tooling state.
- `OPENAI-2026-06-TASKS-ADMIN` - Scheduled Tasks management; Enterprise/Edu usage limits; ChatGPT admin/automation surface.
- `AI-2026-06-G7-TRUSTED-PARTNERS` - G7 trusted partner access to frontier AI models; democratic AI governance; U.S./EU tension.


## 2026-06-21 added/updated index entries

- Buergenstock U.S.-Iran talks | 2026-06-20..21 | See CARD ME-2026-06-USIRAN-BUERGENSTOCK | Themes: Iran, USA, Switzerland, Hormuz, diplomacy, ceasefire, nuclear verification.
- Tyumen refinery strike | 2026-06-20..21 | See CARD UA-2026-06-TYUMEN-DRONE | Themes: Ukraine, Russia, drones, oil infrastructure, deep strike, war economics.
- Zelenskiy large-attack warning | 2026-06-20..21 | See CARD UA-2026-06-RUSSIAN-ATTACK-WARNING | Themes: Ukraine civilian risk, Russian strikes, air raids, escalation.
- G7 AI statecraft | 2026-06-16..21 | See CARD AI-2026-06-G7-AI-STATECRAFT | Themes: AI governance, export control, trusted partners, national security, G7.
- Qatar aircraft / U.S. political controversy | 2026-06-20..21 | See CARD US-2026-06-QATAR-AIRCRAFT-CONTROVERSY | Themes: Trump administration, Air Force One symbolism, foreign gifts, intelligence leadership.
- World Cup June 21 schedule | 2026-06-21 | See CARD CULTURE-2026-06-WORLDCUP-JUN21 | Themes: sports, culture, World Cup 2026, schedule staleness.
