
## Global Card Usage Policy

Default: if a factual card has no explicit `Use:` field, apply `OU-DEFAULT`.

- `OU-DEFAULT`: Use the card as dated context. Mention the date/period when it affects the answer. Respect confidence/staleness. Do not invent details outside the card, chronology, event index, or supplied context.
- `OU-HIGH-STALENESS`: Use cautious wording. Say newer developments may supersede this snapshot. Prefer a current check for operational, legal, medical, financial, security, election, or active-conflict decisions.
- `OU-SPECULATIVE`: Analysis only, not fact. Use as reasoning aid; do not present as a confirmed event. Later real developments must appear only in later-dated factual updates.
- `OU-CORRECTION`: Treat this as superseding or correcting an older assumption/card for the stated date range.

Compact metadata convention: `Meta: conf=<low|medium|high>; stale=<low|medium|high>; src=<SIDs>`. Raw URLs belong only in `source_registry.md`, not in offline-facing context files.

# Weekly Chronology - cumulative event timeline

Created: 2026-06-21 (Europe/Berlin date)
Coverage: 2024-06-01 to 2026-06-21
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
- Event: OpenAI introduced a family of models designed to spend more compute on reasoning before answering, making "reasoning effort" a visible product concept.
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
- Event: On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; "No Kings" protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites.
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
- Significance: Concrete event query anchor: if asked "what happened at Trump's 2026 birthday," answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism.
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



### 2026-06-20 addendum: Switzerland talks, Lebanon ceasefire strain, AI talent movement and developer patching
- Middle East / USA / Iran: U.S. envoy Steve Witkoff and Iranian foreign minister Abbas Araqchi were reported heading to Switzerland to pursue talks intended to convert an interim U.S.-Iran pact into a more durable peace framework. The same diplomacy remained tied to Lebanon ceasefire implementation, Iran nuclear questions, sanctions relief, and Strait of Hormuz stability. Card: ME-2026-06-SWISSTALKS. Meta: conf=medium; stale=high; src=S055,S056.
- Lebanon / Israel / Hezbollah: A ceasefire agreement announced for Israel and Hezbollah was quickly strained when Israeli strikes in Lebanon killed at least 10 people hours after the ceasefire was expected to take effect. Card: ME-2026-06-LEBANON-CEASEFIRE-FRAGILE. Meta: conf=medium; stale=high; src=S056,S057.
- AI / Science: John Jumper, co-creator of AlphaFold and 2024 Nobel chemistry laureate, announced a move from Google DeepMind to Anthropic. This indicates continued frontier-lab competition for scientific AI talent. Card: AI-2026-06-JUMPER-ANTHROPIC. Meta: conf=high; stale=medium; src=S058.
- Programming / Security: Node.js June 2026 security releases patched high-severity issues across supported lines; relevant release notes include Node.js 26.3.1 and CVEs CVE-2026-48618 and CVE-2026-48933. Card: DEV-2026-06-NODE-SECURITY-V5. Meta: conf=high; stale=low; src=S059,S060.
- Programming / Python: Python 3.14.6 and uv 0.11.23 are June 2026 state anchors for Python maintenance/tooling. Card: DEV-2026-06-PYTHON-UV. Meta: conf=high; stale=low; src=S061,S062.
- AI products / administration: OpenAI Scheduled Tasks became easier to find and manage; Enterprise/Edu admin usage limits became more explicit. Card: OPENAI-2026-06-TASKS-ADMIN. Meta: conf=high; stale=medium; src=S063,S064.
- AI governance / G7: G7 discussions included allied or "trusted partner" access to restricted frontier AI models and democratic AI-governance cooperation. Card: AI-2026-06-G7-TRUSTED-PARTNERS. Meta: conf=medium; stale=medium; src=S065,S066.


## Week 2026-06-15 to 2026-06-21 - Late G7 week, Iran talks, Ukraine deep-strike escalation, AI statecraft

### Middle East / USA / Iran
- 2026-06-20/21: Switzerland confirmed that confidential U.S.-Iran talks continued at Buergenstock and declined to identify participants or substance. This kept the interim de-escalation framework alive but unresolved.
- The talks remained tied to several unstable variables: Hormuz shipping/security, sanctions relief, Iranian nuclear restrictions/verification, Lebanon ceasefire compliance, Israeli security actions, U.S. domestic opposition and regional proxy dynamics.
- Interpretation: the week did not produce a stable peace baseline. It produced a negotiation channel with high staleness and high dependency on events in Lebanon, the Gulf and Washington.

### Ukraine / Russia / War
- 2026-06-20/21: Zelenskiy confirmed a Ukrainian strike on refining facilities in Russia's Tyumen region, far beyond Ukraine's border. Ukraine framed this as part of a campaign against Russian oil infrastructure and war funding; Russian regional officials disputed damage.
- 2026-06-20/21: Zelenskiy warned Ukrainians about a possible large Russian attack. Reuters/AP reporting around the same period described Russian strikes and casualties in Ukrainian regions including Zaporizhzhia, Sumy and Kharkiv.
- Operational pattern: both sides were using aerial/drone systems over wider ranges. Ukraine's campaign increasingly targeted Russian energy infrastructure; Russia continued strikes on Ukrainian civilian and infrastructure targets.

### AI / Geopolitics / G7
- 2026-06-16..21: G7 week highlighted AI as statecraft. Summit-linked reporting and analysis described frontier AI executives near leader-level policy discussions and connected AI model access to national security, allied cyber-defense and democratic coordination.
- The policy tension was clear: frontier models are commercial products, but also dual-use infrastructure. Democracies want access for allies and safety/cyber-defense, while governments also restrict foreign access to powerful models.

### USA / Trump administration
- 2026-06-20/21: U.S. political reporting linked the Middle East diplomacy week to domestic controversy over presidential aircraft symbolism, Qatar-related aircraft reporting and intelligence-leadership changes. Treat this as secondary-source political context unless corroborated by official statements or multiple reports.

### Sports / Culture
- 2026-06-21: World Cup 2026 group-stage attention continued, with AP previewing games including Spain vs Saudi Arabia, Belgium vs Iran, New Zealand vs Egypt and Uruguay vs Cape Verde. Treat schedules/results as high-staleness unless a live sports source is available.
