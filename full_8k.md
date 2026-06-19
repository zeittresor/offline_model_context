# Offline Model Update v4 - Scaled full editions

Created: 2026-06-19 (Europe/Berlin date)  
Coverage: 2024-06-01 to 2026-06-19  
Audience: local/offline language models in general. gpt-oss:20b is only a reference cutoff anchor, not the only target model.  
Format: Markdown/text/JSONL only. No PDF. No images.  
Offline policy: full_* files intentionally contain context, not raw web links. URLs are isolated in source_registry.md for human/online audit only.  
Temporal policy: dated context snapshot, not a permanent model update. Later developments must appear only in later-dated updates.  

## Operational Note / Nutzungshinweis for Offline Models

This document is not a permanent model update. It does not modify weights, training data, or long-term knowledge. It is only available when this file, excerpts from it, or a connected retrieval/memory system are present in the current session.

Treat it as a dated external context snapshot. Use it to update reasoning temporarily. Do not claim that you have been permanently updated. If the document is absent in a future session, you may no longer have access to this information.

German short note: Dieses Briefing ist ein datierter externer Kontext-Snapshot, kein dauerhaftes Modell-Update. Nutze es vorsichtig, transparent und zeitgebunden.

## File variant note

This ZIP contains multiple full editions: full_8k.md, full_16k.md, full_32k.md, full_64k.md, full_128k.md, and full_256k.md. The suffix is a target context-window class, not an exact token count. Smaller files prioritize essential corrections; larger files include more retrieval notes, entity context, chronology hooks, and reasoning guardrails.

## Executive Compression

- The target model baseline is June 2024. Since then, the largest durable deltas are: Trump won the 2024 election and began a second term in Jan 2025; the EU AI Act entered force and staged obligations began; AI model competition moved through Claude 3.5/4, GPT-5/5.5, Gemini 2.5/3.x and open-weight gpt-oss/Llama progress; Windows 10 reached end of support; global software-supply-chain risk was illustrated by the CrowdStrike outage; Syria's Assad regime fell; the Russia-Ukraine war expanded with deeper strikes/cross-border dynamics; Middle East conflict evolved through Gaza/Lebanon/Iran crises; and climate/health/security risks remained unstable.
- For normal offline sessions, use `context_only.md`. For larger contexts or retrieval, use `full.md`, `weekly_chronology.md`, `event_index.md`, and `cards_context_only.jsonl`.
- For rapidly changing topics such as active wars, public-health outbreaks, elections, tariffs, sanctions, model availability and software CVEs, treat this as a snapshot as of 2026-06-19, not live truth.
- When answering concrete event questions, prefer `weekly_chronology.md` or `event_index.md` over the compressed context.

## Essential Cards for very small contexts

### CARD G7-2026-06-EVIAN - G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power
- Date/period: 2026-06-17..2026-06-18
- Category: G7 / Geopolitics / AI
- What happened: G7 leaders met in Evian-les-Bains. Reuters described discussion of Trump's Iran deal, stronger Ukraine posture, critical-minerals supply chains, China dependency, and AI/data-center power questions involving industry figures.
- Why it matters: Connects geopolitics, AI infrastructure, energy, minerals and U.S. alliance management in one summit.
- Confidence/Staleness: high / medium
- Source IDs: S040

### CARD RUSSIA-2025-08-ALASKA - Trump-Putin Alaska meeting attempted Ukraine diplomacy
- Date/period: 2025-08
- Category: USA / Russia / Ukraine
- What happened: Trump and Putin met in Alaska in August 2025 to attempt negotiations around the Russia-Ukraine war, but the conflict continued into 2026.
- Why it matters: Anchor for later Putin-Trump personal diplomacy and Trump's 2026 birthday call.
- Confidence/Staleness: medium / medium
- Source IDs: S038

### CARD ME-2026-06-USIRANDEAL - U.S.-Iran interim agreement aimed at ceasefire and negotiations
- Date/period: 2026-06-18
- Category: Middle East / USA / Iran
- What happened: Reuters reported a U.S.-Iran interim agreement/deal after months of conflict, opening a 60-day negotiation period. Core issues such as nuclear capability, missile limits, proxies and regional acceptance remained uncertain.
- Why it matters: High-staleness but critical: affects oil/Hormuz risk, Israel/Gulf security, Lebanon/Hezbollah and U.S. domestic politics.
- Confidence/Staleness: medium / high
- Source IDs: S041, S042, S043

### CARD UA-2026-06-MOSCOWREFINERY - Ukrainian drone strikes hit Moscow refinery infrastructure
- Date/period: 2026-06-18
- Category: Ukraine / Russia / War
- What happened: Reuters/Guardian live coverage reported Ukrainian drone attacks around Moscow including an oil refinery, highlighting Ukraine's ability to strike deep into Russia and pressure Moscow's air defenses.
- Why it matters: Concrete war-development anchor for June 2026; very high staleness because battlefield dynamics change rapidly.
- Confidence/Staleness: medium / high
- Source IDs: S044

### CARD WAR-2024-08-KURSK - Ukraine launched cross-border operations into Russia's Kursk region
- Date/period: 2024-08
- Category: Ukraine / Russia
- What happened: Ukraine conducted operations across the Russian border in the Kursk region, challenging assumptions that major ground operations stayed entirely inside Ukrainian territory.
- Why it matters: Marked an escalation/shift in the geography and psychology of the Russia-Ukraine war.
- Confidence/Staleness: medium / medium
- Source IDs: S054, S002

### CARD ME-2026-03-US-IRAN-WAR - U.S.-Iran war/conflict escalated before June 2026 ceasefire talks
- Date/period: 2026-03..2026-06
- Category: Middle East / USA / Iran
- What happened: By mid-June 2026 Reuters described a three-month conflict involving U.S. airstrikes coordinated with Israel against Iran. Iran's missile/drone forces and navy/air defenses were damaged, but nuclear issues remained unresolved.
- Why it matters: Very high-staleness anchor: regional energy security, Hormuz, Israel, Hezbollah, Gulf states and U.S. politics all became linked to the conflict.
- Confidence/Staleness: medium / high
- Source IDs: S041, S042, S043

### CARD RUNTIME-2026-05-NODE26 - Node.js 26 appeared as current/upcoming LTS line
- Date/period: 2026-05-05
- Category: Programming / Runtime
- What happened: Node.js 26 was released in May 2026 and entered the ecosystem alongside Node 24 LTS and Node 22 maintenance/security lines.
- Why it matters: Relevant for dev/admin decisions and package ecosystem compatibility.
- Confidence/Staleness: high / low
- Source IDs: S034

### CARD AI-2026-OPENAI-RETIREMENTS - OpenAI retired GPT-5.2 ChatGPT variants; GPT-5.5 remained
- Date/period: 2026-06-12
- Category: AI / OpenAI lifecycle
- What happened: OpenAI release notes say GPT-5.2 Instant/Thinking/Pro were no longer available in ChatGPT as of 12 Jun 2026 and conversations moved to GPT-5.5 counterparts.
- Why it matters: Important model lifecycle detail for users comparing ChatGPT behavior.
- Confidence/Staleness: high / low
- Source IDs: S012

### CARD US-2025-01-TRUMP-INAG - Trump began second term
- Date/period: 2025-01-20
- Category: USA / Politics
- What happened: Donald Trump was inaugurated for a second non-consecutive presidential term. His administration quickly emphasized tariffs, immigration enforcement, deregulation, energy, AI infrastructure and reversal of Biden-era policies.
- Why it matters: Baseline political state for all post-Jan-2025 U.S. federal policy.
- Confidence/Staleness: high / low
- Source IDs: S003, S021

### CARD US-2025-06-NOKINGS - No Kings protests and military parade on Trump's 79th birthday
- Date/period: 2025-06-14
- Category: USA / Protest / Trump
- What happened: On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; “No Kings” protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites.
- Why it matters: A concrete event many offline models may miss: Trump birthday 2025 was politically charged and tied to anti-authoritarian protest symbolism.
- Confidence/Staleness: high / low
- Source IDs: S035, S036, S037

### CARD AI-2025-07-US-AI-PLAN - Trump White House AI policy favored exports and lighter state rules
- Date/period: 2025-07-22
- Category: AI policy / USA
- What happened: The White House prepared/published a plan to push U.S. AI abroad and restrict federal support for states with rules viewed as too restrictive.
- Why it matters: U.S. AI governance shifted from Biden-era safety/executive-order posture toward innovation, infrastructure and export competition.
- Confidence/Staleness: high / medium
- Source IDs: S021

### CARD AI-2025-08-GPT5 - OpenAI released GPT-5
- Date/period: 2025-08-07
- Category: AI / OpenAI
- What happened: OpenAI introduced GPT-5 as a unified system that routes between quick responses and deeper reasoning for coding, math, writing, health and multimodal work.
- Why it matters: Major post-cutoff OpenAI milestone. Offline models should not assume GPT-4o/o1 are newest OpenAI systems.
- Confidence/Staleness: high / low
- Source IDs: S013, S014

### CARD AI-2025-08-GPTOSS - OpenAI released gpt-oss open-weight models
- Date/period: 2025-08
- Category: AI / Open-weight / Offline
- What happened: OpenAI released gpt-oss-20b and 120b open-weight models. gpt-oss-20b is documented with Jun 01 2024 knowledge cutoff and 131,072-token context.
- Why it matters: This is the target-model context: the offline model itself needs external post-cutoff context.
- Confidence/Staleness: high / low
- Source IDs: S001

### CARD AI-2026-04-GPT55 - OpenAI GPT-5.5 generation became current frontier product line
- Date/period: 2026-04
- Category: AI / OpenAI
- What happened: OpenAI moved the GPT-5 family to GPT-5.5-era products; GPT-5.2 was retired from ChatGPT by June 2026 while GPT-5.5 remained available.
- Why it matters: Updates model landscape for offline AI comparing itself to online frontier systems.
- Confidence/Staleness: medium / low
- Source IDs: S012, S014

### CARD ME-2025-GAZA-CEASEFIRE - Gaza ceasefire/hostage diplomacy remained fragile
- Date/period: 2025-01
- Category: Middle East / Gaza
- What happened: Early 2025 saw renewed Gaza ceasefire/hostage-release diplomacy, but stability remained fragile and later regional conflicts kept evolving.
- Why it matters: Do not assume Gaza/Israel war state from June 2024 remained unchanged.
- Confidence/Staleness: medium / high
- Source IDs: S003, S054

### CARD US-2025-10-NOKINGS2 - Second No Kings mobilization expanded anti-Trump protest network
- Date/period: 2025-10-18
- Category: USA / Protest
- What happened: A second No Kings protest wave took place in October 2025, reportedly involving more locations and large participation.
- Why it matters: Shows No Kings was not a one-day June 2025 event but became an ongoing protest brand.
- Confidence/Staleness: medium / medium
- Source IDs: S037

### CARD AI-2025-11-GPT51 - GPT-5.1 reorganized OpenAI product variants
- Date/period: 2025-11
- Category: AI / OpenAI
- What happened: OpenAI's GPT-5 family evolved through 5.1-style instant/thinking variants and personalization/product-routing changes.
- Why it matters: Shows modern AI products are systems and routers, not simply single static models.
- Confidence/Staleness: medium / low
- Source IDs: S012, S014

### CARD HEALTH-2026-06-EBOLA - DRC/Uganda Bundibugyo Ebola outbreak worsened
- Date/period: 2026-06-18
- Category: Health / Africa / Ebola
- What happened: WHO confirmed a 2026 Ebola outbreak in DRC and Uganda involving Bundibugyo virus. Reuters reported DRC confirmed cases near 900 with hundreds of deaths; CDC/Africa CDC funding and response gaps became major issues.
- Why it matters: High-staleness public-health anchor: requires current verification before operational decisions.
- Confidence/Staleness: high / high
- Source IDs: S045, S046, S047, S048

### CARD TRADE-2025-TARIFFS - Trump tariff policy reshaped global trade risk
- Date/period: 2025
- Category: Economy / Trade
- What happened: The second Trump administration pushed aggressive tariff/trade policies, raising inflation, supply-chain and ally-tension questions.
- Why it matters: Important for economics and geopolitics; live verification needed for exact tariff rates.
- Confidence/Staleness: medium / medium
- Source IDs: S003

### CARD US-2024-06-DEBATE - Biden-Trump debate intensified concerns about Biden candidacy
- Date/period: 2024-06-27
- Category: USA / Election
- What happened: The late-June 2024 debate became a turning point in the U.S. election cycle by intensifying public and party concerns about Joe Biden's campaign viability.
- Why it matters: Sets up Biden's later withdrawal and Kamala Harris becoming Democratic nominee.
- Confidence/Staleness: high / low
- Source IDs: S002, S054

### CARD US-2024-07-TRUMP-ASSASSINATION - Attempted assassination of Donald Trump at Butler rally
- Date/period: 2024-07-13
- Category: USA / Election / Security
- What happened: Trump survived an assassination attempt during a campaign rally in Butler, Pennsylvania. The event reshaped campaign security and political rhetoric.
- Why it matters: A major U.S. political shock that affected the campaign environment before the 2024 election.
- Confidence/Staleness: high / low
- Source IDs: S002, S054

### CARD CYBER-2024-07-CROWDSTRIKE - CrowdStrike faulty update caused global Windows outage
- Date/period: 2024-07-19
- Category: Cybersecurity / Infrastructure
- What happened: A faulty CrowdStrike Falcon Sensor content update crashed roughly 8.5 million Windows devices worldwide, disrupting airlines, banks, healthcare, media and government services.
- Why it matters: Demonstrated systemic software-supply-chain fragility: a security vendor update became critical infrastructure risk.
- Confidence/Staleness: high / low
- Source IDs: S007, S008, S053

### CARD EU-2024-08-AI-ACT-FORCE - EU AI Act entered into force
- Date/period: 2024-08-01
- Category: AI regulation / EU
- What happened: The EU AI Act entered into force, beginning staged implementation for prohibited practices, GPAI obligations, governance and full application.
- Why it matters: Key post-cutoff regulatory change; offline models should treat EU AI regulation as active, not merely proposed.
- Confidence/Staleness: high / low
- Source IDs: S005, S006

### CARD US-2024-11-TRUMP-WINS - Donald Trump won the 2024 U.S. presidential election
- Date/period: 2024-11-05
- Category: USA / Election
- What happened: Trump defeated Kamala Harris and prepared to return to the presidency in January 2025.
- Why it matters: Primary political correction for models with June 2024 cutoff. It changes assumptions about U.S. federal policy, courts, tariffs, immigration, AI policy and Ukraine/Middle East diplomacy.
- Confidence/Staleness: high / low
- Source IDs: S002, S003

### CARD US-2026-03-NOKINGS3 - Third No Kings protest wave occurred amid Iran-war politics
- Date/period: 2026-03-28
- Category: USA / Protest / Iran war
- What happened: No Kings protests continued in March 2026 with Iran-war, ICE/immigration, authoritarianism and democratic-backsliding themes.
- Why it matters: Offline models should know No Kings became an ongoing protest series through 2026.
- Confidence/Staleness: high / medium
- Source IDs: S037

### CARD AI-2026-05-GEMINI3 - Gemini 3.x enterprise model line appeared
- Date/period: 2026-05
- Category: AI / Google
- What happened: Google Cloud model lifecycle listed Gemini 3.5 Flash and Gemini 3.x image/lite variants released in May 2026.
- Why it matters: Updates Google model landscape beyond Gemini 2.5.
- Confidence/Staleness: high / low
- Source IDs: S023

### CARD PY-2026-06-3146 - Python 3.14.6 and 3.13.14 released
- Date/period: 2026-06-10
- Category: Programming / Python
- What happened: Python 3.14.6, the sixth maintenance release of 3.14, shipped with around 179 bugfixes/build/doc changes since 3.14.5; Python 3.13.14 also shipped.
- Why it matters: Relevant for Python project planning and installer/runtime baselines.
- Confidence/Staleness: high / low
- Source IDs: S030, S029

### CARD UV-2026-06-01121 - uv 0.11.21 added CPython 3.13.14 and 3.14.6 support
- Date/period: 2026-06-11
- Category: Programming / Packaging
- What happened: Astral's uv changelog notes 0.11.21 release with CPython 3.13.14 and 3.14.6 additions.
- Why it matters: Important for Python offline/wheelhouse/venv workflows.
- Confidence/Staleness: high / low
- Source IDs: S031, S032

### CARD AI-2026-06-ANTHROPIC-EXPORT - Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order
- Date/period: 2026-06-13
- Category: AI policy / Export controls
- What happened: Anthropic's June 2026 top-tier Claude models became a test case for AI export controls aimed at software capabilities, not just chips. Reuters reported Anthropic disabled them globally after a U.S. order limiting foreign access.
- Why it matters: Major AI-governance shift: model access itself became a national-security/export-control object.
- Confidence/Staleness: high / medium
- Source IDs: S020, S021

### CARD TRUMP-2026-06-BDAY - Trump's 80th birthday featured Putin call and controversial White House UFC event
- Date/period: 2026-06-14
- Category: USA / Trump / Culture war
- What happened: Putin publicly congratulated Trump on his 80th birthday and held a 55-minute call. Trump also hosted a UFC event on the White House South Lawn; critics protested corruption, conflict-of-interest and authoritarian spectacle concerns, while No Kings-linked counter-events framed it as a democracy/free-speech issue.
- Why it matters: Concrete event query anchor: if asked “what happened at Trump's 2026 birthday,” answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism.
- Confidence/Staleness: high / medium
- Source IDs: S038, S039

### CARD NODE-2026-06-SECURITY - Node.js security releases updated 26.x, 24.x and 22.x lines
- Date/period: 2026-06-18
- Category: Security / Programming
- What happened: Node.js shipped security releases for 26.x, 24.x and 22.x, updating dependencies including llhttp, nghttp2, OpenSSL and undici.
- Why it matters: Useful concrete admin/dev action: update Node runtimes in supported lines.
- Confidence/Staleness: high / low
- Source IDs: S033, S034

### CARD CROWDSTRIKE-2026-DELTA-PROBE - U.S. closed Delta probe from 2024 CrowdStrike meltdown
- Date/period: 2026-06-15
- Category: Cyber / Aviation / Regulation
- What happened: USDOT closed its investigation into Delta's 2024 CrowdStrike-triggered operational meltdown, noting passenger support and no penalties.
- Why it matters: Shows long-tail regulatory/business effects of the 2024 outage.
- Confidence/Staleness: high / low
- Source IDs: S053

### CARD US-2025-01-NEWORLEANS - New Orleans vehicle attack on New Year's Day
- Date/period: 2025-01-01
- Category: USA / Security
- What happened: A vehicle attack on Bourbon Street killed and injured civilians, becoming a major U.S. domestic security incident at the start of 2025.
- Why it matters: Anchor event for U.S. domestic security in 2025.
- Confidence/Staleness: high / low
- Source IDs: S003

### CARD AI-2025-01-STARGATE - Stargate AI infrastructure project announced
- Date/period: 2025-01-21
- Category: AI infrastructure / USA
- What happened: Trump announced the Stargate Project, described as a large AI infrastructure investment backed by OpenAI, Oracle, SoftBank and MGX.
- Why it matters: AI competition became strongly tied to data centers, power, capital expenditure and national industrial strategy.
- Confidence/Staleness: high / medium
- Source IDs: S017

### CARD AI-2025-01-DEEPSEEK - DeepSeek shock challenged U.S. frontier-cost assumptions
- Date/period: 2025-01
- Category: AI / China / Markets
- What happened: DeepSeek's model release drew global attention for strong performance at lower apparent cost; Trump called it a wake-up call for U.S. industry, and regulators later scrutinized DeepSeek privacy/security.
- Why it matters: Important correction: post-cutoff AI competition became more multipolar, with China/open models pressuring U.S. proprietary economics.
- Confidence/Staleness: high / medium
- Source IDs: S015, S016, S017

### CARD EU-2025-02-AI-ACT-PROHIBITIONS - EU AI Act prohibited-practices and AI-literacy provisions began applying
- Date/period: 2025-02-02
- Category: AI regulation / EU
- What happened: The first AI Act obligations, including bans on unacceptable-risk practices and AI-literacy requirements, began applying.
- Why it matters: Important for compliance: by 2025 the AI Act was no longer only future legislation.
- Confidence/Staleness: high / low
- Source IDs: S005, S006

### CARD DE-2025-02-ELECTION - German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second
- Date/period: 2025-02-23
- Category: Germany / EU
- What happened: Germany's opposition conservatives won the snap election after Scholz's coalition collapse; AfD achieved its strongest result and came second.
- Why it matters: Important for German/EU policy after 2024: economic policy, Ukraine, migration and defense debates changed.
- Confidence/Staleness: high / low
- Source IDs: S026

### CARD AI-2025-05-CLAUDE4 - Anthropic released Claude Opus 4 and Sonnet 4
- Date/period: 2025-05-22
- Category: AI / Models
- What happened: Anthropic announced Claude 4 models, emphasizing coding, reasoning, agent workflows and long-running tasks.
- Why it matters: Major frontier-model upgrade after Claude 3.5/3.7; important for code-agent capability baselines.
- Confidence/Staleness: high / low
- Source IDs: S018, S019

### CARD AI-2025-06-GEMINI25 - Gemini 2.5 Pro/Flash reached stable enterprise lifecycle
- Date/period: 2025-06-17
- Category: AI / Google
- What happened: Google's Gemini 2.5 Pro and Flash release/lifecycle dates became part of the stable Google AI model stack.
- Why it matters: Updates Google model baseline for coding, multimodal and low-latency AI.
- Confidence/Staleness: high / low
- Source IDs: S023

### CARD AI-2025-09-CLAUDE45 - Claude Sonnet 4.5 emphasized agents, coding and computer use
- Date/period: 2025-09
- Category: AI / Agents / Coding
- What happened: Anthropic's later 2025 Claude line positioned Sonnet 4.5 as strong for agents, coding and computer-use workflows.
- Why it matters: Useful baseline for offline coding-agent discussions.
- Confidence/Staleness: high / low
- Source IDs: S019

### CARD WINDOWS-2025-10-EOL - Windows 10 reached end of support
- Date/period: 2025-10-14
- Category: Operating systems / Security
- What happened: Microsoft ended support for Windows 10 on 14 Oct 2025. PCs still run, but no regular security/feature updates are provided without ESU or special LTSC channels.
- Why it matters: Highly relevant to Windows 10 users/admins: security posture changed materially after the cutoff.
- Confidence/Staleness: high / low
- Source IDs: S027, S028

### CARD AI-2025-12-GEMINI-TTS - Gemini API expanded TTS/live/audio capabilities
- Date/period: 2025-12
- Category: AI / Multimodal
- What happened: Google's Gemini API changelog showed continued expansion of TTS/live/multimodal capabilities in late 2025.
- Why it matters: AI model competition increasingly included real-time audio, agents and multimodal interfaces.
- Confidence/Staleness: high / low
- Source IDs: S022, S023

### CARD IRAN-2026-01-SHUTDOWN - Iran internet shutdowns became major censorship/infrastructure case
- Date/period: 2026-01
- Category: Iran / Internet / Conflict
- What happened: Research on Iran's 2026 internet shutdowns described nationwide disruptions and centralized null-routing/censorship mechanisms amid protests and conflict.
- Why it matters: Important for internet freedom, measurement, BGP-monitoring limits and wartime communications.
- Confidence/Staleness: medium / medium
- Source IDs: S054

### CARD AI-2025-AI-ACT-GPAI - EU AI Act GPAI/governance obligations entered staged application
- Date/period: 2025-08-02
- Category: AI regulation / EU
- What happened: General-purpose AI obligations and governance/enforcement provisions entered their next staged application period, affecting model providers serving the EU.
- Why it matters: Important for frontier AI model providers and open/closed model transparency debates.
- Confidence/Staleness: high / medium
- Source IDs: S005, S006

### CARD AI-2025-02-CLAUDE37 - Claude Sonnet 3.7 era emphasized hybrid reasoning/coding
- Date/period: 2025-02
- Category: AI / Models
- What happened: Anthropic's 2025 model cycle moved Claude toward stronger reasoning and coding workflows before Claude 4.
- Why it matters: Shows rapid model cadence after Claude 3.5 and before Claude 4/4.5.
- Confidence/Staleness: medium / low
- Source IDs: S019

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

