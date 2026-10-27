# Netflix UX Design - Research and Validation Kit

## Project purpose

**Project:** From Browsing to Belonging  
**Design concept:** Tonight, quickly  
**Platform lens:** Mobile-first Netflix India discovery flow, with familiar Home, Search, My List, and playback entry points  
**Status:** Concept design and self-review are complete. Three viewer interviews and three participant usability sessions remain to be conducted.

The assignment asks for a complete UX process: research, persona and JTBD, competitor analysis, journey, three wireframes, a clickable prototype with save or compare, and testing with three people. This kit makes the research and testing work executable while keeping real evidence separate from scenario assumptions.

## Evidence integrity

- **Source-supported context:** A narrow statement supported by a linked public source.
- **Hypothesis:** A question about viewer behavior that needs primary research.
- **Concept decision:** A design choice made for this prototype.
- **Observed result:** Reserved for notes from real sessions. No participant results are included here.
- **AI-assisted walkthrough:** A designer self-review of the prototype. It is not a participant test and must not be described as user validation.

No interview quotes, usability results, adoption metrics, or improvement percentages have been invented.

## Challenge and scope

Viewers who have a limited time window may spend more effort browsing and comparing than they intended. The design explores whether surfacing optional time, audio-language, and mood filters - then showing concise reasons for fit - can make a short list easier to evaluate.

**In scope:** intent filters, recommendation cards, runtime and language cues, detail evaluation, save/return, compare, and a playback handoff.

**Out of scope:** Netflix production UI, a live catalog or recommendation model, video streaming, subscriptions, account settings implementation, and claims about current Netflix performance.

**Design question:** How might we help a limited-time viewer find a title that feels right without inspecting the entire catalog?

## Research plan

### Participants

Recruit three current streaming viewers. If possible, include:

- A person who often watches alone and one who shares viewing decisions.
- At least one person who regularly uses audio or subtitles beyond their default.
- A mix of people who browse and people who commonly search or return to a saved title.

These are recruitment goals for a small formative study, not a representative sample. Avoid recruiting only UX designers.

### 20-minute interview

1. Welcome, explain that the project is a concept exercise, and ask permission to take notes.
2. Ask for a recent, concrete viewing-choice story before showing any prototype.
3. Follow the actions in order. Ask what was looked at, opened, ruled out, saved, or revisited.
4. Ask what information created confidence and what was still uncertain.
5. Only after the story, show the concept and ask what the participant expects each control to do.
6. Close by asking what would make them return to their current way of choosing.

Do not ask leading questions such as “Would a runtime filter be helpful?” Prefer “What did you need to know before deciding?”

### Neutral interview guide

1. Think about the last time you opened Netflix and were not sure what to watch. What happened?
2. What did you already know about your time, mood, or who was watching?
3. What did you look at before choosing? What made you rule a title in or out?
4. Did you search, browse, ask someone, or return to a saved title? Show me if you can.
5. How did you know the title was a good fit? What was still uncertain?

Useful follow-up prompts: “What happened next?”, “Can you show me?”, “What made that matter?”, and “How often does that happen?”

### Consent and note handling

Tell the participant the goal is to learn about the interface, not evaluate them. Participation is optional; they can stop at any time. Do not record identifying or sensitive information unless explicitly agreed and needed. Keep notes anonymous using P1, P2, and P3.

## Proto-persona

### Meera - after-work viewer (scenario composite)

**Context assumption:** Around 27, often has 30-45 minutes after work, sometimes shares the screen, and moves between phone and TV. These details make a coherent design scenario; they are not findings about a real participant.

**Goal hypothesis:** Find a title that fits tonight without turning the choice into another task.

**Potential friction:** Broad discovery rows may not surface runtime, language availability, or tone early enough.

**Potential need:** A small shortlist, an understandable reason for fit, and an easy way to save a maybe or change direction.

**Validation needed:** Check whether viewers actually use these signals, the order they seek them in, and what “confident enough to play” means to them.

## JTBD, problem frame, and hypotheses

### Job to be done

When I have limited time and a rough sense of what I feel like watching, I want to quickly identify a title that fits my time, language, and mood, so I can feel good about pressing Play instead of continuing to browse.

### How might we

Help a limited-time viewer find a title that feels right without making them inspect the entire catalog?

### Opportunity hypotheses

| Hypothesis | What to learn | Evidence to capture |
|---|---|---|
| A recommendation needs to explain its fit. | Does a concise reason help people shortlist? | Card opens, reasons mentioned, shortlist choices |
| Runtime, language, and mood may be decision signals. | Which signals are sought before details? | Search/filter path, detail checks, participant language |
| Save and compare may reduce backtracking. | Can viewers change direction and return easily? | Revisits, saved-title retrieval, comparison actions |

After interviews, tag observed behavior first. Keep a participant quote distinct from the researcher’s interpretation. Update or discard hypotheses when evidence disagrees.

## Competitor and product-pattern desk scan

This is a directional review of public product/help material. It is not a hands-on usability audit.

| Product | Public pattern reviewed | Design learning | Concept opportunity |
|---|---|---|---|
| Netflix | Recommendations are personalized; audio/subtitles can be selected; My Netflix brings together saved and in-progress items on supported surfaces. | Personalization and return paths are important discovery infrastructure. | Make short-list intent and fit cues explicit in one route. |
| Prime Video | Public help covers profiles, title details, playback language, and captions. | Language and profile expectations matter through discovery and playback. | Surface language availability before the viewer commits. |
| JioHotstar | Public accessibility-plan scope includes discovery and playback areas such as search, home, watch, categories, and My Space. | Discovery accessibility spans entry points. | Keep labels, focus states, and handoff understandable. |

These sources do not establish comparative usability, satisfaction, or performance. See the source list at the end.

## Journey map

| Stage | Viewer action | Question | Friction hypothesis | Design opportunity |
|---|---|---|---|---|
| Open | Opens the app | What fits tonight? | Intent is not explicit | Capture optional context |
| Browse | Scans rows or searches | Where should I look? | Too many similar choices | Show a focused short list |
| Evaluate | Opens title details | Will I enjoy it? | Key information arrives late | Surface runtime, language, tone |
| Decide | Chooses or saves | Is there a better pick? | Decision fatigue | Confirm fit and support saving |
| Play | Starts a title | Is audio right? | Language surprise | Expose audio and subtitle labels |
| Return | Resumes or revisits | Where is my pick? | Shortlist may be lost | Keep My List visible |

This map is a working model to check during interviews, not a report of measured user behavior.

## Information architecture

- **Discover:** Home rows and the optional Tonight, quickly route.
- **Search:** Existing title, genre, or language lookup remains available.
- **My Netflix / My List:** Saved titles and return paths.
- **Account:** Existing profile and language settings.
- **Title details:** Synopsis, runtime, maturity label, audio/subtitle signals, Play, Save.
- **Playback handoff:** A concept transition; no video is streamed in this prototype.

## Core user flows

### Find something now

Open Home → optionally set time → optionally set audio language → optionally set mood → scan fit cues → open details → Play.

### Keep an option for later

Open a title → Save → return to Home → open My List → review fit → Play or remove.

Filters are optional and reversible. Standard Search and My List remain reachable.

## Wireframe intent

### Screen 1 - Discovery

Question answered: “What fits tonight?”

- Optional time, language, and mood chips.
- Compact set of distinct candidates.
- Runtime and audio visible without opening details.
- A concise “why it may fit” reason.
- Save and details actions.

### Screen 2 - Title details

Question answered: “Is this the one?”

- Clear title identity and synopsis.
- Runtime, genre, and maturity label.
- Audio and subtitle availability separated.
- Fit summary that references the selected intent.
- Play and My List actions.

### Screen 3 - Decision support

Question answered: “Help me compare.”

- Compare up to three titles.
- Show runtime, mood, genre, audio, and subtitles.
- Use plain differences rather than a single opaque score.
- Allow removal and return to discovery.

The clickthrough prototype implements discovery, title details, compare, save-to-My-List, and a playback handoff using fictional content.

## Prototype behavior

Open index.html in a browser or enable GitHub Pages after uploading.

- Time, audio-language, and mood filters update the concept list.
- Clear filters restores the default list.
- View details and back preserve the discovery state.
- Save changes to Saved, gives feedback, and stores locally in the browser.
- My List shows saved concept titles.
- Compare can hold up to three titles and presents their signals side by side.
- Play opens a clearly labeled concept handoff; it does not stream video.

All titles, artwork, runtimes, language availability, and descriptions are invented interaction examples. No real catalog data is represented.

## Usability test plan

### Participants and setup

Run three moderated sessions, approximately 15-20 minutes each. Use the prototype on a phone-sized viewport where possible. Ask participants to think aloud, but do not steer them toward a particular filter or card. Start a timer when each task is read. Stop it when the participant selects Play or completes the intended save-and-return task.

### Task prompts

1. “You have about half an hour and want something light in Hindi. Find a title you would consider playing.”
2. “You are not ready now. Save a title, then show me where you would return to it.”
3. “Compare two options and tell me what would make you choose one.”

### Measures and definitions

| Measure | Record |
|---|---|
| Task success | Independent, assisted, or not completed; define the intended end state before each session. |
| Time to decision | Seconds from reading the task to selecting a suitable Play or saved return state. |
| Confusion | Misclicks, backtracking, hesitation, questions, and where they occur. |
| Confidence | Ask for a 1-5 rating after each task and “What drove that rating?” |
| Qualitative fit | Which signal or information changed the participant’s choice, if any. |

Do not average three people into a performance claim. Use the sessions to find breakdowns and decide what to revise. Report participant count and context with any observation.

### Blank session record

Duplicate this section once per participant.

**Participant ID:**  
**Date / device:**  
**Viewing context (self-described):**  

| Task | Success (independent / assisted / no) | Time | Confusion / backtracking | Confidence (1-5) | Quote or observable note |
|---|---|---|---|---|---|
| 1. Find a light Hindi title under 30 min |  |  |  |  |  |
| 2. Save and find a title again |  |  |  |  |  |
| 3. Compare two options |  |  |  |  |  |

**What helped:**  
**What blocked progress:**  
**Unexpected behavior:**  
**Follow-up change to test:**  

## AI-assisted walkthrough and iteration notes

These are designer-led, AI-assisted task rehearsals using the concept state. They are not user research, not usability tests, and not evidence of participant behavior or improved outcomes. No times, scores, or quotes were generated.

| Scenario rehearsal | Intended path | Design check |
|---|---|---|
| Find a fit | Choose under 30 minutes, light mood, and Hindi audio; compare Monsoon Letters and Small Wins; inspect details; reach the concept Play state. | Runtime, audio, and the reason for fit are visible before opening details. |
| Save for later | Save a title, see confirmation, open My List, and return to its detail page. | Saved state and return location are unmistakable. |
| Compare choices | Select two titles, compare runtime, mood, and language, then remove one or return to discovery. | Differences are legible; the small shortlist stays manageable. |

**Iterations included in the prototype:** empty-state recovery, Saved confirmation and My List, separate audio/subtitle labels, and a three-title comparison cap. These rehearsals produce no participant metrics.

## Accessibility and trust checklist

- Use semantic headings, buttons, and tables; ensure controls are keyboard reachable.
- Provide visible focus and text labels for selected states.
- Keep audio and subtitle availability distinct.
- Do not autoplay sound or imply artwork is the only source of title information.
- Preserve a clear back path and a way to reset filters.
- Explain that content and availability are fictional concept data.
- Do not claim algorithmic personalization or a Netflix integration.
- Avoid presenting AI-assisted walkthrough notes as findings from viewers.

## Sources

1. Netflix Help Center, “How Netflix recommendations work”: https://help.netflix.com/en/node/100639/
2. Netflix Help Center, “How to use subtitles, captions, or choose audio language”: https://help.netflix.com/en/node/372
3. Netflix Help Center, My Netflix / TV experience: https://help.netflix.com/en/node/321880164349028
4. Prime Video Help: https://www.primevideo.com/-/te/help?tr=gp
5. JioHotstar Accessibility Plan: https://secure-media.hotstar.com/web-assets/prod/accessibilityplan/ca/eng/accessibilityplan_ca_eng.html
