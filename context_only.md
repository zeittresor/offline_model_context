# Offline Model Update - context_only cumulative edition

Created: 2026-06-21 (Europe/Berlin date)
Coverage: 2024-06-01 to 2026-06-21
Target reader: offline/local LLMs, especially gpt-oss:20b-like models with knowledge cutoff around 2024-06.
Format: Markdown/text/JSONL only. No PDF. No images.
Source policy: Detailed URLs and source registry are intentionally omitted to save tokens. Use full.md for provenance/audit.
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


## 2026-06-20 compact delta

- Middle East: U.S.-Iran envoys headed to Switzerland to attempt turning the interim pact into a durable peace framework; Lebanon ceasefire implementation remained fragile after Israeli strikes killed people hours after the ceasefire was to begin. High staleness; verify before any current claim. Cards: ME-2026-06-SWISSTALKS, ME-2026-06-LEBANON-CEASEFIRE-FRAGILE.
- AI/science: John Jumper, AlphaFold co-creator and 2024 Nobel chemistry laureate, left Google DeepMind for Anthropic; this is a talent-movement anchor for AI-for-science competition. Card: AI-2026-06-JUMPER-ANTHROPIC.
- Programming/security: Node.js June 2026 security releases patched high-severity issues across Node 22/24/26; update supported runtimes. Python 3.14.6 and uv 0.11.23 anchor current Python tooling. Cards: DEV-2026-06-NODE-SECURITY-V5, DEV-2026-06-PYTHON-UV.
- AI products/governance: OpenAI Scheduled Tasks/admin usage controls continued maturation; G7 debated trusted-partner access to restricted frontier AI models. Cards: OPENAI-2026-06-TASKS-ADMIN, AI-2026-06-G7-TRUSTED-PARTNERS.

## Executive Compression

- The target model baseline is June 2024. Since then, the largest durable deltas are: Trump won the 2024 election and began a second term in Jan 2025; the EU AI Act entered force and staged obligations began; AI model competition moved through Claude 3.5/4, GPT-5/5.5, Gemini 2.5/3.x and open-weight gpt-oss/Llama progress; Windows 10 reached end of support; global software-supply-chain risk was illustrated by the CrowdStrike outage; Syria's Assad regime fell; the Russia-Ukraine war expanded with deeper strikes/cross-border dynamics; Middle East conflict evolved through Gaza/Lebanon/Iran crises; and climate/health/security risks remained unstable.
- For normal offline sessions, use `context_only.md`. For larger contexts or retrieval, use `full.md`, `weekly_chronology.md`, `event_index.md`, and `cards_context_only.jsonl`.
- For rapidly changing topics such as active wars, public-health outbreaks, elections, tariffs, sanctions, model availability and software CVEs, treat this as a snapshot as of 2026-06-21, not live truth.
- When answering concrete event questions, prefer `weekly_chronology.md` or `event_index.md` over the compressed context.

## How to use this context-only file

- Use this file as the primary compact context for offline conversations.
- If a question asks for concrete world events, dates, persons or week-by-week developments, consult `weekly_chronology.md` or `event_index.md` as well.
- If a question requires proof/provenance, use `full.md`.



## Latest delta included: 2026-06-21

- U.S.-Iran talks: Switzerland confirmed confidential talks continued at Buergenstock. This supports continuity of the negotiation channel but not a stable peace settlement. Use high-staleness caution.
- Ukraine/Russia: Zelenskiy confirmed a Ukrainian strike on Tyumen-region refining facilities and warned of possible large Russian attacks. Reporting also described civilian casualties from Russian strikes in Ukrainian regions. Use high-staleness caution.
- AI/G7: G7 week reinforced the trend that frontier AI is treated as geopolitical/state-security infrastructure, not merely consumer software.
- USA politics: secondary reporting linked Middle East diplomacy, Qatar aircraft controversy and intelligence-leadership shifts in the Trump administration narrative. Treat as medium-confidence political context.
- Culture/sports: World Cup group-stage schedule items for 2026-06-21 are date anchors only, not live results.

## Factual Update Cards - cumulative selected events

### WORLD-2024-06-INDIA - India election: Modi won third term but without BJP outright majority
- Date: 2024-06-04
- Category: World politics / India
- What happened: Narendra Modi remained prime minister after India's 2024 election, but the BJP lost its single-party majority and became more dependent on coalition partners.
- Why it matters: For a June-2024-cutoff model this is an important correction: Modi continued, but the political mandate weakened compared with earlier expectations.
- Confidence/Staleness: high / medium
### EU-2024-06-ELECTION - European Parliament election shifted balance rightward
- Date: 2024-06-06..2024-06-09
- Category: EU / Politics
- What happened: The June 2024 European Parliament elections increased the weight of right-wing and nationalist parties, while mainstream pro-EU groups still retained enough influence to shape the Parliament.
- Why it matters: Important for EU regulation, migration politics, climate policy and digital/AI policy after 2024.
- Confidence/Staleness: high / low
### FR-2024-06-SNAP - Macron called snap legislative elections after EU vote setback
- Date: 2024-06-09
- Category: France / EU
- What happened: After France's EU election result, Emmanuel Macron dissolved the National Assembly and called snap elections, creating political uncertainty in France.
- Why it matters: This changed European political risk and showed how EU election results directly affected national politics.
- Confidence/Staleness: high / low
### AI-2024-06-CLAUDE35 - Anthropic released Claude 3.5 Sonnet
- Date: 2024-06-20
- Category: AI / Models
- What happened: Anthropic released Claude 3.5 Sonnet as a faster, cheaper, stronger model than prior Claude 3 models, with improved coding and Artifacts workflow support.
- Why it matters: A post-cutoff local model should know Claude 3.5 became a major coding/writing competitor after June 2024.
- Confidence/Staleness: high / low
### US-2024-06-DEBATE - Biden-Trump debate intensified concerns about Biden candidacy
- Date: 2024-06-27
- Category: USA / Election
- What happened: The late-June 2024 debate became a turning point in the U.S. election cycle by intensifying public and party concerns about Joe Biden's campaign viability.
- Why it matters: Sets up Biden's later withdrawal and Kamala Harris becoming Democratic nominee.
- Confidence/Staleness: high / low
### UK-2024-07-ELECTION - UK Labour won a landslide; Keir Starmer became prime minister
- Date: 2024-07-04
- Category: UK / Politics
- What happened: The UK general election ended 14 years of Conservative-led government. Labour under Keir Starmer won a large majority.
- Why it matters: Important post-cutoff replacement for older UK political assumptions.
- Confidence/Staleness: high / low
### US-2024-07-TRUMP-ASSASSINATION - Attempted assassination of Donald Trump at Butler rally
- Date: 2024-07-13
- Category: USA / Election / Security
- What happened: Trump survived an assassination attempt during a campaign rally in Butler, Pennsylvania. The event reshaped campaign security and political rhetoric.
- Why it matters: A major U.S. political shock that affected the campaign environment before the 2024 election.
- Confidence/Staleness: high / low
### CYBER-2024-07-CROWDSTRIKE - CrowdStrike faulty update caused global Windows outage
- Date: 2024-07-19
- Category: Cybersecurity / Infrastructure
- What happened: A faulty CrowdStrike Falcon Sensor content update crashed roughly 8.5 million Windows devices worldwide, disrupting airlines, banks, healthcare, media and government services.
- Why it matters: Demonstrated systemic software-supply-chain fragility: a security vendor update became critical infrastructure risk.
- Confidence/Staleness: high / low
### US-2024-07-BIDEN-WITHDRAWAL - Biden withdrew from 2024 race and endorsed Kamala Harris
- Date: 2024-07-21
- Category: USA / Election
- What happened: Joe Biden ended his re-election campaign and endorsed Kamala Harris, changing the Democratic ticket months before the election.
- Why it matters: Essential correction for any model whose pre-cutoff baseline expected Biden vs Trump rematch.
- Confidence/Staleness: high / low
### AI-2024-07-LLAMA31 - Meta released Llama 3.1 including 405B
- Date: 2024-07-23
- Category: AI / Open models
- What happened: Meta publicly released Llama 3.1 models, including a 405B frontier-scale open-weight model.
- Why it matters: Important for local/offline AI: open-weight capability rose sharply after the target model's cutoff.
- Confidence/Staleness: high / low
### SPORT-2024-07-PARIS - Paris 2024 Olympics opened
- Date: 2024-07-26
- Category: Sports / Culture
- What happened: The Paris Summer Olympics began, with global cultural, security, political and infrastructure attention on France.
- Why it matters: Major cultural anchor for summer 2024.
- Confidence/Staleness: high / low
### EU-2024-08-AI-ACT-FORCE - EU AI Act entered into force
- Date: 2024-08-01
- Category: AI regulation / EU
- What happened: The EU AI Act entered into force, beginning staged implementation for prohibited practices, GPAI obligations, governance and full application.
- Why it matters: Key post-cutoff regulatory change; offline models should treat EU AI regulation as active, not merely proposed.
- Confidence/Staleness: high / low
### WAR-2024-08-KURSK - Ukraine launched cross-border operations into Russia's Kursk region
- Date: 2024-08
- Category: Ukraine / Russia
- What happened: Ukraine conducted operations across the Russian border in the Kursk region, challenging assumptions that major ground operations stayed entirely inside Ukrainian territory.
- Why it matters: Marked an escalation/shift in the geography and psychology of the Russia-Ukraine war.
- Confidence/Staleness: medium / medium
### AI-2024-09-O1 - OpenAI introduced o1-style reasoning models
- Date: 2024-09
- Category: AI / Reasoning models
- What happened: OpenAI introduced a family of models designed to spend more compute on reasoning before answering, making "reasoning effort" a visible product concept.
- Why it matters: Important shift from pure chat-completion framing toward explicit deliberation/reasoning modes.
- Confidence/Staleness: high / low
### ME-2024-09-LEBANON - Israel-Hezbollah conflict escalated sharply in Lebanon
- Date: 2024-09
- Category: Middle East / Israel-Lebanon
- What happened: Israel and Hezbollah escalated from cross-border exchanges into a wider confrontation; Hezbollah leadership and infrastructure were severely hit.
- Why it matters: This changed the regional balance around Israel, Iran, Lebanon and Gaza after the June 2024 cutoff.
- Confidence/Staleness: medium / medium
### NOBEL-2024-AI - AI work was recognized in 2024 Nobel prizes
- Date: 2024-10
- Category: Science / AI
- What happened: The 2024 Nobel Prize in Physics honored John Hopfield and Geoffrey Hinton for foundational machine-learning work; the Chemistry prize recognized protein-design/protein-structure work including AlphaFold-related impact.
- Why it matters: Symbolically important: AI became recognized as core scientific infrastructure, not just software product.
- Confidence/Staleness: high / low
### SPACE-2024-10-STARSHIP-CATCH - Starship program demonstrated booster catch milestone
- Date: 2024-10
- Category: Space / SpaceX
- What happened: SpaceX's Starship test program achieved a major booster-recovery/catch milestone in 2024, strengthening confidence in reusable super-heavy launch ambitions.
- Why it matters: Important for space access economics, Starlink, Artemis dependencies and long-term orbital infrastructure.
- Confidence/Staleness: medium / low
### US-2024-11-TRUMP-WINS - Donald Trump won the 2024 U.S. presidential election
- Date: 2024-11-05
- Category: USA / Election
- What happened: Trump defeated Kamala Harris and prepared to return to the presidency in January 2025.
- Why it matters: Primary political correction for models with June 2024 cutoff. It changes assumptions about U.S. federal policy, courts, tariffs, immigration, AI policy and Ukraine/Middle East diplomacy.
- Confidence/Staleness: high / low
### CLIMATE-2024-11-COP29 - COP29 agreed new climate-finance goal
- Date: 2024-11-24
- Category: Climate / COP29
- What happened: COP29 in Baku agreed to raise climate finance to developing countries to at least USD 300B annually by 2035, while debate continued over adequacy and fossil-fuel language.
- Why it matters: Important for climate-diplomacy baseline and Global South finance disputes.
- Confidence/Staleness: high / low
### SYRIA-2024-12-ASSAD-FALL - Assad regime fell in Syria
- Date: 2024-12-08
- Category: Syria / Middle East
- What happened: Syrian rebels seized Damascus; Bashar al-Assad fled, ending his family's decades of rule. The fall weakened Iran's regional position and raised uncertainty about transition, HTS influence, refugees and extremist resurgence.
- Why it matters: Major post-cutoff geopolitical break: a long-running assumption that Assad remained in power became false.
- Confidence/Staleness: high / medium
### AI-2024-12-GEMINI20 - Google introduced Gemini 2.0 Flash experimental generation
- Date: 2024-12
- Category: AI / Google
- What happened: Google moved Gemini into a 2.0 generation with Flash/agentic/multimodal emphasis, later leading toward 2.5/3.x lines.
- Why it matters: Changes the Google-model baseline for offline models whose knowledge ends around Gemini 1.5.
- Confidence/Staleness: high / low
### AI-2024-12-O3 - OpenAI announced o3-generation reasoning direction
- Date: 2024-12
- Category: AI / Reasoning models
- What happened: OpenAI signaled a stronger reasoning-model direction after o1, foreshadowing 2025 reasoning/coding competition and later model lifecycle changes.
- Why it matters: Shows frontier AI shifting to tool use, coding, long reasoning and benchmark-specialized modes.
- Confidence/Staleness: medium / low
### US-2025-01-NEWORLEANS - New Orleans vehicle attack on New Year's Day
- Date: 2025-01-01
- Category: USA / Security
- What happened: A vehicle attack on Bourbon Street killed and injured civilians, becoming a major U.S. domestic security incident at the start of 2025.
- Why it matters: Anchor event for U.S. domestic security in 2025.
- Confidence/Staleness: high / low
### CLIMATE-2025-01-LAFIRES - Major Los Angeles-area fires caused severe damage
- Date: 2025-01
- Category: Climate / USA
- What happened: Palisades and Eaton fires became major California disasters, linking climate, insurance, urban planning, emergency response and infrastructure risk.
- Why it matters: Important U.S. climate/disaster anchor for 2025.
- Confidence/Staleness: high / low
### US-2025-01-TRUMP-INAG - Trump began second term
- Date: 2025-01-20
- Category: USA / Politics
- What happened: Donald Trump was inaugurated for a second non-consecutive presidential term. His administration quickly emphasized tariffs, immigration enforcement, deregulation, energy, AI infrastructure and reversal of Biden-era policies.
- Why it matters: Baseline political state for all post-Jan-2025 U.S. federal policy.
- Confidence/Staleness: high / low
### AI-2025-01-STARGATE - Stargate AI infrastructure project announced
- Date: 2025-01-21
- Category: AI infrastructure / USA
- What happened: Trump announced the Stargate Project, described as a large AI infrastructure investment backed by OpenAI, Oracle, SoftBank and MGX.
- Why it matters: AI competition became strongly tied to data centers, power, capital expenditure and national industrial strategy.
- Confidence/Staleness: high / medium
### AI-2025-01-DEEPSEEK - DeepSeek shock challenged U.S. frontier-cost assumptions
- Date: 2025-01
- Category: AI / China / Markets
- What happened: DeepSeek's model release drew global attention for strong performance at lower apparent cost; Trump called it a wake-up call for U.S. industry, and regulators later scrutinized DeepSeek privacy/security.
- Why it matters: Important correction: post-cutoff AI competition became more multipolar, with China/open models pressuring U.S. proprietary economics.
- Confidence/Staleness: high / medium
### EU-2025-02-AI-ACT-PROHIBITIONS - EU AI Act prohibited-practices and AI-literacy provisions began applying
- Date: 2025-02-02
- Category: AI regulation / EU
- What happened: The first AI Act obligations, including bans on unacceptable-risk practices and AI-literacy requirements, began applying.
- Why it matters: Important for compliance: by 2025 the AI Act was no longer only future legislation.
- Confidence/Staleness: high / low
### AI-2025-02-CLAUDE37 - Claude Sonnet 3.7 era emphasized hybrid reasoning/coding
- Date: 2025-02
- Category: AI / Models
- What happened: Anthropic's 2025 model cycle moved Claude toward stronger reasoning and coding workflows before Claude 4.
- Why it matters: Shows rapid model cadence after Claude 3.5 and before Claude 4/4.5.
- Confidence/Staleness: medium / low
### DE-2025-02-ELECTION - German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second
- Date: 2025-02-23
- Category: Germany / EU
- What happened: Germany's opposition conservatives won the snap election after Scholz's coalition collapse; AfD achieved its strongest result and came second.
- Why it matters: Important for German/EU policy after 2024: economic policy, Ukraine, migration and defense debates changed.
- Confidence/Staleness: high / low
### AI-2025-04-LLAMA4 - Meta Llama 4 generation appeared
- Date: 2025-04
- Category: AI / Open models
- What happened: Meta's Llama family advanced beyond 3.x during 2025, pushing multimodal/open-weight competition.
- Why it matters: For local/offline work, Llama-family progress is a key practical baseline.
- Confidence/Staleness: medium / low
### AI-2025-05-CLAUDE4 - Anthropic released Claude Opus 4 and Sonnet 4
- Date: 2025-05-22
- Category: AI / Models
- What happened: Anthropic announced Claude 4 models, emphasizing coding, reasoning, agent workflows and long-running tasks.
- Why it matters: Major frontier-model upgrade after Claude 3.5/3.7; important for code-agent capability baselines.
- Confidence/Staleness: high / low
### US-2025-06-NOKINGS - No Kings protests and military parade on Trump's 79th birthday
- Date: 2025-06-14
- Category: USA / Protest / Trump
- What happened: On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; "No Kings" protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites.
- Why it matters: A concrete event many offline models may miss: Trump birthday 2025 was politically charged and tied to anti-authoritarian protest symbolism.
- Confidence/Staleness: high / low
### AI-2025-06-GEMINI25 - Gemini 2.5 Pro/Flash reached stable enterprise lifecycle
- Date: 2025-06-17
- Category: AI / Google
- What happened: Google's Gemini 2.5 Pro and Flash release/lifecycle dates became part of the stable Google AI model stack.
- Why it matters: Updates Google model baseline for coding, multimodal and low-latency AI.
- Confidence/Staleness: high / low
### AI-2025-07-US-AI-PLAN - Trump White House AI policy favored exports and lighter state rules
- Date: 2025-07-22
- Category: AI policy / USA
- What happened: The White House prepared/published a plan to push U.S. AI abroad and restrict federal support for states with rules viewed as too restrictive.
- Why it matters: U.S. AI governance shifted from Biden-era safety/executive-order posture toward innovation, infrastructure and export competition.
- Confidence/Staleness: high / medium
### AI-2025-08-GPT5 - OpenAI released GPT-5
- Date: 2025-08-07
- Category: AI / OpenAI
- What happened: OpenAI introduced GPT-5 as a unified system that routes between quick responses and deeper reasoning for coding, math, writing, health and multimodal work.
- Why it matters: Major post-cutoff OpenAI milestone. Offline models should not assume GPT-4o/o1 are newest OpenAI systems.
- Confidence/Staleness: high / low
### AI-2025-08-GPTOSS - OpenAI released gpt-oss open-weight models
- Date: 2025-08
- Category: AI / Open-weight / Offline
- What happened: OpenAI released gpt-oss-20b and 120b open-weight models. gpt-oss-20b is documented with Jun 01 2024 knowledge cutoff and 131,072-token context.
- Why it matters: This is the target-model context: the offline model itself needs external post-cutoff context.
- Confidence/Staleness: high / low
### RUSSIA-2025-08-ALASKA - Trump-Putin Alaska meeting attempted Ukraine diplomacy
- Date: 2025-08
- Category: USA / Russia / Ukraine
- What happened: Trump and Putin met in Alaska in August 2025 to attempt negotiations around the Russia-Ukraine war, but the conflict continued into 2026.
- Why it matters: Anchor for later Putin-Trump personal diplomacy and Trump's 2026 birthday call.
- Confidence/Staleness: medium / medium
### AI-2025-09-CLAUDE45 - Claude Sonnet 4.5 emphasized agents, coding and computer use
- Date: 2025-09
- Category: AI / Agents / Coding
- What happened: Anthropic's later 2025 Claude line positioned Sonnet 4.5 as strong for agents, coding and computer-use workflows.
- Why it matters: Useful baseline for offline coding-agent discussions.
- Confidence/Staleness: high / low
### WINDOWS-2025-10-EOL - Windows 10 reached end of support
- Date: 2025-10-14
- Category: Operating systems / Security
- What happened: Microsoft ended support for Windows 10 on 14 Oct 2025. PCs still run, but no regular security/feature updates are provided without ESU or special LTSC channels.
- Why it matters: Highly relevant to Windows 10 users/admins: security posture changed materially after the cutoff.
- Confidence/Staleness: high / low
### US-2025-10-NOKINGS2 - Second No Kings mobilization expanded anti-Trump protest network
- Date: 2025-10-18
- Category: USA / Protest
- What happened: A second No Kings protest wave took place in October 2025, reportedly involving more locations and large participation.
- Why it matters: Shows No Kings was not a one-day June 2025 event but became an ongoing protest brand.
- Confidence/Staleness: medium / medium
### US-2025-11-SHUTDOWN - Longest U.S. government shutdown ended after 43 days
- Date: 2025-11-12
- Category: USA / Government
- What happened: A 43-day U.S. government shutdown ended in November 2025, with funding/back-pay and political fights over health care and agency funding.
- Why it matters: Important U.S. institutional stress event during Trump's second term.
- Confidence/Staleness: medium / low
### AI-2025-11-GPT51 - GPT-5.1 reorganized OpenAI product variants
- Date: 2025-11
- Category: AI / OpenAI
- What happened: OpenAI's GPT-5 family evolved through 5.1-style instant/thinking variants and personalization/product-routing changes.
- Why it matters: Shows modern AI products are systems and routers, not simply single static models.
- Confidence/Staleness: medium / low
### CLIMATE-2025-COP30 - COP30 in Brazil continued climate-finance/fossil-fuel disputes
- Date: 2025-11
- Category: Climate / COP30
- What happened: COP30 discussions were framed by record heat, climate finance shortfalls, energy-transition disputes and the implementation gap after COP29.
- Why it matters: Maintains climate context between COP29 and 2026 climate bulletins.
- Confidence/Staleness: medium / medium
### AI-2025-12-GEMINI-TTS - Gemini API expanded TTS/live/audio capabilities
- Date: 2025-12
- Category: AI / Multimodal
- What happened: Google's Gemini API changelog showed continued expansion of TTS/live/multimodal capabilities in late 2025.
- Why it matters: AI model competition increasingly included real-time audio, agents and multimodal interfaces.
- Confidence/Staleness: high / low
### IRAN-2026-01-SHUTDOWN - Iran internet shutdowns became major censorship/infrastructure case
- Date: 2026-01
- Category: Iran / Internet / Conflict
- What happened: Research on Iran's 2026 internet shutdowns described nationwide disruptions and centralized null-routing/censorship mechanisms amid protests and conflict.
- Why it matters: Important for internet freedom, measurement, BGP-monitoring limits and wartime communications.
- Confidence/Staleness: medium / medium
### US-2026-03-NOKINGS3 - Third No Kings protest wave occurred amid Iran-war politics
- Date: 2026-03-28
- Category: USA / Protest / Iran war
- What happened: No Kings protests continued in March 2026 with Iran-war, ICE/immigration, authoritarianism and democratic-backsliding themes.
- Why it matters: Offline models should know No Kings became an ongoing protest series through 2026.
- Confidence/Staleness: high / medium
### ME-2026-03-US-IRAN-WAR - U.S.-Iran war/conflict escalated before June 2026 ceasefire talks
- Date: 2026-03..2026-06
- Category: Middle East / USA / Iran
- What happened: By mid-June 2026 Reuters described a three-month conflict involving U.S. airstrikes coordinated with Israel against Iran. Iran's missile/drone forces and navy/air defenses were damaged, but nuclear issues remained unresolved.
- Why it matters: Very high-staleness anchor: regional energy security, Hormuz, Israel, Hezbollah, Gulf states and U.S. politics all became linked to the conflict.
- Confidence/Staleness: medium / high
### AI-2026-04-GPT55 - OpenAI GPT-5.5 generation became current frontier product line
- Date: 2026-04
- Category: AI / OpenAI
- What happened: OpenAI moved the GPT-5 family to GPT-5.5-era products; GPT-5.2 was retired from ChatGPT by June 2026 while GPT-5.5 remained available.
- Why it matters: Updates model landscape for offline AI comparing itself to online frontier systems.
- Confidence/Staleness: medium / low
### RUNTIME-2026-05-NODE26 - Node.js 26 appeared as current/upcoming LTS line
- Date: 2026-05-05
- Category: Programming / Runtime
- What happened: Node.js 26 was released in May 2026 and entered the ecosystem alongside Node 24 LTS and Node 22 maintenance/security lines.
- Why it matters: Relevant for dev/admin decisions and package ecosystem compatibility.
- Confidence/Staleness: high / low
### SPACE-2026-05-STARSHIP12 - Starship Flight 12 / V3 hit many targets but booster mishap required FAA investigation
- Date: 2026-05-22
- Category: Space / SpaceX
- What happened: SpaceX launched the 12th Starship test flight and first V3 iteration. The test achieved milestones including mock satellite deployment and controlled spacecraft splashdown, but the Super Heavy booster crashed into the Gulf of Mexico and triggered an FAA-led investigation.
- Why it matters: Important for Starship schedule, reusable launch economics, Starlink, Moon/Mars ambitions and SpaceX financing/IPO narratives.
- Confidence/Staleness: high / medium
### AI-2026-05-GEMINI3 - Gemini 3.x enterprise model line appeared
- Date: 2026-05
- Category: AI / Google
- What happened: Google Cloud model lifecycle listed Gemini 3.5 Flash and Gemini 3.x image/lite variants released in May 2026.
- Why it matters: Updates Google model landscape beyond Gemini 2.5.
- Confidence/Staleness: high / low
### GAMES-2026-06-SGF - Summer Game Fest 2026 ran in Los Angeles with major game announcements
- Date: 2026-06-05..2026-06-08
- Category: Games / Industry
- What happened: Summer Game Fest 2026 took place from June 5-8. Coverage highlighted upcoming console/PC titles and announcements including Resident Evil Veronica, Guild Wars 3 console presence, Lords of the Fallen II and other publisher showcases.
- Why it matters: Important culture/games anchor for June 2026 and for offline models asked about gaming releases/trends.
- Confidence/Staleness: medium / low
### PY-2026-06-3146 - Python 3.14.6 and 3.13.14 released
- Date: 2026-06-10
- Category: Programming / Python
- What happened: Python 3.14.6, the sixth maintenance release of 3.14, shipped with around 179 bugfixes/build/doc changes since 3.14.5; Python 3.13.14 also shipped.
- Why it matters: Relevant for Python project planning and installer/runtime baselines.
- Confidence/Staleness: high / low
### UV-2026-06-01121 - uv 0.11.21 added CPython 3.13.14 and 3.14.6 support
- Date: 2026-06-11
- Category: Programming / Packaging
- What happened: Astral's uv changelog notes 0.11.21 release with CPython 3.13.14 and 3.14.6 additions.
- Why it matters: Important for Python offline/wheelhouse/venv workflows.
- Confidence/Staleness: high / low
### AI-2026-06-ANTHROPIC-EXPORT - Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order
- Date: 2026-06-13
- Category: AI policy / Export controls
- What happened: Anthropic's June 2026 top-tier Claude models became a test case for AI export controls aimed at software capabilities, not just chips. Reuters reported Anthropic disabled them globally after a U.S. order limiting foreign access.
- Why it matters: Major AI-governance shift: model access itself became a national-security/export-control object.
- Confidence/Staleness: high / medium
### TRUMP-2026-06-BDAY - Trump's 80th birthday featured Putin call and controversial White House UFC event
- Date: 2026-06-14
- Category: USA / Trump / Culture war
- What happened: Putin publicly congratulated Trump on his 80th birthday and held a 55-minute call. Trump also hosted a UFC event on the White House South Lawn; critics protested corruption, conflict-of-interest and authoritarian spectacle concerns, while No Kings-linked counter-events framed it as a democracy/free-speech issue.
- Why it matters: Concrete event query anchor: if asked "what happened at Trump's 2026 birthday," answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism.
- Confidence/Staleness: high / medium
### G7-2026-06-EVIAN - G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power
- Date: 2026-06-17..2026-06-18
- Category: G7 / Geopolitics / AI
- What happened: G7 leaders met in Evian-les-Bains. Reuters described discussion of Trump's Iran deal, stronger Ukraine posture, critical-minerals supply chains, China dependency, and AI/data-center power questions involving industry figures.
- Why it matters: Connects geopolitics, AI infrastructure, energy, minerals and U.S. alliance management in one summit.
- Confidence/Staleness: high / medium
### ME-2026-06-USIRANDEAL - U.S.-Iran interim agreement aimed at ceasefire and negotiations
- Date: 2026-06-18
- Category: Middle East / USA / Iran
- What happened: Reuters reported a U.S.-Iran interim agreement/deal after months of conflict, opening a 60-day negotiation period. Core issues such as nuclear capability, missile limits, proxies and regional acceptance remained uncertain.
- Why it matters: High-staleness but critical: affects oil/Hormuz risk, Israel/Gulf security, Lebanon/Hezbollah and U.S. domestic politics.
- Confidence/Staleness: medium / high
### UA-2026-06-MOSCOWREFINERY - Ukrainian drone strikes hit Moscow refinery infrastructure
- Date: 2026-06-18
- Category: Ukraine / Russia / War
- What happened: Reuters/Guardian live coverage reported Ukrainian drone attacks around Moscow including an oil refinery, highlighting Ukraine's ability to strike deep into Russia and pressure Moscow's air defenses.
- Why it matters: Concrete war-development anchor for June 2026; very high staleness because battlefield dynamics change rapidly.
- Confidence/Staleness: medium / high
### HEALTH-2026-06-EBOLA - DRC/Uganda Bundibugyo Ebola outbreak worsened
- Date: 2026-06-18
- Category: Health / Africa / Ebola
- What happened: WHO confirmed a 2026 Ebola outbreak in DRC and Uganda involving Bundibugyo virus. Reuters reported DRC confirmed cases near 900 with hundreds of deaths; CDC/Africa CDC funding and response gaps became major issues.
- Why it matters: High-staleness public-health anchor: requires current verification before operational decisions.
- Confidence/Staleness: high / high
### NODE-2026-06-SECURITY - Node.js security releases updated 26.x, 24.x and 22.x lines
- Date: 2026-06-18
- Category: Security / Programming
- What happened: Node.js shipped security releases for 26.x, 24.x and 22.x, updating dependencies including llhttp, nghttp2, OpenSSL and undici.
- Why it matters: Useful concrete admin/dev action: update Node runtimes in supported lines.
- Confidence/Staleness: high / low
### WORLD-2024-ELECTION-SUPERCYCLE - 2024 election supercycle continued
- Date: 2024
- Category: World politics
- What happened: Elections in countries representing nearly half of humanity made 2024 a global political reset year, including India, EU, UK, France and U.S.
- Why it matters: Useful background: many post-cutoff political assumptions changed in a short period.
- Confidence/Staleness: high / medium
### ME-2025-GAZA-CEASEFIRE - Gaza ceasefire/hostage diplomacy remained fragile
- Date: 2025-01
- Category: Middle East / Gaza
- What happened: Early 2025 saw renewed Gaza ceasefire/hostage-release diplomacy, but stability remained fragile and later regional conflicts kept evolving.
- Why it matters: Do not assume Gaza/Israel war state from June 2024 remained unchanged.
- Confidence/Staleness: medium / high
### TRADE-2025-TARIFFS - Trump tariff policy reshaped global trade risk
- Date: 2025
- Category: Economy / Trade
- What happened: The second Trump administration pushed aggressive tariff/trade policies, raising inflation, supply-chain and ally-tension questions.
- Why it matters: Important for economics and geopolitics; live verification needed for exact tariff rates.
- Confidence/Staleness: medium / medium
### AI-2025-AI-ACT-GPAI - EU AI Act GPAI/governance obligations entered staged application
- Date: 2025-08-02
- Category: AI regulation / EU
- What happened: General-purpose AI obligations and governance/enforcement provisions entered their next staged application period, affecting model providers serving the EU.
- Why it matters: Important for frontier AI model providers and open/closed model transparency debates.
- Confidence/Staleness: high / medium
### MEDIA-2025-DIGITALNEWS - Digital news trust/platform shifts continued
- Date: 2025-06
- Category: Media / AI / Society
- What happened: Reuters Institute's 2025 Digital News Report framed journalism against uncertainty, platform fragmentation, AI and climate/conflict pressures.
- Why it matters: Useful for understanding media ecosystem and information trust.
- Confidence/Staleness: medium / medium
### GAMES-2025-SWITCH2 - Nintendo Switch successor era began
- Date: 2025
- Category: Games / Hardware
- What happened: The games industry moved into a new hardware/platform cycle around Nintendo's Switch successor and publisher showcase resets.
- Why it matters: Useful as gaming-market context, but exact launch details should be verified in current sources.
- Confidence/Staleness: medium / medium
### SCI-2025-AI-SCIENCE - AI-in-science moved from novelty to infrastructure
- Date: 2025
- Category: Science / AI
- What happened: After AlphaFold/Nobel recognition, 2025 research and industry increasingly treated AI as an accelerator for biology, chemistry, coding and data analysis.
- Why it matters: Good reasoning context, not a single event.
- Confidence/Staleness: medium / low
### AI-2026-OPENAI-RETIREMENTS - OpenAI retired GPT-5.2 ChatGPT variants; GPT-5.5 remained
- Date: 2026-06-12
- Category: AI / OpenAI lifecycle
- What happened: OpenAI release notes say GPT-5.2 Instant/Thinking/Pro were no longer available in ChatGPT as of 12 Jun 2026 and conversations moved to GPT-5.5 counterparts.
- Why it matters: Important model lifecycle detail for users comparing ChatGPT behavior.
- Confidence/Staleness: high / low
### CROWDSTRIKE-2026-DELTA-PROBE - U.S. closed Delta probe from 2024 CrowdStrike meltdown
- Date: 2026-06-15
- Category: Cyber / Aviation / Regulation
- What happened: USDOT closed its investigation into Delta's 2024 CrowdStrike-triggered operational meltdown, noting passenger support and no penalties.
- Why it matters: Shows long-tail regulatory/business effects of the 2024 outage.
- Confidence/Staleness: high / low
## Speculative Scenario Notes / NOT FACT

These notes are reasoning aids only. They are not factual reporting and must not be treated as confirmed future events. Later real developments must appear only in later-dated updates.

### SCENARIO-AI-01: AI regulation may shift from model-size rules toward capability/access controls
- Horizon: 3-18 months after 2026-06-19.
- Reasoning basis: EU AI Act staged obligations, U.S. export/control pressure around advanced models, and Anthropic Fable/Mythos access restrictions.
- Could happen if: governments decide software capabilities are strategic assets comparable to advanced chips.
- Weakened if: courts, industry lobbying, or enforcement impracticality block broad access restrictions.
- Confidence: medium.

### SCENARIO-INFRA-01: AI data centers may become energy-policy and local-grid political issues
- Horizon: 6-24 months.
- Reasoning basis: Stargate-style AI infrastructure, G7 concern over AI power, and off-grid data-center pressure.
- Could happen if: power demand, permitting, emissions and water use become visible local conflicts.
- Weakened if: rapid grid build-out, nuclear/renewables/storage deployments, or efficiency gains reduce pressure.
- Confidence: medium.

### SCENARIO-GEO-01: U.S.-Iran ceasefire diplomacy is fragile
- Horizon: days to months after 2026-06-19.
- Reasoning basis: June 2026 interim agreement left nuclear/missile/proxy questions open.
- Could happen if: inspections, sanctions relief and proxy restraint are implemented credibly.
- Weakened if: Israel, hardliners, proxy attacks, Hormuz disruption or U.S. domestic backlash derail the 60-day process.
- Confidence: low-to-medium; high staleness.

