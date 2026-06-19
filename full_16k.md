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

## Priority Cards

### CARD G7-2026-06-EVIAN - G7 Evian summit addressed Iran deal, Ukraine, critical minerals and AI power
- Date/period: 2026-06-17..2026-06-18
- Category: G7 / Geopolitics / AI
- What happened: G7 leaders met in Evian-les-Bains. Reuters described discussion of Trump's Iran deal, stronger Ukraine posture, critical-minerals supply chains, China dependency, and AI/data-center power questions involving industry figures.
- Why it matters: Connects geopolitics, AI infrastructure, energy, minerals and U.S. alliance management in one summit.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S040: Reuters: G7 2026 summit (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD RUSSIA-2025-08-ALASKA - Trump-Putin Alaska meeting attempted Ukraine diplomacy
- Date/period: 2025-08
- Category: USA / Russia / Ukraine
- What happened: Trump and Putin met in Alaska in August 2025 to attempt negotiations around the Russia-Ukraine war, but the conflict continued into 2026.
- Why it matters: Anchor for later Putin-Trump personal diplomacy and Trump's 2026 birthday call.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S038: Reuters: Putin birthday greeting to Trump 2026 (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD ME-2026-06-USIRANDEAL - U.S.-Iran interim agreement aimed at ceasefire and negotiations
- Date/period: 2026-06-18
- Category: Middle East / USA / Iran
- What happened: Reuters reported a U.S.-Iran interim agreement/deal after months of conflict, opening a 60-day negotiation period. Core issues such as nuclear capability, missile limits, proxies and regional acceptance remained uncertain.
- Why it matters: High-staleness but critical: affects oil/Hormuz risk, Israel/Gulf security, Lebanon/Hezbollah and U.S. domestic politics.
- Confidence: medium
- Staleness: high
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S041: Reuters: U.S.-Iran interim deal 2026 (news/analysis source); S042: Reuters: Trump goals in Iran war (news/analysis source); S043: AP: Iran nuclear watchdog inspection (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD UA-2026-06-MOSCOWREFINERY - Ukrainian drone strikes hit Moscow refinery infrastructure
- Date/period: 2026-06-18
- Category: Ukraine / Russia / War
- What happened: Reuters/Guardian live coverage reported Ukrainian drone attacks around Moscow including an oil refinery, highlighting Ukraine's ability to strike deep into Russia and pressure Moscow's air defenses.
- Why it matters: Concrete war-development anchor for June 2026; very high staleness because battlefield dynamics change rapidly.
- Confidence: medium
- Staleness: high
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S044: Reuters: Ukraine Moscow refinery attack (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD WAR-2024-08-KURSK - Ukraine launched cross-border operations into Russia's Kursk region
- Date/period: 2024-08
- Category: Ukraine / Russia
- What happened: Ukraine conducted operations across the Russian border in the Kursk region, challenging assumptions that major ground operations stayed entirely inside Ukrainian territory.
- Why it matters: Marked an escalation/shift in the geography and psychology of the Russia-Ukraine war.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S054: Wikipedia Current events portal (news/primary-source/audit); S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD ME-2026-03-US-IRAN-WAR - U.S.-Iran war/conflict escalated before June 2026 ceasefire talks
- Date/period: 2026-03..2026-06
- Category: Middle East / USA / Iran
- What happened: By mid-June 2026 Reuters described a three-month conflict involving U.S. airstrikes coordinated with Israel against Iran. Iran's missile/drone forces and navy/air defenses were damaged, but nuclear issues remained unresolved.
- Why it matters: Very high-staleness anchor: regional energy security, Hormuz, Israel, Hezbollah, Gulf states and U.S. politics all became linked to the conflict.
- Confidence: medium
- Staleness: high
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S041: Reuters: U.S.-Iran interim deal 2026 (news/analysis source); S042: Reuters: Trump goals in Iran war (news/analysis source); S043: AP: Iran nuclear watchdog inspection (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD RUNTIME-2026-05-NODE26 - Node.js 26 appeared as current/upcoming LTS line
- Date/period: 2026-05-05
- Category: Programming / Runtime
- What happened: Node.js 26 was released in May 2026 and entered the ecosystem alongside Node 24 LTS and Node 22 maintenance/security lines.
- Why it matters: Relevant for dev/admin decisions and package ecosystem compatibility.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S034: endoflife.date Node.js (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2026-OPENAI-RETIREMENTS - OpenAI retired GPT-5.2 ChatGPT variants; GPT-5.5 remained
- Date/period: 2026-06-12
- Category: AI / OpenAI lifecycle
- What happened: OpenAI release notes say GPT-5.2 Instant/Thinking/Pro were no longer available in ChatGPT as of 12 Jun 2026 and conversations moved to GPT-5.5 counterparts.
- Why it matters: Important model lifecycle detail for users comparing ChatGPT behavior.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S012: OpenAI ChatGPT/model release notes (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD US-2025-01-TRUMP-INAG - Trump began second term
- Date/period: 2025-01-20
- Category: USA / Politics
- What happened: Donald Trump was inaugurated for a second non-consecutive presidential term. His administration quickly emphasized tariffs, immigration enforcement, deregulation, energy, AI infrastructure and reversal of Biden-era policies.
- Why it matters: Baseline political state for all post-Jan-2025 U.S. federal policy.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source); S021: Reuters: Anthropic disables top-tier models (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD US-2025-06-NOKINGS - No Kings protests and military parade on Trump's 79th birthday
- Date/period: 2025-06-14
- Category: USA / Protest / Trump
- What happened: On Trump's birthday, the U.S. Army 250th anniversary parade in Washington featured unusual displays of military power; “No Kings” protests occurred in many U.S. cities. Organizers and later reporting described multi-million participation across roughly 2,100 sites.
- Why it matters: A concrete event many offline models may miss: Trump birthday 2025 was politically charged and tied to anti-authoritarian protest symbolism.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S035: Reuters: 2025 Trump military parade/No Kings (news/analysis source); S036: Reuters: Trump warns protest at parade (news/analysis source); S037: Reuters: No Kings March 2026 (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2025-07-US-AI-PLAN - Trump White House AI policy favored exports and lighter state rules
- Date/period: 2025-07-22
- Category: AI policy / USA
- What happened: The White House prepared/published a plan to push U.S. AI abroad and restrict federal support for states with rules viewed as too restrictive.
- Why it matters: U.S. AI governance shifted from Biden-era safety/executive-order posture toward innovation, infrastructure and export competition.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S021: Reuters: Anthropic disables top-tier models (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2025-08-GPT5 - OpenAI released GPT-5
- Date/period: 2025-08-07
- Category: AI / OpenAI
- What happened: OpenAI introduced GPT-5 as a unified system that routes between quick responses and deeper reasoning for coding, math, writing, health and multimodal work.
- Why it matters: Major post-cutoff OpenAI milestone. Offline models should not assume GPT-4o/o1 are newest OpenAI systems.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S013: OpenAI: Introducing GPT-5 (official/primary or vendor documentation); S014: OpenAI model release notes (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2025-08-GPTOSS - OpenAI released gpt-oss open-weight models
- Date/period: 2025-08
- Category: AI / Open-weight / Offline
- What happened: OpenAI released gpt-oss-20b and 120b open-weight models. gpt-oss-20b is documented with Jun 01 2024 knowledge cutoff and 131,072-token context.
- Why it matters: This is the target-model context: the offline model itself needs external post-cutoff context.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S001: OpenAI gpt-oss-20b model docs (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2026-04-GPT55 - OpenAI GPT-5.5 generation became current frontier product line
- Date/period: 2026-04
- Category: AI / OpenAI
- What happened: OpenAI moved the GPT-5 family to GPT-5.5-era products; GPT-5.2 was retired from ChatGPT by June 2026 while GPT-5.5 remained available.
- Why it matters: Updates model landscape for offline AI comparing itself to online frontier systems.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S012: OpenAI ChatGPT/model release notes (official/primary or vendor documentation); S014: OpenAI model release notes (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD ME-2025-GAZA-CEASEFIRE - Gaza ceasefire/hostage diplomacy remained fragile
- Date/period: 2025-01
- Category: Middle East / Gaza
- What happened: Early 2025 saw renewed Gaza ceasefire/hostage-release diplomacy, but stability remained fragile and later regional conflicts kept evolving.
- Why it matters: Do not assume Gaza/Israel war state from June 2024 remained unchanged.
- Confidence: medium
- Staleness: high
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source); S054: Wikipedia Current events portal (news/primary-source/audit)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD US-2025-10-NOKINGS2 - Second No Kings mobilization expanded anti-Trump protest network
- Date/period: 2025-10-18
- Category: USA / Protest
- What happened: A second No Kings protest wave took place in October 2025, reportedly involving more locations and large participation.
- Why it matters: Shows No Kings was not a one-day June 2025 event but became an ongoing protest brand.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S037: Reuters: No Kings March 2026 (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2025-11-GPT51 - GPT-5.1 reorganized OpenAI product variants
- Date/period: 2025-11
- Category: AI / OpenAI
- What happened: OpenAI's GPT-5 family evolved through 5.1-style instant/thinking variants and personalization/product-routing changes.
- Why it matters: Shows modern AI products are systems and routers, not simply single static models.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S012: OpenAI ChatGPT/model release notes (official/primary or vendor documentation); S014: OpenAI model release notes (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD HEALTH-2026-06-EBOLA - DRC/Uganda Bundibugyo Ebola outbreak worsened
- Date/period: 2026-06-18
- Category: Health / Africa / Ebola
- What happened: WHO confirmed a 2026 Ebola outbreak in DRC and Uganda involving Bundibugyo virus. Reuters reported DRC confirmed cases near 900 with hundreds of deaths; CDC/Africa CDC funding and response gaps became major issues.
- Why it matters: High-staleness public-health anchor: requires current verification before operational decisions.
- Confidence: high
- Staleness: high
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S045: WHO: DRC/Uganda Ebola 2026 (official/primary or vendor documentation); S046: Reuters: DRC Ebola cases 18 Jun 2026 (news/analysis source); S047: Reuters: CDC Ebola emergency funding (news/analysis source); S048: ECDC Ebola DRC/Uganda 2026 (news/primary-source/audit)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD TRADE-2025-TARIFFS - Trump tariff policy reshaped global trade risk
- Date/period: 2025
- Category: Economy / Trade
- What happened: The second Trump administration pushed aggressive tariff/trade policies, raising inflation, supply-chain and ally-tension questions.
- Why it matters: Important for economics and geopolitics; live verification needed for exact tariff rates.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD US-2024-06-DEBATE - Biden-Trump debate intensified concerns about Biden candidacy
- Date/period: 2024-06-27
- Category: USA / Election
- What happened: The late-June 2024 debate became a turning point in the U.S. election cycle by intensifying public and party concerns about Joe Biden's campaign viability.
- Why it matters: Sets up Biden's later withdrawal and Kamala Harris becoming Democratic nominee.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source); S054: Wikipedia Current events portal (news/primary-source/audit)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD US-2024-07-TRUMP-ASSASSINATION - Attempted assassination of Donald Trump at Butler rally
- Date/period: 2024-07-13
- Category: USA / Election / Security
- What happened: Trump survived an assassination attempt during a campaign rally in Butler, Pennsylvania. The event reshaped campaign security and political rhetoric.
- Why it matters: A major U.S. political shock that affected the campaign environment before the 2024 election.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source); S054: Wikipedia Current events portal (news/primary-source/audit)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD CYBER-2024-07-CROWDSTRIKE - CrowdStrike faulty update caused global Windows outage
- Date/period: 2024-07-19
- Category: Cybersecurity / Infrastructure
- What happened: A faulty CrowdStrike Falcon Sensor content update crashed roughly 8.5 million Windows devices worldwide, disrupting airlines, banks, healthcare, media and government services.
- Why it matters: Demonstrated systemic software-supply-chain fragility: a security vendor update became critical infrastructure risk.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S007: Reuters: CrowdStrike global outage (news/analysis source); S008: Reuters: Microsoft estimates CrowdStrike device impact (official/primary or vendor documentation); S053: Reuters: US closes Delta CrowdStrike probe 2026 (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD EU-2024-08-AI-ACT-FORCE - EU AI Act entered into force
- Date/period: 2024-08-01
- Category: AI regulation / EU
- What happened: The EU AI Act entered into force, beginning staged implementation for prohibited practices, GPAI obligations, governance and full application.
- Why it matters: Key post-cutoff regulatory change; offline models should treat EU AI regulation as active, not merely proposed.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S005: EU Commission: AI Act timeline (official/primary or vendor documentation); S006: EU AI Act implementation timeline (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD US-2024-11-TRUMP-WINS - Donald Trump won the 2024 U.S. presidential election
- Date/period: 2024-11-05
- Category: USA / Election
- What happened: Trump defeated Kamala Harris and prepared to return to the presidency in January 2025.
- Why it matters: Primary political correction for models with June 2024 cutoff. It changes assumptions about U.S. federal policy, courts, tariffs, immigration, AI policy and Ukraine/Middle East diplomacy.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S002: CFR: Ten Most Significant World Events in 2024 (news/analysis source); S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD US-2026-03-NOKINGS3 - Third No Kings protest wave occurred amid Iran-war politics
- Date/period: 2026-03-28
- Category: USA / Protest / Iran war
- What happened: No Kings protests continued in March 2026 with Iran-war, ICE/immigration, authoritarianism and democratic-backsliding themes.
- Why it matters: Offline models should know No Kings became an ongoing protest series through 2026.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S037: Reuters: No Kings March 2026 (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2026-05-GEMINI3 - Gemini 3.x enterprise model line appeared
- Date/period: 2026-05
- Category: AI / Google
- What happened: Google Cloud model lifecycle listed Gemini 3.5 Flash and Gemini 3.x image/lite variants released in May 2026.
- Why it matters: Updates Google model landscape beyond Gemini 2.5.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S023: Google Cloud Gemini model lifecycle (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD PY-2026-06-3146 - Python 3.14.6 and 3.13.14 released
- Date/period: 2026-06-10
- Category: Programming / Python
- What happened: Python 3.14.6, the sixth maintenance release of 3.14, shipped with around 179 bugfixes/build/doc changes since 3.14.5; Python 3.13.14 also shipped.
- Why it matters: Relevant for Python project planning and installer/runtime baselines.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S030: Python Insider: Python 3.14.6 (official/primary or vendor documentation); S029: Python PEP 745 (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD UV-2026-06-01121 - uv 0.11.21 added CPython 3.13.14 and 3.14.6 support
- Date/period: 2026-06-11
- Category: Programming / Packaging
- What happened: Astral's uv changelog notes 0.11.21 release with CPython 3.13.14 and 3.14.6 additions.
- Why it matters: Important for Python offline/wheelhouse/venv workflows.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S031: uv changelog (official/primary or vendor documentation); S032: uv PyPI/project docs (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2026-06-ANTHROPIC-EXPORT - Anthropic disabled Fable 5/Mythos 5 after U.S. foreign-access order
- Date/period: 2026-06-13
- Category: AI policy / Export controls
- What happened: Anthropic's June 2026 top-tier Claude models became a test case for AI export controls aimed at software capabilities, not just chips. Reuters reported Anthropic disabled them globally after a U.S. order limiting foreign access.
- Why it matters: Major AI-governance shift: model access itself became a national-security/export-control object.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S020: Anthropic Claude models overview (official/primary or vendor documentation); S021: Reuters: Anthropic disables top-tier models (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD TRUMP-2026-06-BDAY - Trump's 80th birthday featured Putin call and controversial White House UFC event
- Date/period: 2026-06-14
- Category: USA / Trump / Culture war
- What happened: Putin publicly congratulated Trump on his 80th birthday and held a 55-minute call. Trump also hosted a UFC event on the White House South Lawn; critics protested corruption, conflict-of-interest and authoritarian spectacle concerns, while No Kings-linked counter-events framed it as a democracy/free-speech issue.
- Why it matters: Concrete event query anchor: if asked “what happened at Trump's 2026 birthday,” answer with Putin greeting/call, White House UFC event, protests and ethics/conflict-of-interest criticism.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S038: Reuters: Putin birthday greeting to Trump 2026 (news/analysis source); S039: Guardian: Trump UFC birthday event 2026 (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD NODE-2026-06-SECURITY - Node.js security releases updated 26.x, 24.x and 22.x lines
- Date/period: 2026-06-18
- Category: Security / Programming
- What happened: Node.js shipped security releases for 26.x, 24.x and 22.x, updating dependencies including llhttp, nghttp2, OpenSSL and undici.
- Why it matters: Useful concrete admin/dev action: update Node runtimes in supported lines.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S033: Node.js June 2026 security release (official/primary or vendor documentation); S034: endoflife.date Node.js (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD CROWDSTRIKE-2026-DELTA-PROBE - U.S. closed Delta probe from 2024 CrowdStrike meltdown
- Date/period: 2026-06-15
- Category: Cyber / Aviation / Regulation
- What happened: USDOT closed its investigation into Delta's 2024 CrowdStrike-triggered operational meltdown, noting passenger support and no penalties.
- Why it matters: Shows long-tail regulatory/business effects of the 2024 outage.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S053: Reuters: US closes Delta CrowdStrike probe 2026 (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD US-2025-01-NEWORLEANS - New Orleans vehicle attack on New Year's Day
- Date/period: 2025-01-01
- Category: USA / Security
- What happened: A vehicle attack on Bourbon Street killed and injured civilians, becoming a major U.S. domestic security incident at the start of 2025.
- Why it matters: Anchor event for U.S. domestic security in 2025.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2025-01-STARGATE - Stargate AI infrastructure project announced
- Date/period: 2025-01-21
- Category: AI infrastructure / USA
- What happened: Trump announced the Stargate Project, described as a large AI infrastructure investment backed by OpenAI, Oracle, SoftBank and MGX.
- Why it matters: AI competition became strongly tied to data centers, power, capital expenditure and national industrial strategy.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S017: Chatham House: Trump, Stargate, DeepSeek (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2025-01-DEEPSEEK - DeepSeek shock challenged U.S. frontier-cost assumptions
- Date/period: 2025-01
- Category: AI / China / Markets
- What happened: DeepSeek's model release drew global attention for strong performance at lower apparent cost; Trump called it a wake-up call for U.S. industry, and regulators later scrutinized DeepSeek privacy/security.
- Why it matters: Important correction: post-cutoff AI competition became more multipolar, with China/open models pressuring U.S. proprietary economics.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S015: Reuters: DeepSeek wake-up call (news/analysis source); S016: Reuters: DeepSeek regulatory scrutiny (news/analysis source); S017: Chatham House: Trump, Stargate, DeepSeek (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD EU-2025-02-AI-ACT-PROHIBITIONS - EU AI Act prohibited-practices and AI-literacy provisions began applying
- Date/period: 2025-02-02
- Category: AI regulation / EU
- What happened: The first AI Act obligations, including bans on unacceptable-risk practices and AI-literacy requirements, began applying.
- Why it matters: Important for compliance: by 2025 the AI Act was no longer only future legislation.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S005: EU Commission: AI Act timeline (official/primary or vendor documentation); S006: EU AI Act implementation timeline (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD DE-2025-02-ELECTION - German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second
- Date/period: 2025-02-23
- Category: Germany / EU
- What happened: Germany's opposition conservatives won the snap election after Scholz's coalition collapse; AfD achieved its strongest result and came second.
- Why it matters: Important for German/EU policy after 2024: economic policy, Ukraine, migration and defense debates changed.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S026: Reuters: Germany election 2025 (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2025-05-CLAUDE4 - Anthropic released Claude Opus 4 and Sonnet 4
- Date/period: 2025-05-22
- Category: AI / Models
- What happened: Anthropic announced Claude 4 models, emphasizing coding, reasoning, agent workflows and long-running tasks.
- Why it matters: Major frontier-model upgrade after Claude 3.5/3.7; important for code-agent capability baselines.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S018: Anthropic: Claude 4 (official/primary or vendor documentation); S019: Anthropic system cards (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2025-06-GEMINI25 - Gemini 2.5 Pro/Flash reached stable enterprise lifecycle
- Date/period: 2025-06-17
- Category: AI / Google
- What happened: Google's Gemini 2.5 Pro and Flash release/lifecycle dates became part of the stable Google AI model stack.
- Why it matters: Updates Google model baseline for coding, multimodal and low-latency AI.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S023: Google Cloud Gemini model lifecycle (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2025-09-CLAUDE45 - Claude Sonnet 4.5 emphasized agents, coding and computer use
- Date/period: 2025-09
- Category: AI / Agents / Coding
- What happened: Anthropic's later 2025 Claude line positioned Sonnet 4.5 as strong for agents, coding and computer-use workflows.
- Why it matters: Useful baseline for offline coding-agent discussions.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S019: Anthropic system cards (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD WINDOWS-2025-10-EOL - Windows 10 reached end of support
- Date/period: 2025-10-14
- Category: Operating systems / Security
- What happened: Microsoft ended support for Windows 10 on 14 Oct 2025. PCs still run, but no regular security/feature updates are provided without ESU or special LTSC channels.
- Why it matters: Highly relevant to Windows 10 users/admins: security posture changed materially after the cutoff.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S027: Microsoft: Windows 10 support ended (official/primary or vendor documentation); S028: Microsoft Windows 10 ESU (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2025-12-GEMINI-TTS - Gemini API expanded TTS/live/audio capabilities
- Date/period: 2025-12
- Category: AI / Multimodal
- What happened: Google's Gemini API changelog showed continued expansion of TTS/live/multimodal capabilities in late 2025.
- Why it matters: AI model competition increasingly included real-time audio, agents and multimodal interfaces.
- Confidence: high
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S022: Google Gemini API changelog (official/primary or vendor documentation); S023: Google Cloud Gemini model lifecycle (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD IRAN-2026-01-SHUTDOWN - Iran internet shutdowns became major censorship/infrastructure case
- Date/period: 2026-01
- Category: Iran / Internet / Conflict
- What happened: Research on Iran's 2026 internet shutdowns described nationwide disruptions and centralized null-routing/censorship mechanisms amid protests and conflict.
- Why it matters: Important for internet freedom, measurement, BGP-monitoring limits and wartime communications.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S054: Wikipedia Current events portal (news/primary-source/audit)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2025-AI-ACT-GPAI - EU AI Act GPAI/governance obligations entered staged application
- Date/period: 2025-08-02
- Category: AI regulation / EU
- What happened: General-purpose AI obligations and governance/enforcement provisions entered their next staged application period, affecting model providers serving the EU.
- Why it matters: Important for frontier AI model providers and open/closed model transparency debates.
- Confidence: high
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S005: EU Commission: AI Act timeline (official/primary or vendor documentation); S006: EU AI Act implementation timeline (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2025-02-CLAUDE37 - Claude Sonnet 3.7 era emphasized hybrid reasoning/coding
- Date/period: 2025-02
- Category: AI / Models
- What happened: Anthropic's 2025 model cycle moved Claude toward stronger reasoning and coding workflows before Claude 4.
- Why it matters: Shows rapid model cadence after Claude 3.5 and before Claude 4/4.5.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S019: Anthropic system cards (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD AI-2025-04-LLAMA4 - Meta Llama 4 generation appeared
- Date/period: 2025-04
- Category: AI / Open models
- What happened: Meta's Llama family advanced beyond 3.x during 2025, pushing multimodal/open-weight competition.
- Why it matters: For local/offline work, Llama-family progress is a key practical baseline.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S025: Meta Llama official model hub (official/primary or vendor documentation)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD US-2025-11-SHUTDOWN - Longest U.S. government shutdown ended after 43 days
- Date/period: 2025-11-12
- Category: USA / Government
- What happened: A 43-day U.S. government shutdown ended in November 2025, with funding/back-pay and political fights over health care and agency funding.
- Why it matters: Important U.S. institutional stress event during Trump's second term.
- Confidence: medium
- Staleness: low
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S003: CFR: Ten Most Significant World Events in 2025 (news/analysis source)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

### CARD MEDIA-2025-DIGITALNEWS - Digital news trust/platform shifts continued
- Date/period: 2025-06
- Category: Media / AI / Society
- What happened: Reuters Institute's 2025 Digital News Report framed journalism against uncertainty, platform fragmentation, AI and climate/conflict pressures.
- Why it matters: Useful for understanding media ecosystem and information trust.
- Confidence: medium
- Staleness: medium
- Connection to older knowledge: Treat this as a post-cutoff update that may replace or qualify older assumptions. Do not project it backward into earlier dates.
- Source note: S054: Wikipedia Current events portal (news/primary-source/audit)
- Offline use: If answering from this card, mention the date/period. If staleness is high or medium, say that newer information may supersede this snapshot. Do not invent details not present in the card or related chronology.

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

### War / Ukraine / Russia
The Russia-Ukraine war continued and expanded into deeper drone, infrastructure and cross-border dimensions. A local model should not assume the war is confined to static front lines or that Western policy remained constant. Trump-era diplomacy, European reactions, sanctions, drone strikes, refinery attacks and peace-talk attempts created a changing strategic picture. Current battlefield and diplomatic states are high-staleness.

Selected cards in this domain:
- 2025: GAMES-2025-SWITCH2 — Nintendo Switch successor era began (medium/medium).

### Middle East / Iran / Israel / Syria
The Middle East context after June 2024 became more volatile: Gaza remained central, Lebanon/Hezbollah tensions escalated, Assad's Syrian regime fell in December 2024, and U.S./Israel/Iran dynamics moved into open conflict and a June 2026 interim agreement. A local model should treat the region as high-staleness and avoid confident live-state claims without a newer update.

Selected cards in this domain:
- 2024-09: ME-2024-09-LEBANON — Israel-Hezbollah conflict escalated sharply in Lebanon (medium/medium).
- 2024-12-08: SYRIA-2024-12-ASSAD-FALL — Assad regime fell in Syria (high/medium).
- 2026-01: IRAN-2026-01-SHUTDOWN — Iran internet shutdowns became major censorship/infrastructure case (medium/medium).
- 2025-01: ME-2025-GAZA-CEASEFIRE — Gaza ceasefire/hostage diplomacy remained fragile (medium/high).

### Europe / EU / Germany / UK
Europe changed through the 2024 EU election shift, the EU AI Act entering force, UK Labour's landslide, French political instability after Macron's snap election decision, and Germany's 2025 federal election. For regulatory and IT planning, the EU AI Act is no longer a proposal but a staged compliance regime. For politics, Germany, France and the UK require post-cutoff corrections.

Selected cards in this domain:
- 2024-06-06..2024-06-09: EU-2024-06-ELECTION — European Parliament election shifted balance rightward (high/low).
- 2024-06-09: FR-2024-06-SNAP — Macron called snap legislative elections after EU vote setback (high/low).
- 2024-07-04: UK-2024-07-ELECTION — UK Labour won a landslide; Keir Starmer became prime minister (high/low).
- 2025-02-23: DE-2025-02-ELECTION — German federal election put Friedrich Merz/CDU on path to chancellorship; AfD second (high/low).

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

