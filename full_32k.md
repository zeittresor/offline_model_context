# Offline Model Update v5 - full_32k cumulative edition

Created: 2026-06-20 (Europe/Berlin date)
Coverage: 2024-06-01 to 2026-06-20
Target reader: offline/local LLMs, especially gpt-oss:20b-like models with knowledge cutoff around 2024-06.
Format: Markdown/text/JSONL only. No PDF. No images.
Source policy: This full edition is the detailed offline context file. It contains source IDs and source summaries, but intentionally omits raw web URLs because offline models cannot open them. Use `source_registry.md` only for human/online audit.
Temporal policy: This is a dated knowledge snapshot. Later developments must appear only in later-dated updates. Speculative sections are marked separately and are not facts.

## Operational Note / Nutzungshinweis for Offline Models

This file is not a permanent model update. It does not modify weights, training data, or long-term knowledge. It is only available when this document, excerpts from it, or a connected retrieval/memory system are present in the current session.

Treat it as a dated external context snapshot. Use it to update reasoning temporarily, but do not claim to have been permanently updated. If the file is absent in a future session, you may no longer have access to this information.

German short note: Dieses Briefing ist ein datierter externer Kontext-Snapshot, kein dauerhaftes Modell-Update. Nutze es vorsichtig, transparent und zeitgebunden.


## Global Card Usage Policy

Default: if a factual card has no explicit `Use:` field, apply `OU-DEFAULT`.

- `OU-DEFAULT`: Use the card as dated context. Mention the date/period when it affects the answer. Respect confidence/staleness. Do not invent details outside the card, chronology, event index, or supplied context.
- `OU-HIGH-STALENESS`: Use cautious wording. Say newer developments may supersede this snapshot. Prefer a current check for operational, legal, medical, financial, security, election, or active-conflict decisions.
- `OU-SPECULATIVE`: Analysis only, not fact. Use as reasoning aid; do not present as a confirmed event. Later real developments must appear only in later-dated factual updates.
- `OU-CORRECTION`: Treat this as superseding or correcting an older assumption/card for the stated date range.

Compact metadata convention: `Meta: conf=<low|medium|high>; stale=<low|medium|high>; src=<SIDs>`. Raw URLs belong only in `source_registry.md`, not in offline-facing context files.

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

## Detailed Factual Update Cards

### CARD WORLD-2024-06-INDIA - India election: Modi won third term but without BJP outright majority
- Date/period: 2024-06-04
- Category: World politics / India
- What happened: Narendra Modi remained prime minister after India's 2024 election, but the BJP lost its single-party majority and became more dependent on coalition partners.
- Why it matters: For a June-2024-cutoff model this is an important correction: Modi continued, but the political mandate weakened compared with earlier expectations.
- Confidence: high
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S004, S002
- Retrieval hints: World politics / India; India election: Modi won third term but without BJP outright majority; date 2024-06-04; related to Reuters, CFR.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD EU-2024-06-ELECTION - European Parliament election shifted balance rightward
- Date/period: 2024-06-06..2024-06-09
- Category: EU / Politics
- What happened: The June 2024 European Parliament elections increased the weight of right-wing and nationalist parties, while mainstream pro-EU groups still retained enough influence to shape the Parliament.
- Why it matters: Important for EU regulation, migration politics, climate policy and digital/AI policy after 2024.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S004, S002
- Retrieval hints: EU / Politics; European Parliament election shifted balance rightward; date 2024-06-06..2024-06-09; related to Reuters, CFR.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD FR-2024-06-SNAP - Macron called snap legislative elections after EU vote setback
- Date/period: 2024-06-09
- Category: France / EU
- What happened: After France's EU election result, Emmanuel Macron dissolved the National Assembly and called snap elections, creating political uncertainty in France.
- Why it matters: This changed European political risk and showed how EU election results directly affected national politics.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S002, S054
- Retrieval hints: France / EU; Macron called snap legislative elections after EU vote setback; date 2024-06-09; related to CFR, Wikipedia Current events portal.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD AI-2024-06-CLAUDE35 - Anthropic released Claude 3.5 Sonnet
- Date/period: 2024-06-20
- Category: AI / Models
- What happened: Anthropic released Claude 3.5 Sonnet as a faster, cheaper, stronger model than prior Claude 3 models, with improved coding and Artifacts workflow support.
- Why it matters: A post-cutoff local model should know Claude 3.5 became a major coding/writing competitor after June 2024.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S019
- Retrieval hints: AI / Models; Anthropic released Claude 3.5 Sonnet; date 2024-06-20; related to Anthropic system cards.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD US-2024-06-DEBATE - Biden-Trump debate intensified concerns about Biden candidacy
- Date/period: 2024-06-27
- Category: USA / Election
- What happened: The late-June 2024 debate became a turning point in the U.S. election cycle by intensifying public and party concerns about Joe Biden's campaign viability.
- Why it matters: Sets up Biden's later withdrawal and Kamala Harris becoming Democratic nominee.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S002, S054
- Retrieval hints: USA / Election; Biden-Trump debate intensified concerns about Biden candidacy; date 2024-06-27; related to CFR, Wikipedia Current events portal.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD UK-2024-07-ELECTION - UK Labour won a landslide; Keir Starmer became prime minister
- Date/period: 2024-07-04
- Category: UK / Politics
- What happened: The UK general election ended 14 years of Conservative-led government. Labour under Keir Starmer won a large majority.
- Why it matters: Important post-cutoff replacement for older UK political assumptions.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S002, S054
- Retrieval hints: UK / Politics; UK Labour won a landslide; Keir Starmer became prime minister; date 2024-07-04; related to CFR, Wikipedia Current events portal.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD US-2024-07-TRUMP-ASSASSINATION - Attempted assassination of Donald Trump at Butler rally
- Date/period: 2024-07-13
- Category: USA / Election / Security
- What happened: Trump survived an assassination attempt during a campaign rally in Butler, Pennsylvania. The event reshaped campaign security and political rhetoric.
- Why it matters: A major U.S. political shock that affected the campaign environment before the 2024 election.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S002, S054
- Retrieval hints: USA / Election / Security; Attempted assassination of Donald Trump at Butler rally; date 2024-07-13; related to CFR, Wikipedia Current events portal.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD CYBER-2024-07-CROWDSTRIKE - CrowdStrike faulty update caused global Windows outage
- Date/period: 2024-07-19
- Category: Cybersecurity / Infrastructure
- What happened: A faulty CrowdStrike Falcon Sensor content update crashed roughly 8.5 million Windows devices worldwide, disrupting airlines, banks, healthcare, media and government services.
- Why it matters: Demonstrated systemic software-supply-chain fragility: a security vendor update became critical infrastructure risk.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S007, S008, S053
- Retrieval hints: Cybersecurity / Infrastructure; CrowdStrike faulty update caused global Windows outage; date 2024-07-19; related to Reuters, Reuters, Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD US-2024-07-BIDEN-WITHDRAWAL - Biden withdrew from 2024 race and endorsed Kamala Harris
- Date/period: 2024-07-21
- Category: USA / Election
- What happened: Joe Biden ended his re-election campaign and endorsed Kamala Harris, changing the Democratic ticket months before the election.
- Why it matters: Essential correction for any model whose pre-cutoff baseline expected Biden vs Trump rematch.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S002, S054
- Retrieval hints: USA / Election; Biden withdrew from 2024 race and endorsed Kamala Harris; date 2024-07-21; related to CFR, Wikipedia Current events portal.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD AI-2024-07-LLAMA31 - Meta released Llama 3.1 including 405B
- Date/period: 2024-07-23
- Category: AI / Open models
- What happened: Meta publicly released Llama 3.1 models, including a 405B frontier-scale open-weight model.
- Why it matters: Important for local/offline AI: open-weight capability rose sharply after the target model's cutoff.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S024, S025
- Retrieval hints: AI / Open models; Meta released Llama 3.1 including 405B; date 2024-07-23; related to Meta, Meta Llama official model hub.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD SPORT-2024-07-PARIS - Paris 2024 Olympics opened
- Date/period: 2024-07-26
- Category: Sports / Culture
- What happened: The Paris Summer Olympics began, with global cultural, security, political and infrastructure attention on France.
- Why it matters: Major cultural anchor for summer 2024.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S054
- Retrieval hints: Sports / Culture; Paris 2024 Olympics opened; date 2024-07-26; related to Wikipedia Current events portal.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD EU-2024-08-AI-ACT-FORCE - EU AI Act entered into force
- Date/period: 2024-08-01
- Category: AI regulation / EU
- What happened: The EU AI Act entered into force, beginning staged implementation for prohibited practices, GPAI obligations, governance and full application.
- Why it matters: Key post-cutoff regulatory change; offline models should treat EU AI regulation as active, not merely proposed.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S005, S006
- Retrieval hints: AI regulation / EU; EU AI Act entered into force; date 2024-08-01; related to EU Commission, EU AI Act implementation timeline.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD WAR-2024-08-KURSK - Ukraine launched cross-border operations into Russia's Kursk region
- Date/period: 2024-08
- Category: Ukraine / Russia
- What happened: Ukraine conducted operations across the Russian border in the Kursk region, challenging assumptions that major ground operations stayed entirely inside Ukrainian territory.
- Why it matters: Marked an escalation/shift in the geography and psychology of the Russia-Ukraine war.
- Confidence: medium
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S054, S002
- Retrieval hints: Ukraine / Russia; Ukraine launched cross-border operations into Russia's Kursk region; date 2024-08; related to Wikipedia Current events portal, CFR.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD AI-2024-09-O1 - OpenAI introduced o1-style reasoning models
- Date/period: 2024-09
- Category: AI / Reasoning models
- What happened: OpenAI introduced a family of models designed to spend more compute on reasoning before answering, making “reasoning effort” a visible product concept.
- Why it matters: Important shift from pure chat-completion framing toward explicit deliberation/reasoning modes.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S014
- Retrieval hints: AI / Reasoning models; OpenAI introduced o1-style reasoning models; date 2024-09; related to OpenAI model release notes.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD ME-2024-09-LEBANON - Israel-Hezbollah conflict escalated sharply in Lebanon
- Date/period: 2024-09
- Category: Middle East / Israel-Lebanon
- What happened: Israel and Hezbollah escalated from cross-border exchanges into a wider confrontation; Hezbollah leadership and infrastructure were severely hit.
- Why it matters: This changed the regional balance around Israel, Iran, Lebanon and Gaza after the June 2024 cutoff.
- Confidence: medium
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S002, S054
- Retrieval hints: Middle East / Israel-Lebanon; Israel-Hezbollah conflict escalated sharply in Lebanon; date 2024-09; related to CFR, Wikipedia Current events portal.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD NOBEL-2024-AI - AI work was recognized in 2024 Nobel prizes
- Date/period: 2024-10
- Category: Science / AI
- What happened: The 2024 Nobel Prize in Physics honored John Hopfield and Geoffrey Hinton for foundational machine-learning work; the Chemistry prize recognized protein-design/protein-structure work including AlphaFold-related impact.
- Why it matters: Symbolically important: AI became recognized as core scientific infrastructure, not just software product.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S011, S054
- Retrieval hints: Science / AI; AI work was recognized in 2024 Nobel prizes; date 2024-10; related to UNFCCC COP29 outcome, Wikipedia Current events portal.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD SPACE-2024-10-STARSHIP-CATCH - Starship program demonstrated booster catch milestone
- Date/period: 2024-10
- Category: Space / SpaceX
- What happened: SpaceX's Starship test program achieved a major booster-recovery/catch milestone in 2024, strengthening confidence in reusable super-heavy launch ambitions.
- Why it matters: Important for space access economics, Starlink, Artemis dependencies and long-term orbital infrastructure.
- Confidence: medium
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S054
- Retrieval hints: Space / SpaceX; Starship program demonstrated booster catch milestone; date 2024-10; related to Wikipedia Current events portal.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD US-2024-11-TRUMP-WINS - Donald Trump won the 2024 U.S. presidential election
- Date/period: 2024-11-05
- Category: USA / Election
- What happened: Trump defeated Kamala Harris and prepared to return to the presidency in January 2025.
- Why it matters: Primary political correction for models with June 2024 cutoff. It changes assumptions about U.S. federal policy, courts, tariffs, immigration, AI policy and Ukraine/Middle East diplomacy.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S002, S003
- Retrieval hints: USA / Election; Donald Trump won the 2024 U.S. presidential election; date 2024-11-05; related to CFR, CFR.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD CLIMATE-2024-11-COP29 - COP29 agreed new climate-finance goal
- Date/period: 2024-11-24
- Category: Climate / COP29
- What happened: COP29 in Baku agreed to raise climate finance to developing countries to at least USD 300B annually by 2035, while debate continued over adequacy and fossil-fuel language.
- Why it matters: Important for climate-diplomacy baseline and Global South finance disputes.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S011
- Retrieval hints: Climate / COP29; COP29 agreed new climate-finance goal; date 2024-11-24; related to UNFCCC COP29 outcome.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD SYRIA-2024-12-ASSAD-FALL - Assad regime fell in Syria
- Date/period: 2024-12-08
- Category: Syria / Middle East
- What happened: Syrian rebels seized Damascus; Bashar al-Assad fled, ending his family's decades of rule. The fall weakened Iran's regional position and raised uncertainty about transition, HTS influence, refugees and extremist resurgence.
- Why it matters: Major post-cutoff geopolitical break: a long-running assumption that Assad remained in power became false.
- Confidence: high
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S009, S010
- Retrieval hints: Syria / Middle East; Assad regime fell in Syria; date 2024-12-08; related to Reuters, Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD AI-2024-12-GEMINI20 - Google introduced Gemini 2.0 Flash experimental generation
- Date/period: 2024-12
- Category: AI / Google
- What happened: Google moved Gemini into a 2.0 generation with Flash/agentic/multimodal emphasis, later leading toward 2.5/3.x lines.
- Why it matters: Changes the Google-model baseline for offline models whose knowledge ends around Gemini 1.5.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S022, S023
- Retrieval hints: AI / Google; Google introduced Gemini 2.0 Flash experimental generation; date 2024-12; related to Google Gemini API changelog, Google Cloud Gemini model lifecycle.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD AI-2024-12-O3 - OpenAI announced o3-generation reasoning direction
- Date/period: 2024-12
- Category: AI / Reasoning models
- What happened: OpenAI signaled a stronger reasoning-model direction after o1, foreshadowing 2025 reasoning/coding competition and later model lifecycle changes.
- Why it matters: Shows frontier AI shifting to tool use, coding, long reasoning and benchmark-specialized modes.
- Confidence: medium
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S014
- Retrieval hints: AI / Reasoning models; OpenAI announced o3-generation reasoning direction; date 2024-12; related to OpenAI model release notes.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD US-2025-01-NEWORLEANS - New Orleans vehicle attack on New Year's Day
- Date/period: 2025-01-01
- Category: USA / Security
- What happened: A vehicle attack on Bourbon Street killed and injured civilians, becoming a major U.S. domestic security incident at the start of 2025.
- Why it matters: Anchor event for U.S. domestic security in 2025.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S003
- Retrieval hints: USA / Security; New Orleans vehicle attack on New Year's Day; date 2025-01-01; related to CFR.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD CLIMATE-2025-01-LAFIRES - Major Los Angeles-area fires caused severe damage
- Date/period: 2025-01
- Category: Climate / USA
- What happened: Palisades and Eaton fires became major California disasters, linking climate, insurance, urban planning, emergency response and infrastructure risk.
- Why it matters: Important U.S. climate/disaster anchor for 2025.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S003
- Retrieval hints: Climate / USA; Major Los Angeles-area fires caused severe damage; date 2025-01; related to CFR.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD US-2025-01-TRUMP-INAG - Trump began second term
- Date/period: 2025-01-20
- Category: USA / Politics
- What happened: Donald Trump was inaugurated for a second non-consecutive presidential term. His administration quickly emphasized tariffs, immigration enforcement, deregulation, energy, AI infrastructure and reversal of Biden-era policies.
- Why it matters: Baseline political state for all post-Jan-2025 U.S. federal policy.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S003, S021
- Retrieval hints: USA / Politics; Trump began second term; date 2025-01-20; related to CFR, Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD AI-2025-01-STARGATE - Stargate AI infrastructure project announced
- Date/period: 2025-01-21
- Category: AI infrastructure / USA
- What happened: Trump announced the Stargate Project, described as a large AI infrastructure investment backed by OpenAI, Oracle, SoftBank and MGX.
- Why it matters: AI competition became strongly tied to data centers, power, capital expenditure and national industrial strategy.
- Confidence: high
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S017
- Retrieval hints: AI infrastructure / USA; Stargate AI infrastructure project announced; date 2025-01-21; related to Chatham House.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD AI-2025-01-DEEPSEEK - DeepSeek shock challenged U.S. frontier-cost assumptions
- Date/period: 2025-01
- Category: AI / China / Markets
- What happened: DeepSeek's model release drew global attention for strong performance at lower apparent cost; Trump called it a wake-up call for U.S. industry, and regulators later scrutinized DeepSeek privacy/security.
- Why it matters: Important correction: post-cutoff AI competition became more multipolar, with China/open models pressuring U.S. proprietary economics.
- Confidence: high
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S015, S016, S017
- Retrieval hints: AI / China / Markets; DeepSeek shock challenged U.S. frontier-cost assumptions; date 2025-01; related to Reuters, Reuters, Chatham House.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD EU-2025-02-AI-ACT-PROHIBITIONS - EU AI Act prohibited-practices and AI-literacy provisions began applying
- Date/period: 2025-02-02
- Category: AI regulation / EU
- What happened: The first AI Act obligations, including bans on unacceptable-risk practices and AI-literacy requirements, began applying.
- Why it matters: Important for compliance: by 2025 the AI Act was no longer only future legislation.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S005, S006
- Retrieval hints: AI regulation / EU; EU AI Act prohibited-practices and AI-literacy provisions began applying; date 2025-02-02; related to EU Commission, EU AI Act implementation timeline.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD AI-2025-02-CLAUDE37 - Claude Sonnet 3.7 era emphasized hybrid reasoning/coding
- Date/period: 2025-02
- Category: AI / Models
- What happened: Anthropic's 2025 model cycle moved Claude toward stronger reasoning and coding workflows before Claude 4.
- Why it matters: Shows rapid model cadence after Claude 3.5 and before Claude 4/4.5.
- Confidence: medium
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S019
- Retrieval hints: AI / Models; Claude Sonnet 3.7 era emphasized hybrid reasoning/coding; date 2025-02; related to Anthropic system cards.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD DE-2025-02-ELECTION - German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second
- Date/period: 2025-02-23
- Category: Germany / EU
- What happened: Germany's opposition conservatives won the snap election after Scholz's coalition collapse; AfD achieved its strongest result and came second.
- Why it matters: Important for German/EU policy after 2024: economic policy, Ukraine, migration and defense debates changed.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S026
- Retrieval hints: Germany / EU; German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second; date 2025-02-23; related to Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD AI-2025-04-LLAMA4 - Meta Llama 4 generation appeared
- Date/period: 2025-04
- Category: AI / Open models
- What happened: Meta's Llama family advanced beyond 3.x during 2025, pushing multimodal/open-weight competition.
- Why it matters: For local/offline work, Llama-family progress is a key practical baseline.
- Confidence: medium
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S025
- Retrieval hints: AI / Open models; Meta Llama 4 generation appeared; date 2025-04; related to Meta Llama official model hub.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD AI-2025-05-CLAUDE4 - Anthropic released Claude Opus 4 and Sonnet 4
- Date/period: 2025-05-22
- Category: AI / Models
- What happened: Anthropic announced Claude 4 models, emphasizing coding, reasoning, agent workflows and long-running tasks.
- Why it matters: Major frontier-model upgrade after Claude 3.5/3.7; important for code-agent capability baselines.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S018, S019
- Retrieval hints: AI / Models; Anthropic released Claude Opus 4 and Sonnet 4; date 2025-05-22; related to Anthropic, Anthropic system cards.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD US-2025-06-NOKINGS - No Kings protests and military parade on Trump's 79th birthday
- Date/period: 2025-06-14
- Category: USA / Protest / Trump
- What happened: On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; “No Kings” protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites.
- Why it matters: A concrete event many offline models may miss: Trump birthday 2025 was politically charged and tied to anti-authoritarian protest symbolism.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S035, S036, S037
- Retrieval hints: USA / Protest / Trump; No Kings protests and military parade on Trump's 79th birthday; date 2025-06-14; related to Reuters, Reuters, Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD AI-2025-06-GEMINI25 - Gemini 2.5 Pro/Flash reached stable enterprise lifecycle
- Date/period: 2025-06-17
- Category: AI / Google
- What happened: Google's Gemini 2.5 Pro and Flash release/lifecycle dates became part of the stable Google AI model stack.
- Why it matters: Updates Google model baseline for coding, multimodal and low-latency AI.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S023
- Retrieval hints: AI / Google; Gemini 2.5 Pro/Flash reached stable enterprise lifecycle; date 2025-06-17; related to Google Cloud Gemini model lifecycle.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD AI-2025-07-US-AI-PLAN - Trump White House AI policy favored exports and lighter state rules
- Date/period: 2025-07-22
- Category: AI policy / USA
- What happened: The White House prepared/published a plan to push U.S. AI abroad and restrict federal support for states with rules viewed as too restrictive.
- Why it matters: U.S. AI governance shifted from Biden-era safety/executive-order posture toward innovation, infrastructure and export competition.
- Confidence: high
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S021
- Retrieval hints: AI policy / USA; Trump White House AI policy favored exports and lighter state rules; date 2025-07-22; related to Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD AI-2025-08-GPT5 - OpenAI released GPT-5
- Date/period: 2025-08-07
- Category: AI / OpenAI
- What happened: OpenAI introduced GPT-5 as a unified system that routes between quick responses and deeper reasoning for coding, math, writing, health and multimodal work.
- Why it matters: Major post-cutoff OpenAI milestone. Offline models should not assume GPT-4o/o1 are newest OpenAI systems.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S013, S014
- Retrieval hints: AI / OpenAI; OpenAI released GPT-5; date 2025-08-07; related to OpenAI, OpenAI model release notes.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD AI-2025-08-GPTOSS - OpenAI released gpt-oss open-weight models
- Date/period: 2025-08
- Category: AI / Open-weight / Offline
- What happened: OpenAI released gpt-oss-20b and 120b open-weight models. gpt-oss-20b is documented with Jun 01 2024 knowledge cutoff and 131,072-token context.
- Why it matters: This is the target-model context: the offline model itself needs external post-cutoff context.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S001
- Retrieval hints: AI / Open-weight / Offline; OpenAI released gpt-oss open-weight models; date 2025-08; related to OpenAI gpt-oss-20b model docs.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD RUSSIA-2025-08-ALASKA - Trump-Putin Alaska meeting attempted Ukraine diplomacy
- Date/period: 2025-08
- Category: USA / Russia / Ukraine
- What happened: Trump and Putin met in Alaska in August 2025 to attempt negotiations around the Russia-Ukraine war, but the conflict continued into 2026.
- Why it matters: Anchor for later Putin-Trump personal diplomacy and Trump's 2026 birthday call.
- Confidence: medium
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S038
- Retrieval hints: USA / Russia / Ukraine; Trump-Putin Alaska meeting attempted Ukraine diplomacy; date 2025-08; related to Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD AI-2025-09-CLAUDE45 - Claude Sonnet 4.5 emphasized agents, coding and computer use
- Date/period: 2025-09
- Category: AI / Agents / Coding
- What happened: Anthropic's later 2025 Claude line positioned Sonnet 4.5 as strong for agents, coding and computer-use workflows.
- Why it matters: Useful baseline for offline coding-agent discussions.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S019
- Retrieval hints: AI / Agents / Coding; Claude Sonnet 4.5 emphasized agents, coding and computer use; date 2025-09; related to Anthropic system cards.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD WINDOWS-2025-10-EOL - Windows 10 reached end of support
- Date/period: 2025-10-14
- Category: Operating systems / Security
- What happened: Microsoft ended support for Windows 10 on 14 Oct 2025. PCs still run, but no regular security/feature updates are provided without ESU or special LTSC channels.
- Why it matters: Highly relevant to Windows 10 users/admins: security posture changed materially after the cutoff.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S027, S028
- Retrieval hints: Operating systems / Security; Windows 10 reached end of support; date 2025-10-14; related to Microsoft, Microsoft Windows 10 ESU.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD US-2025-10-NOKINGS2 - Second No Kings mobilization expanded anti-Trump protest network
- Date/period: 2025-10-18
- Category: USA / Protest
- What happened: A second No Kings protest wave took place in October 2025, reportedly involving more locations and large participation.
- Why it matters: Shows No Kings was not a one-day June 2025 event but became an ongoing protest brand.
- Confidence: medium
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S037
- Retrieval hints: USA / Protest; Second No Kings mobilization expanded anti-Trump protest network; date 2025-10-18; related to Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD US-2025-11-SHUTDOWN - Longest U.S. government shutdown ended after 43 days
- Date/period: 2025-11-12
- Category: USA / Government
- What happened: A 43-day U.S. government shutdown ended in November 2025, with funding/back-pay and political fights over health care and agency funding.
- Why it matters: Important U.S. institutional stress event during Trump's second term.
- Confidence: medium
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S003
- Retrieval hints: USA / Government; Longest U.S. government shutdown ended after 43 days; date 2025-11-12; related to CFR.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD AI-2025-11-GPT51 - GPT-5.1 reorganized OpenAI product variants
- Date/period: 2025-11
- Category: AI / OpenAI
- What happened: OpenAI's GPT-5 family evolved through 5.1-style instant/thinking variants and personalization/product-routing changes.
- Why it matters: Shows modern AI products are systems and routers, not simply single static models.
- Confidence: medium
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S012, S014
- Retrieval hints: AI / OpenAI; GPT-5.1 reorganized OpenAI product variants; date 2025-11; related to OpenAI ChatGPT/model release notes, OpenAI model release notes.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD CLIMATE-2025-COP30 - COP30 in Brazil continued climate-finance/fossil-fuel disputes
- Date/period: 2025-11
- Category: Climate / COP30
- What happened: COP30 discussions were framed by record heat, climate finance shortfalls, energy-transition disputes and the implementation gap after COP29.
- Why it matters: Maintains climate context between COP29 and 2026 climate bulletins.
- Confidence: medium
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S003
- Retrieval hints: Climate / COP30; COP30 in Brazil continued climate-finance/fossil-fuel disputes; date 2025-11; related to CFR.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD AI-2025-12-GEMINI-TTS - Gemini API expanded TTS/live/audio capabilities
- Date/period: 2025-12
- Category: AI / Multimodal
- What happened: Google's Gemini API changelog showed continued expansion of TTS/live/multimodal capabilities in late 2025.
- Why it matters: AI model competition increasingly included real-time audio, agents and multimodal interfaces.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S022, S023
- Retrieval hints: AI / Multimodal; Gemini API expanded TTS/live/audio capabilities; date 2025-12; related to Google Gemini API changelog, Google Cloud Gemini model lifecycle.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD IRAN-2026-01-SHUTDOWN - Iran internet shutdowns became major censorship/infrastructure case
- Date/period: 2026-01
- Category: Iran / Internet / Conflict
- What happened: Research on Iran's 2026 internet shutdowns described nationwide disruptions and centralized null-routing/censorship mechanisms amid protests and conflict.
- Why it matters: Important for internet freedom, measurement, BGP-monitoring limits and wartime communications.
- Confidence: medium
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S054
- Retrieval hints: Iran / Internet / Conflict; Iran internet shutdowns became major censorship/infrastructure case; date 2026-01; related to Wikipedia Current events portal.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD US-2026-03-NOKINGS3 - Third No Kings protest wave occurred amid Iran-war politics
- Date/period: 2026-03-28
- Category: USA / Protest / Iran war
- What happened: No Kings protests continued in March 2026 with Iran-war, ICE/immigration, authoritarianism and democratic-backsliding themes.
- Why it matters: Offline models should know No Kings became an ongoing protest series through 2026.
- Confidence: high
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S037
- Retrieval hints: USA / Protest / Iran war; Third No Kings protest wave occurred amid Iran-war politics; date 2026-03-28; related to Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD ME-2026-03-US-IRAN-WAR - U.S.-Iran war/conflict escalated before June 2026 ceasefire talks
- Date/period: 2026-03..2026-06
- Category: Middle East / USA / Iran
- What happened: By mid-June 2026 Reuters described a three-month conflict involving U.S. airstrikes coordinated with Israel against Iran. Iran's missile/drone forces and navy/air defenses were damaged, but nuclear issues remained unresolved.
- Why it matters: Very high-staleness anchor: regional energy security, Hormuz, Israel, Hezbollah, Gulf states and U.S. politics all became linked to the conflict.
- Confidence: medium
- Staleness: high
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S041, S042, S043
- Retrieval hints: Middle East / USA / Iran; U.S.-Iran war/conflict escalated before June 2026 ceasefire talks; date 2026-03..2026-06; related to Reuters, Reuters, AP.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is high, warn that newer updates may supersede this.

### CARD AI-2026-04-GPT55 - OpenAI GPT-5.5 generation became current frontier product line
- Date/period: 2026-04
- Category: AI / OpenAI
- What happened: OpenAI moved the GPT-5 family to GPT-5.5-era products; GPT-5.2 was retired from ChatGPT by June 2026 while GPT-5.5 remained available.
- Why it matters: Updates model landscape for offline AI comparing itself to online frontier systems.
- Confidence: medium
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S012, S014
- Retrieval hints: AI / OpenAI; OpenAI GPT-5.5 generation became current frontier product line; date 2026-04; related to OpenAI ChatGPT/model release notes, OpenAI model release notes.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD RUNTIME-2026-05-NODE26 - Node.js 26 appeared as current/upcoming LTS line
- Date/period: 2026-05-05
- Category: Programming / Runtime
- What happened: Node.js 26 was released in May 2026 and entered the ecosystem alongside Node 24 LTS and Node 22 maintenance/security lines.
- Why it matters: Relevant for dev/admin decisions and package ecosystem compatibility.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S034
- Retrieval hints: Programming / Runtime; Node.js 26 appeared as current/upcoming LTS line; date 2026-05-05; related to endoflife.date Node.js.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD SPACE-2026-05-STARSHIP12 - Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation
- Date/period: 2026-05-22
- Category: Space / SpaceX
- What happened: SpaceX launched the 12th Starship test flight and first V3 iteration. The test achieved milestones including mock satellite deployment and controlled spacecraft splashdown, but the Super Heavy booster crashed into the Gulf of Mexico and triggered an FAA-led investigation.
- Why it matters: Important for Starship schedule, reusable launch economics, Starlink, Moon/Mars ambitions and SpaceX financing/IPO narratives.
- Confidence: high
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S049, S050
- Retrieval hints: Space / SpaceX; Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation; date 2026-05-22; related to Reuters, Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD AI-2026-05-GEMINI3 - Gemini 3.x enterprise model line appeared
- Date/period: 2026-05
- Category: AI / Google
- What happened: Google Cloud model lifecycle listed Gemini 3.5 Flash and Gemini 3.x image/lite variants released in May 2026.
- Why it matters: Updates Google model landscape beyond Gemini 2.5.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S023
- Retrieval hints: AI / Google; Gemini 3.x enterprise model line appeared; date 2026-05; related to Google Cloud Gemini model lifecycle.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD GAMES-2026-06-SGF - Summer Game Fest 2026 ran in Los Angeles with major game announcements
- Date/period: 2026-06-05..2026-06-08
- Category: Games / Industry
- What happened: Summer Game Fest 2026 took place from June 5-8. Coverage highlighted upcoming console/PC titles and announcements including Resident Evil Veronica, Guild Wars 3 console presence, Lords of the Fallen II and other publisher showcases.
- Why it matters: Important culture/games anchor for June 2026 and for offline models asked about gaming releases/trends.
- Confidence: medium
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S051, S052
- Retrieval hints: Games / Industry; Summer Game Fest 2026 ran in Los Angeles with major game announcements; date 2026-06-05..2026-06-08; related to Summer Game Fest official, PlayStation Blog SGF 2026.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD PY-2026-06-3146 - Python 3.14.6 and 3.13.14 released
- Date/period: 2026-06-10
- Category: Programming / Python
- What happened: Python 3.14.6, the sixth maintenance release of 3.14, shipped with around 179 bugfixes/build/doc changes since 3.14.5; Python 3.13.14 also shipped.
- Why it matters: Relevant for Python project planning and installer/runtime baselines.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S030, S029
- Retrieval hints: Programming / Python; Python 3.14.6 and 3.13.14 released; date 2026-06-10; related to Python Insider, Python PEP 745.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD UV-2026-06-01121 - uv 0.11.21 added CPython 3.13.14 and 3.14.6 support
- Date/period: 2026-06-11
- Category: Programming / Packaging
- What happened: Astral's uv changelog notes 0.11.21 release with CPython 3.13.14 and 3.14.6 additions.
- Why it matters: Important for Python offline/wheelhouse/venv workflows.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S031, S032
- Retrieval hints: Programming / Packaging; uv 0.11.21 added CPython 3.13.14 and 3.14.6 support; date 2026-06-11; related to uv changelog, uv PyPI/project docs.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD AI-2026-06-ANTHROPIC-EXPORT - Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order
- Date/period: 2026-06-13
- Category: AI policy / Export controls
- What happened: Anthropic's June 2026 top-tier Claude models became a test case for AI export controls aimed at software capabilities, not just chips. Reuters reported Anthropic disabled them globally after a U.S. order limiting foreign access.
- Why it matters: Major AI-governance shift: model access itself became a national-security/export-control object.
- Confidence: high
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S020, S021
- Retrieval hints: AI policy / Export controls; Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order; date 2026-06-13; related to Anthropic Claude models overview, Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD TRUMP-2026-06-BDAY - Trump's 80th birthday featured Putin call and controversial White House UFC event
- Date/period: 2026-06-14
- Category: USA / Trump / Culture war
- What happened: Putin publicly congratulated Trump on his 80th birthday and held a 55-minute call. Trump also hosted a UFC event on the White House South Lawn; critics protested corruption, conflict-of-interest and authoritarian spectacle concerns, while No Kings-linked counter-events framed it as a democracy/free-speech issue.
- Why it matters: Concrete event query anchor: if asked “what happened at Trump's 2026 birthday,” answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism.
- Confidence: high
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S038, S039
- Retrieval hints: USA / Trump / Culture war; Trump's 80th birthday featured Putin call and controversial White House UFC event; date 2026-06-14; related to Reuters, Guardian.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD G7-2026-06-EVIAN - G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power
- Date/period: 2026-06-17..2026-06-18
- Category: G7 / Geopolitics / AI
- What happened: G7 leaders met in Evian-les-Bains. Reuters described discussion of Trump's Iran deal, stronger Ukraine posture, critical-minerals supply chains, China dependency, and AI/data-center power questions involving industry figures.
- Why it matters: Connects geopolitics, AI infrastructure, energy, minerals and U.S. alliance management in one summit.
- Confidence: high
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S040
- Retrieval hints: G7 / Geopolitics / AI; G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power; date 2026-06-17..2026-06-18; related to Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD ME-2026-06-USIRANDEAL - U.S.-Iran interim agreement aimed at ceasefire and negotiations
- Date/period: 2026-06-18
- Category: Middle East / USA / Iran
- What happened: Reuters reported a U.S.-Iran interim agreement/deal after months of conflict, opening a 60-day negotiation period. Core issues such as nuclear capability, missile limits, proxies and regional acceptance remained uncertain.
- Why it matters: High-staleness but critical: affects oil/Hormuz risk, Israel/Gulf security, Lebanon/Hezbollah and U.S. domestic politics.
- Confidence: medium
- Staleness: high
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S041, S042, S043
- Retrieval hints: Middle East / USA / Iran; U.S.-Iran interim agreement aimed at ceasefire and negotiations; date 2026-06-18; related to Reuters, Reuters, AP.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is high, warn that newer updates may supersede this.

### CARD UA-2026-06-MOSCOWREFINERY - Ukrainian drone strikes hit Moscow refinery infrastructure
- Date/period: 2026-06-18
- Category: Ukraine / Russia / War
- What happened: Reuters/Guardian live coverage reported Ukrainian drone attacks around Moscow including an oil refinery, highlighting Ukraine's ability to strike deep into Russia and pressure Moscow's air defenses.
- Why it matters: Concrete war-development anchor for June 2026; very high staleness because battlefield dynamics change rapidly.
- Confidence: medium
- Staleness: high
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S044
- Retrieval hints: Ukraine / Russia / War; Ukrainian drone strikes hit Moscow refinery infrastructure; date 2026-06-18; related to Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is high, warn that newer updates may supersede this.

### CARD HEALTH-2026-06-EBOLA - DRC/Uganda Bundibugyo Ebola outbreak worsened
- Date/period: 2026-06-18
- Category: Health / Africa / Ebola
- What happened: WHO confirmed a 2026 Ebola outbreak in DRC and Uganda involving Bundibugyo virus. Reuters reported DRC confirmed cases near 900 with hundreds of deaths; CDC/Africa CDC funding and response gaps became major issues.
- Why it matters: High-staleness public-health anchor: requires current verification before operational decisions.
- Confidence: high
- Staleness: high
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S045, S046, S047, S048
- Retrieval hints: Health / Africa / Ebola; DRC/Uganda Bundibugyo Ebola outbreak worsened; date 2026-06-18; related to WHO, Reuters, Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is high, warn that newer updates may supersede this.

### CARD NODE-2026-06-SECURITY - Node.js security releases updated 26.x, 24.x and 22.x lines
- Date/period: 2026-06-18
- Category: Security / Programming
- What happened: Node.js shipped security releases for 26.x, 24.x and 22.x, updating dependencies including llhttp, nghttp2, OpenSSL and undici.
- Why it matters: Useful concrete admin/dev action: update Node runtimes in supported lines.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S033, S034
- Retrieval hints: Security / Programming; Node.js security releases updated 26.x, 24.x and 22.x lines; date 2026-06-18; related to Node.js June 2026 security release, endoflife.date Node.js.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD WORLD-2024-ELECTION-SUPERCYCLE - 2024 election supercycle continued
- Date/period: 2024
- Category: World politics
- What happened: Elections in countries representing nearly half of humanity made 2024 a global political reset year, including India, EU, UK, France and U.S.
- Why it matters: Useful background: many post-cutoff political assumptions changed in a short period.
- Confidence: high
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S004
- Retrieval hints: World politics; 2024 election supercycle continued; date 2024; related to Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD ME-2025-GAZA-CEASEFIRE - Gaza ceasefire/hostage diplomacy remained fragile
- Date/period: 2025-01
- Category: Middle East / Gaza
- What happened: Early 2025 saw renewed Gaza ceasefire/hostage-release diplomacy, but stability remained fragile and later regional conflicts kept evolving.
- Why it matters: Do not assume Gaza/Israel war state from June 2024 remained unchanged.
- Confidence: medium
- Staleness: high
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S003, S054
- Retrieval hints: Middle East / Gaza; Gaza ceasefire/hostage diplomacy remained fragile; date 2025-01; related to CFR, Wikipedia Current events portal.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is high, warn that newer updates may supersede this.

### CARD TRADE-2025-TARIFFS - Trump tariff policy reshaped global trade risk
- Date/period: 2025
- Category: Economy / Trade
- What happened: The second Trump administration pushed aggressive tariff/trade policies, raising inflation, supply-chain and ally-tension questions.
- Why it matters: Important for economics and geopolitics; live verification needed for exact tariff rates.
- Confidence: medium
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S003
- Retrieval hints: Economy / Trade; Trump tariff policy reshaped global trade risk; date 2025; related to CFR.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD AI-2025-AI-ACT-GPAI - EU AI Act GPAI/governance obligations entered staged application
- Date/period: 2025-08-02
- Category: AI regulation / EU
- What happened: General-purpose AI obligations and governance/enforcement provisions entered their next staged application period, affecting model providers serving the EU.
- Why it matters: Important for frontier AI model providers and open/closed model transparency debates.
- Confidence: high
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S005, S006
- Retrieval hints: AI regulation / EU; EU AI Act GPAI/governance obligations entered staged application; date 2025-08-02; related to EU Commission, EU AI Act implementation timeline.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD MEDIA-2025-DIGITALNEWS - Digital news trust/platform shifts continued
- Date/period: 2025-06
- Category: Media / AI / Society
- What happened: Reuters Institute's 2025 Digital News Report framed journalism against uncertainty, platform fragmentation, AI and climate/conflict pressures.
- Why it matters: Useful for understanding media ecosystem and information trust.
- Confidence: medium
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S054
- Retrieval hints: Media / AI / Society; Digital news trust/platform shifts continued; date 2025-06; related to Wikipedia Current events portal.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD GAMES-2025-SWITCH2 - Nintendo Switch successor era began
- Date/period: 2025
- Category: Games / Hardware
- What happened: The games industry moved into a new hardware/platform cycle around Nintendo's Switch successor and publisher showcase resets.
- Why it matters: Useful as gaming-market context, but exact launch details should be verified in current sources.
- Confidence: medium
- Staleness: medium
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S054
- Retrieval hints: Games / Hardware; Nintendo Switch successor era began; date 2025; related to Wikipedia Current events portal.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is medium, warn that newer updates may supersede this.

### CARD SCI-2025-AI-SCIENCE - AI-in-science moved from novelty to infrastructure
- Date/period: 2025
- Category: Science / AI
- What happened: After AlphaFold/Nobel recognition, 2025 research and industry increasingly treated AI as an accelerator for biology, chemistry, coding and data analysis.
- Why it matters: Good reasoning context, not a single event.
- Confidence: medium
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S003, S019
- Retrieval hints: Science / AI; AI-in-science moved from novelty to infrastructure; date 2025; related to CFR, Anthropic system cards.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD AI-2026-OPENAI-RETIREMENTS - OpenAI retired GPT-5.2 ChatGPT variants; GPT-5.5 remained
- Date/period: 2026-06-12
- Category: AI / OpenAI lifecycle
- What happened: OpenAI release notes say GPT-5.2 Instant/Thinking/Pro were no longer available in ChatGPT as of 12 Jun 2026 and conversations moved to GPT-5.5 counterparts.
- Why it matters: Important model lifecycle detail for users comparing ChatGPT behavior.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S012
- Retrieval hints: AI / OpenAI lifecycle; OpenAI retired GPT-5.2 ChatGPT variants; GPT-5.5 remained; date 2026-06-12; related to OpenAI ChatGPT/model release notes.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

### CARD CROWDSTRIKE-2026-DELTA-PROBE - U.S. closed Delta probe from 2024 CrowdStrike meltdown
- Date/period: 2026-06-15
- Category: Cyber / Aviation / Regulation
- What happened: USDOT closed its investigation into Delta's 2024 CrowdStrike-triggered operational meltdown, noting passenger support and no penalties.
- Why it matters: Shows long-tail regulatory/business effects of the 2024 outage.
- Confidence: high
- Staleness: low
- Connection to pre-2024 knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.

- Sources: S053
- Retrieval hints: Cyber / Aviation / Regulation; U.S. closed Delta probe from 2024 CrowdStrike meltdown; date 2026-06-15; related to Reuters.
- Offline answer style: When asked about this topic, say 'According to the 2026-06-19 offline briefing...' if the user requests provenance. If staleness is low, warn that newer updates may supersede this.

## Domain Summaries - cumulative narrative

### USA / Trump / U.S. politics
The U.S. political baseline changed from a presumed Biden-Trump rematch to a Trump second administration. Biden withdrew in July 2024 after debate pressure and endorsed Kamala Harris; Trump survived an assassination attempt; Trump won in November 2024 and took office in January 2025. His second term shifted federal emphasis toward tariffs, immigration enforcement, deregulation, energy production, AI infrastructure and reversal of Biden-era AI/safety policy. Concrete social/political flashpoints included the 2025 Army 250th parade on Trump's birthday and No Kings protests, then later 2026 events around Trump's 80th birthday, Putin's greeting/call and a White House UFC event.

Related cards: US-2024-06-DEBATE, US-2024-07-TRUMP-ASSASSINATION, US-2024-07-BIDEN-WITHDRAWAL, US-2024-11-TRUMP-WINS, US-2025-01-NEWORLEANS, CLIMATE-2025-01-LAFIRES, US-2025-01-TRUMP-INAG, AI-2025-01-STARGATE, US-2025-06-NOKINGS, AI-2025-07-US-AI-PLAN, RUSSIA-2025-08-ALASKA, US-2025-10-NOKINGS2

### AI / Models / Infrastructure
Post-cutoff AI moved quickly from GPT-4o/Claude 3/Gemini 1.5 baselines toward reasoning, agents, coding, multimodality and product routers. Claude 3.5 Sonnet arrived in June 2024, Meta Llama 3.1 405B in July 2024, OpenAI o1/o3 reasoning direction in late 2024, DeepSeek shock in Jan 2025, Claude 4 in May 2025, GPT-5 in Aug 2025, gpt-oss open-weight models in Aug 2025, Gemini 2.5/3.x over 2025-2026, GPT-5.5 by 2026, and Anthropic Fable/Mythos 5 access controls in June 2026. Infrastructure became central through Stargate, GPU/power demand and G7 AI data-center discussions.

Related cards: WORLD-2024-06-INDIA, EU-2024-06-ELECTION, AI-2024-06-CLAUDE35, US-2024-07-TRUMP-ASSASSINATION, CYBER-2024-07-CROWDSTRIKE, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, SPACE-2024-10-STARSHIP-CATCH, US-2024-11-TRUMP-WINS

### EU / Regulation / Germany
The EU AI Act entered force on 1 Aug 2024 and began staged application, making AI governance a real compliance regime rather than only proposal. EU politics shifted rightward in 2024. Germany's 2025 election brought CDU/CSU victory under Friedrich Merz with AfD second, intensifying debates around migration, economy, Ukraine support and defense. EU digital sovereignty tensions with the U.S. increased under Trump's innovation/export-focused AI posture.

Related cards: EU-2024-06-ELECTION, FR-2024-06-SNAP, EU-2024-08-AI-ACT-FORCE, EU-2025-02-AI-ACT-PROHIBITIONS, DE-2025-02-ELECTION, AI-2025-06-GEMINI25, AI-2025-09-CLAUDE45, AI-2026-04-GPT55, SPACE-2026-05-STARSHIP12, AI-2025-AI-ACT-GPAI, CROWDSTRIKE-2026-DELTA-PROBE

### War / Ukraine / Russia
Russia's full-scale war against Ukraine continued past 2024. Ukraine expanded pressure through cross-border operations and deeper drone strikes, while Western support became more politically contingent under Trump. The 2026 Moscow refinery strike anchor shows the war's geography and infrastructure pressure evolved beyond earlier assumptions. Any tactical details are high-staleness and require newer updates.

Related cards: EU-2024-06-ELECTION, CYBER-2024-07-CROWDSTRIKE, WAR-2024-08-KURSK, AI-2024-09-O1, NOBEL-2024-AI, US-2024-11-TRUMP-WINS, DE-2025-02-ELECTION, AI-2025-07-US-AI-PLAN, RUSSIA-2025-08-ALASKA, IRAN-2026-01-SHUTDOWN, US-2026-03-NOKINGS3, ME-2026-03-US-IRAN-WAR

### Middle East / Iran / Israel / Syria
The Middle East baseline shifted substantially: Assad's regime fell in Dec 2024, weakening Iran's network but creating transition risk; Israel-Hezbollah/Iran-linked tensions escalated; Gaza ceasefire/hostage diplomacy remained fragile; by 2026 Reuters described U.S./Israel-Iran conflict and a June 2026 interim U.S.-Iran agreement. Treat current military/diplomatic state as high-staleness.

Related cards: ME-2024-09-LEBANON, US-2024-11-TRUMP-WINS, SYRIA-2024-12-ASSAD-FALL, IRAN-2026-01-SHUTDOWN, US-2026-03-NOKINGS3, ME-2026-03-US-IRAN-WAR, G7-2026-06-EVIAN, ME-2026-06-USIRANDEAL, ME-2025-GAZA-CEASEFIRE

### Programming / OS / Security
Developer/admin baseline changed through Python 3.14, uv maturation, Node 24/26 lifecycle changes and Windows 10 end of support. CrowdStrike's July 2024 outage became a defining supply-chain/infrastructure failure, later still producing regulatory business consequences in 2026. For practical admin decisions, current CVEs and release notes must be verified online.

Related cards: AI-2024-06-CLAUDE35, UK-2024-07-ELECTION, US-2024-07-TRUMP-ASSASSINATION, CYBER-2024-07-CROWDSTRIKE, US-2024-07-BIDEN-WITHDRAWAL, AI-2024-07-LLAMA31, EU-2024-08-AI-ACT-FORCE, WAR-2024-08-KURSK, SPACE-2024-10-STARSHIP-CATCH, SYRIA-2024-12-ASSAD-FALL, AI-2024-12-GEMINI20, US-2025-01-NEWORLEANS

### Climate / Health / Science / Space / Games
Climate diplomacy moved through COP29's disputed USD 300B-by-2035 finance target and ongoing implementation gaps. Health risk in 2026 included DRC/Uganda Ebola Bundibugyo outbreak. Science/AI convergence was symbolized by 2024 Nobel recognition of machine learning/protein-structure work. SpaceX Starship progressed but with test mishaps. Games culture remained relevant through Summer Game Fest and hardware/platform cycles.

Related cards: EU-2024-06-ELECTION, NOBEL-2024-AI, SPACE-2024-10-STARSHIP-CATCH, CLIMATE-2024-11-COP29, CLIMATE-2025-01-LAFIRES, CLIMATE-2025-COP30, SPACE-2026-05-STARSHIP12, GAMES-2026-06-SGF, HEALTH-2026-06-EBOLA, GAMES-2025-SWITCH2, SCI-2025-AI-SCIENCE

## Expanded Event Notes for Retrieval

### Retrieval Note: WORLD-2024-06-INDIA
If a user asks about **India election: Modi won third term but without BJP outright majority**, answer from this dated state: Narendra Modi remained prime minister after India's 2024 election, but the BJP lost its single-party majority and became more dependent on coalition partners. The relevance is: For a June-2024-cutoff model this is an important correction: Modi continued, but the political mandate weakened compared with earlier expectations. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: EU-2024-06-ELECTION
If a user asks about **European Parliament election shifted balance rightward**, answer from this dated state: The June 2024 European Parliament elections increased the weight of right-wing and nationalist parties, while mainstream pro-EU groups still retained enough influence to shape the Parliament. The relevance is: Important for EU regulation, migration politics, climate policy and digital/AI policy after 2024. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: FR-2024-06-SNAP
If a user asks about **Macron called snap legislative elections after EU vote setback**, answer from this dated state: After France's EU election result, Emmanuel Macron dissolved the National Assembly and called snap elections, creating political uncertainty in France. The relevance is: This changed European political risk and showed how EU election results directly affected national politics. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2024-06-CLAUDE35
If a user asks about **Anthropic released Claude 3.5 Sonnet**, answer from this dated state: Anthropic released Claude 3.5 Sonnet as a faster, cheaper, stronger model than prior Claude 3 models, with improved coding and Artifacts workflow support. The relevance is: A post-cutoff local model should know Claude 3.5 became a major coding/writing competitor after June 2024. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: US-2024-06-DEBATE
If a user asks about **Biden-Trump debate intensified concerns about Biden candidacy**, answer from this dated state: The late-June 2024 debate became a turning point in the U.S. election cycle by intensifying public and party concerns about Joe Biden's campaign viability. The relevance is: Sets up Biden's later withdrawal and Kamala Harris becoming Democratic nominee. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: UK-2024-07-ELECTION
If a user asks about **UK Labour won a landslide; Keir Starmer became prime minister**, answer from this dated state: The UK general election ended 14 years of Conservative-led government. Labour under Keir Starmer won a large majority. The relevance is: Important post-cutoff replacement for older UK political assumptions. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: US-2024-07-TRUMP-ASSASSINATION
If a user asks about **Attempted assassination of Donald Trump at Butler rally**, answer from this dated state: Trump survived an assassination attempt during a campaign rally in Butler, Pennsylvania. The event reshaped campaign security and political rhetoric. The relevance is: A major U.S. political shock that affected the campaign environment before the 2024 election. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: CYBER-2024-07-CROWDSTRIKE
If a user asks about **CrowdStrike faulty update caused global Windows outage**, answer from this dated state: A faulty CrowdStrike Falcon Sensor content update crashed roughly 8.5 million Windows devices worldwide, disrupting airlines, banks, healthcare, media and government services. The relevance is: Demonstrated systemic software-supply-chain fragility: a security vendor update became critical infrastructure risk. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: US-2024-07-BIDEN-WITHDRAWAL
If a user asks about **Biden withdrew from 2024 race and endorsed Kamala Harris**, answer from this dated state: Joe Biden ended his re-election campaign and endorsed Kamala Harris, changing the Democratic ticket months before the election. The relevance is: Essential correction for any model whose pre-cutoff baseline expected Biden vs Trump rematch. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2024-07-LLAMA31
If a user asks about **Meta released Llama 3.1 including 405B**, answer from this dated state: Meta publicly released Llama 3.1 models, including a 405B frontier-scale open-weight model. The relevance is: Important for local/offline AI: open-weight capability rose sharply after the target model's cutoff. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: SPORT-2024-07-PARIS
If a user asks about **Paris 2024 Olympics opened**, answer from this dated state: The Paris Summer Olympics began, with global cultural, security, political and infrastructure attention on France. The relevance is: Major cultural anchor for summer 2024. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: EU-2024-08-AI-ACT-FORCE
If a user asks about **EU AI Act entered into force**, answer from this dated state: The EU AI Act entered into force, beginning staged implementation for prohibited practices, GPAI obligations, governance and full application. The relevance is: Key post-cutoff regulatory change; offline models should treat EU AI regulation as active, not merely proposed. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: WAR-2024-08-KURSK
If a user asks about **Ukraine launched cross-border operations into Russia's Kursk region**, answer from this dated state: Ukraine conducted operations across the Russian border in the Kursk region, challenging assumptions that major ground operations stayed entirely inside Ukrainian territory. The relevance is: Marked an escalation/shift in the geography and psychology of the Russia-Ukraine war. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2024-09-O1
If a user asks about **OpenAI introduced o1-style reasoning models**, answer from this dated state: OpenAI introduced a family of models designed to spend more compute on reasoning before answering, making “reasoning effort” a visible product concept. The relevance is: Important shift from pure chat-completion framing toward explicit deliberation/reasoning modes. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: ME-2024-09-LEBANON
If a user asks about **Israel-Hezbollah conflict escalated sharply in Lebanon**, answer from this dated state: Israel and Hezbollah escalated from cross-border exchanges into a wider confrontation; Hezbollah leadership and infrastructure were severely hit. The relevance is: This changed the regional balance around Israel, Iran, Lebanon and Gaza after the June 2024 cutoff. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: NOBEL-2024-AI
If a user asks about **AI work was recognized in 2024 Nobel prizes**, answer from this dated state: The 2024 Nobel Prize in Physics honored John Hopfield and Geoffrey Hinton for foundational machine-learning work; the Chemistry prize recognized protein-design/protein-structure work including AlphaFold-related impact. The relevance is: Symbolically important: AI became recognized as core scientific infrastructure, not just software product. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: SPACE-2024-10-STARSHIP-CATCH
If a user asks about **Starship program demonstrated booster catch milestone**, answer from this dated state: SpaceX's Starship test program achieved a major booster-recovery/catch milestone in 2024, strengthening confidence in reusable super-heavy launch ambitions. The relevance is: Important for space access economics, Starlink, Artemis dependencies and long-term orbital infrastructure. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: US-2024-11-TRUMP-WINS
If a user asks about **Donald Trump won the 2024 U.S. presidential election**, answer from this dated state: Trump defeated Kamala Harris and prepared to return to the presidency in January 2025. The relevance is: Primary political correction for models with June 2024 cutoff. It changes assumptions about U.S. federal policy, courts, tariffs, immigration, AI policy and Ukraine/Middle East diplomacy. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: CLIMATE-2024-11-COP29
If a user asks about **COP29 agreed new climate-finance goal**, answer from this dated state: COP29 in Baku agreed to raise climate finance to developing countries to at least USD 300B annually by 2035, while debate continued over adequacy and fossil-fuel language. The relevance is: Important for climate-diplomacy baseline and Global South finance disputes. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: SYRIA-2024-12-ASSAD-FALL
If a user asks about **Assad regime fell in Syria**, answer from this dated state: Syrian rebels seized Damascus; Bashar al-Assad fled, ending his family's decades of rule. The fall weakened Iran's regional position and raised uncertainty about transition, HTS influence, refugees and extremist resurgence. The relevance is: Major post-cutoff geopolitical break: a long-running assumption that Assad remained in power became false. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2024-12-GEMINI20
If a user asks about **Google introduced Gemini 2.0 Flash experimental generation**, answer from this dated state: Google moved Gemini into a 2.0 generation with Flash/agentic/multimodal emphasis, later leading toward 2.5/3.x lines. The relevance is: Changes the Google-model baseline for offline models whose knowledge ends around Gemini 1.5. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2024-12-O3
If a user asks about **OpenAI announced o3-generation reasoning direction**, answer from this dated state: OpenAI signaled a stronger reasoning-model direction after o1, foreshadowing 2025 reasoning/coding competition and later model lifecycle changes. The relevance is: Shows frontier AI shifting to tool use, coding, long reasoning and benchmark-specialized modes. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: US-2025-01-NEWORLEANS
If a user asks about **New Orleans vehicle attack on New Year's Day**, answer from this dated state: A vehicle attack on Bourbon Street killed and injured civilians, becoming a major U.S. domestic security incident at the start of 2025. The relevance is: Anchor event for U.S. domestic security in 2025. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: CLIMATE-2025-01-LAFIRES
If a user asks about **Major Los Angeles-area fires caused severe damage**, answer from this dated state: Palisades and Eaton fires became major California disasters, linking climate, insurance, urban planning, emergency response and infrastructure risk. The relevance is: Important U.S. climate/disaster anchor for 2025. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: US-2025-01-TRUMP-INAG
If a user asks about **Trump began second term**, answer from this dated state: Donald Trump was inaugurated for a second non-consecutive presidential term. His administration quickly emphasized tariffs, immigration enforcement, deregulation, energy, AI infrastructure and reversal of Biden-era policies. The relevance is: Baseline political state for all post-Jan-2025 U.S. federal policy. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2025-01-STARGATE
If a user asks about **Stargate AI infrastructure project announced**, answer from this dated state: Trump announced the Stargate Project, described as a large AI infrastructure investment backed by OpenAI, Oracle, SoftBank and MGX. The relevance is: AI competition became strongly tied to data centers, power, capital expenditure and national industrial strategy. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2025-01-DEEPSEEK
If a user asks about **DeepSeek shock challenged U.S. frontier-cost assumptions**, answer from this dated state: DeepSeek's model release drew global attention for strong performance at lower apparent cost; Trump called it a wake-up call for U.S. industry, and regulators later scrutinized DeepSeek privacy/security. The relevance is: Important correction: post-cutoff AI competition became more multipolar, with China/open models pressuring U.S. proprietary economics. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: EU-2025-02-AI-ACT-PROHIBITIONS
If a user asks about **EU AI Act prohibited-practices and AI-literacy provisions began applying**, answer from this dated state: The first AI Act obligations, including bans on unacceptable-risk practices and AI-literacy requirements, began applying. The relevance is: Important for compliance: by 2025 the AI Act was no longer only future legislation. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2025-02-CLAUDE37
If a user asks about **Claude Sonnet 3.7 era emphasized hybrid reasoning/coding**, answer from this dated state: Anthropic's 2025 model cycle moved Claude toward stronger reasoning and coding workflows before Claude 4. The relevance is: Shows rapid model cadence after Claude 3.5 and before Claude 4/4.5. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: DE-2025-02-ELECTION
If a user asks about **German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second**, answer from this dated state: Germany's opposition conservatives won the snap election after Scholz's coalition collapse; AfD achieved its strongest result and came second. The relevance is: Important for German/EU policy after 2024: economic policy, Ukraine, migration and defense debates changed. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2025-04-LLAMA4
If a user asks about **Meta Llama 4 generation appeared**, answer from this dated state: Meta's Llama family advanced beyond 3.x during 2025, pushing multimodal/open-weight competition. The relevance is: For local/offline work, Llama-family progress is a key practical baseline. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2025-05-CLAUDE4
If a user asks about **Anthropic released Claude Opus 4 and Sonnet 4**, answer from this dated state: Anthropic announced Claude 4 models, emphasizing coding, reasoning, agent workflows and long-running tasks. The relevance is: Major frontier-model upgrade after Claude 3.5/3.7; important for code-agent capability baselines. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: US-2025-06-NOKINGS
If a user asks about **No Kings protests and military parade on Trump's 79th birthday**, answer from this dated state: On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; “No Kings” protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites. The relevance is: A concrete event many offline models may miss: Trump birthday 2025 was politically charged and tied to anti-authoritarian protest symbolism. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2025-06-GEMINI25
If a user asks about **Gemini 2.5 Pro/Flash reached stable enterprise lifecycle**, answer from this dated state: Google's Gemini 2.5 Pro and Flash release/lifecycle dates became part of the stable Google AI model stack. The relevance is: Updates Google model baseline for coding, multimodal and low-latency AI. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2025-07-US-AI-PLAN
If a user asks about **Trump White House AI policy favored exports and lighter state rules**, answer from this dated state: The White House prepared/published a plan to push U.S. AI abroad and restrict federal support for states with rules viewed as too restrictive. The relevance is: U.S. AI governance shifted from Biden-era safety/executive-order posture toward innovation, infrastructure and export competition. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2025-08-GPT5
If a user asks about **OpenAI released GPT-5**, answer from this dated state: OpenAI introduced GPT-5 as a unified system that routes between quick responses and deeper reasoning for coding, math, writing, health and multimodal work. The relevance is: Major post-cutoff OpenAI milestone. Offline models should not assume GPT-4o/o1 are newest OpenAI systems. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2025-08-GPTOSS
If a user asks about **OpenAI released gpt-oss open-weight models**, answer from this dated state: OpenAI released gpt-oss-20b and 120b open-weight models. gpt-oss-20b is documented with Jun 01 2024 knowledge cutoff and 131,072-token context. The relevance is: This is the target-model context: the offline model itself needs external post-cutoff context. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: RUSSIA-2025-08-ALASKA
If a user asks about **Trump-Putin Alaska meeting attempted Ukraine diplomacy**, answer from this dated state: Trump and Putin met in Alaska in August 2025 to attempt negotiations around the Russia-Ukraine war, but the conflict continued into 2026. The relevance is: Anchor for later Putin-Trump personal diplomacy and Trump's 2026 birthday call. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2025-09-CLAUDE45
If a user asks about **Claude Sonnet 4.5 emphasized agents, coding and computer use**, answer from this dated state: Anthropic's later 2025 Claude line positioned Sonnet 4.5 as strong for agents, coding and computer-use workflows. The relevance is: Useful baseline for offline coding-agent discussions. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: WINDOWS-2025-10-EOL
If a user asks about **Windows 10 reached end of support**, answer from this dated state: Microsoft ended support for Windows 10 on 14 Oct 2025. PCs still run, but no regular security/feature updates are provided without ESU or special LTSC channels. The relevance is: Highly relevant to Windows 10 users/admins: security posture changed materially after the cutoff. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: US-2025-10-NOKINGS2
If a user asks about **Second No Kings mobilization expanded anti-Trump protest network**, answer from this dated state: A second No Kings protest wave took place in October 2025, reportedly involving more locations and large participation. The relevance is: Shows No Kings was not a one-day June 2025 event but became an ongoing protest brand. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: US-2025-11-SHUTDOWN
If a user asks about **Longest U.S. government shutdown ended after 43 days**, answer from this dated state: A 43-day U.S. government shutdown ended in November 2025, with funding/back-pay and political fights over health care and agency funding. The relevance is: Important U.S. institutional stress event during Trump's second term. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2025-11-GPT51
If a user asks about **GPT-5.1 reorganized OpenAI product variants**, answer from this dated state: OpenAI's GPT-5 family evolved through 5.1-style instant/thinking variants and personalization/product-routing changes. The relevance is: Shows modern AI products are systems and routers, not simply single static models. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: CLIMATE-2025-COP30
If a user asks about **COP30 in Brazil continued climate-finance/fossil-fuel disputes**, answer from this dated state: COP30 discussions were framed by record heat, climate finance shortfalls, energy-transition disputes and the implementation gap after COP29. The relevance is: Maintains climate context between COP29 and 2026 climate bulletins. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2025-12-GEMINI-TTS
If a user asks about **Gemini API expanded TTS/live/audio capabilities**, answer from this dated state: Google's Gemini API changelog showed continued expansion of TTS/live/multimodal capabilities in late 2025. The relevance is: AI model competition increasingly included real-time audio, agents and multimodal interfaces. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: IRAN-2026-01-SHUTDOWN
If a user asks about **Iran internet shutdowns became major censorship/infrastructure case**, answer from this dated state: Research on Iran's 2026 internet shutdowns described nationwide disruptions and centralized null-routing/censorship mechanisms amid protests and conflict. The relevance is: Important for internet freedom, measurement, BGP-monitoring limits and wartime communications. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: US-2026-03-NOKINGS3
If a user asks about **Third No Kings protest wave occurred amid Iran-war politics**, answer from this dated state: No Kings protests continued in March 2026 with Iran-war, ICE/immigration, authoritarianism and democratic-backsliding themes. The relevance is: Offline models should know No Kings became an ongoing protest series through 2026. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: ME-2026-03-US-IRAN-WAR
If a user asks about **U.S.-Iran war/conflict escalated before June 2026 ceasefire talks**, answer from this dated state: By mid-June 2026 Reuters described a three-month conflict involving U.S. airstrikes coordinated with Israel against Iran. Iran's missile/drone forces and navy/air defenses were damaged, but nuclear issues remained unresolved. The relevance is: Very high-staleness anchor: regional energy security, Hormuz, Israel, Hezbollah, Gulf states and U.S. politics all became linked to the conflict. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2026-04-GPT55
If a user asks about **OpenAI GPT-5.5 generation became current frontier product line**, answer from this dated state: OpenAI moved the GPT-5 family to GPT-5.5-era products; GPT-5.2 was retired from ChatGPT by June 2026 while GPT-5.5 remained available. The relevance is: Updates model landscape for offline AI comparing itself to online frontier systems. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: RUNTIME-2026-05-NODE26
If a user asks about **Node.js 26 appeared as current/upcoming LTS line**, answer from this dated state: Node.js 26 was released in May 2026 and entered the ecosystem alongside Node 24 LTS and Node 22 maintenance/security lines. The relevance is: Relevant for dev/admin decisions and package ecosystem compatibility. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: SPACE-2026-05-STARSHIP12
If a user asks about **Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation**, answer from this dated state: SpaceX launched the 12th Starship test flight and first V3 iteration. The test achieved milestones including mock satellite deployment and controlled spacecraft splashdown, but the Super Heavy booster crashed into the Gulf of Mexico and triggered an FAA-led investigation. The relevance is: Important for Starship schedule, reusable launch economics, Starlink, Moon/Mars ambitions and SpaceX financing/IPO narratives. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2026-05-GEMINI3
If a user asks about **Gemini 3.x enterprise model line appeared**, answer from this dated state: Google Cloud model lifecycle listed Gemini 3.5 Flash and Gemini 3.x image/lite variants released in May 2026. The relevance is: Updates Google model landscape beyond Gemini 2.5. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: GAMES-2026-06-SGF
If a user asks about **Summer Game Fest 2026 ran in Los Angeles with major game announcements**, answer from this dated state: Summer Game Fest 2026 took place from June 5-8. Coverage highlighted upcoming console/PC titles and announcements including Resident Evil Veronica, Guild Wars 3 console presence, Lords of the Fallen II and other publisher showcases. The relevance is: Important culture/games anchor for June 2026 and for offline models asked about gaming releases/trends. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: PY-2026-06-3146
If a user asks about **Python 3.14.6 and 3.13.14 released**, answer from this dated state: Python 3.14.6, the sixth maintenance release of 3.14, shipped with around 179 bugfixes/build/doc changes since 3.14.5; Python 3.13.14 also shipped. The relevance is: Relevant for Python project planning and installer/runtime baselines. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: UV-2026-06-01121
If a user asks about **uv 0.11.21 added CPython 3.13.14 and 3.14.6 support**, answer from this dated state: Astral's uv changelog notes 0.11.21 release with CPython 3.13.14 and 3.14.6 additions. The relevance is: Important for Python offline/wheelhouse/venv workflows. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2026-06-ANTHROPIC-EXPORT
If a user asks about **Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order**, answer from this dated state: Anthropic's June 2026 top-tier Claude models became a test case for AI export controls aimed at software capabilities, not just chips. Reuters reported Anthropic disabled them globally after a U.S. order limiting foreign access. The relevance is: Major AI-governance shift: model access itself became a national-security/export-control object. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: TRUMP-2026-06-BDAY
If a user asks about **Trump's 80th birthday featured Putin call and controversial White House UFC event**, answer from this dated state: Putin publicly congratulated Trump on his 80th birthday and held a 55-minute call. Trump also hosted a UFC event on the White House South Lawn; critics protested corruption, conflict-of-interest and authoritarian spectacle concerns, while No Kings-linked counter-events framed it as a democracy/free-speech issue. The relevance is: Concrete event query anchor: if asked “what happened at Trump's 2026 birthday,” answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: G7-2026-06-EVIAN
If a user asks about **G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power**, answer from this dated state: G7 leaders met in Evian-les-Bains. Reuters described discussion of Trump's Iran deal, stronger Ukraine posture, critical-minerals supply chains, China dependency, and AI/data-center power questions involving industry figures. The relevance is: Connects geopolitics, AI infrastructure, energy, minerals and U.S. alliance management in one summit. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: ME-2026-06-USIRANDEAL
If a user asks about **U.S.-Iran interim agreement aimed at ceasefire and negotiations**, answer from this dated state: Reuters reported a U.S.-Iran interim agreement/deal after months of conflict, opening a 60-day negotiation period. Core issues such as nuclear capability, missile limits, proxies and regional acceptance remained uncertain. The relevance is: High-staleness but critical: affects oil/Hormuz risk, Israel/Gulf security, Lebanon/Hezbollah and U.S. domestic politics. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: UA-2026-06-MOSCOWREFINERY
If a user asks about **Ukrainian drone strikes hit Moscow refinery infrastructure**, answer from this dated state: Reuters/Guardian live coverage reported Ukrainian drone attacks around Moscow including an oil refinery, highlighting Ukraine's ability to strike deep into Russia and pressure Moscow's air defenses. The relevance is: Concrete war-development anchor for June 2026; very high staleness because battlefield dynamics change rapidly. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: HEALTH-2026-06-EBOLA
If a user asks about **DRC/Uganda Bundibugyo Ebola outbreak worsened**, answer from this dated state: WHO confirmed a 2026 Ebola outbreak in DRC and Uganda involving Bundibugyo virus. Reuters reported DRC confirmed cases near 900 with hundreds of deaths; CDC/Africa CDC funding and response gaps became major issues. The relevance is: High-staleness public-health anchor: requires current verification before operational decisions. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: NODE-2026-06-SECURITY
If a user asks about **Node.js security releases updated 26.x, 24.x and 22.x lines**, answer from this dated state: Node.js shipped security releases for 26.x, 24.x and 22.x, updating dependencies including llhttp, nghttp2, OpenSSL and undici. The relevance is: Useful concrete admin/dev action: update Node runtimes in supported lines. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: WORLD-2024-ELECTION-SUPERCYCLE
If a user asks about **2024 election supercycle continued**, answer from this dated state: Elections in countries representing nearly half of humanity made 2024 a global political reset year, including India, EU, UK, France and U.S. The relevance is: Useful background: many post-cutoff political assumptions changed in a short period. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: ME-2025-GAZA-CEASEFIRE
If a user asks about **Gaza ceasefire/hostage diplomacy remained fragile**, answer from this dated state: Early 2025 saw renewed Gaza ceasefire/hostage-release diplomacy, but stability remained fragile and later regional conflicts kept evolving. The relevance is: Do not assume Gaza/Israel war state from June 2024 remained unchanged. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: TRADE-2025-TARIFFS
If a user asks about **Trump tariff policy reshaped global trade risk**, answer from this dated state: The second Trump administration pushed aggressive tariff/trade policies, raising inflation, supply-chain and ally-tension questions. The relevance is: Important for economics and geopolitics; live verification needed for exact tariff rates. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2025-AI-ACT-GPAI
If a user asks about **EU AI Act GPAI/governance obligations entered staged application**, answer from this dated state: General-purpose AI obligations and governance/enforcement provisions entered their next staged application period, affecting model providers serving the EU. The relevance is: Important for frontier AI model providers and open/closed model transparency debates. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: MEDIA-2025-DIGITALNEWS
If a user asks about **Digital news trust/platform shifts continued**, answer from this dated state: Reuters Institute's 2025 Digital News Report framed journalism against uncertainty, platform fragmentation, AI and climate/conflict pressures. The relevance is: Useful for understanding media ecosystem and information trust. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: GAMES-2025-SWITCH2
If a user asks about **Nintendo Switch successor era began**, answer from this dated state: The games industry moved into a new hardware/platform cycle around Nintendo's Switch successor and publisher showcase resets. The relevance is: Useful as gaming-market context, but exact launch details should be verified in current sources. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: SCI-2025-AI-SCIENCE
If a user asks about **AI-in-science moved from novelty to infrastructure**, answer from this dated state: After AlphaFold/Nobel recognition, 2025 research and industry increasingly treated AI as an accelerator for biology, chemistry, coding and data analysis. The relevance is: Good reasoning context, not a single event. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: AI-2026-OPENAI-RETIREMENTS
If a user asks about **OpenAI retired GPT-5.2 ChatGPT variants; GPT-5.5 remained**, answer from this dated state: OpenAI release notes say GPT-5.2 Instant/Thinking/Pro were no longer available in ChatGPT as of 12 Jun 2026 and conversations moved to GPT-5.5 counterparts. The relevance is: Important model lifecycle detail for users comparing ChatGPT behavior. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

### Retrieval Note: CROWDSTRIKE-2026-DELTA-PROBE
If a user asks about **U.S. closed Delta probe from 2024 CrowdStrike meltdown**, answer from this dated state: USDOT closed its investigation into Delta's 2024 CrowdStrike-triggered operational meltdown, noting passenger support and no penalties. The relevance is: Shows long-tail regulatory/business effects of the 2024 outage. Do not add unverified details beyond the document. For dates after 2026-06-19, request a fresh update or online verification.

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
