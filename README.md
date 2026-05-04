# AI-Assisted Artifacts

> Architecture Reference // 2026
> Every effort produces an artifact. Every artifact closes a loop. Every loop closes with evidence — not a status update.
> **8 domains · 27 rules**
> Lifecycle: EFFORT · ARTIFACT · CLOSE · EVIDENCE

---

## 01 // Foundation
**What is the artifact principle, and why is "done" not the same as "closed"?**

An artifact is the externalized evidence that work happened — a document, a commit, a recording, a decision log. Without an artifact, work exists only in the head of the person who did it: invisible to the team, unreviewable, and unable to compound. High performance in remote, distributed teams is not heroic individual output — it is consistent loop-closing through intentional artifact creation. **If a day of effort produced no artifact, either the work wasn't worth it, or the output wasn't captured — and both are problems worth surfacing.**

1. **An artifact is the only verifiable evidence that work happened** — Work that lives only in someone's head is not done — it is invisible. An artifact externalizes the output of effort in a form that can be read, reviewed, questioned, and built upon by others. The absence of an artifact is not humility; it is a system gap. In remote teams, invisible work is the same as no work — neither can be coordinated, reviewed, or compounded.
2. **"Done" is a process state — "closed" is an evidence state** — Marking a ticket done means the work stopped. A closed loop means the right people have the artifact, the signal has been observed, and the work's impact is confirmed. A PR can be merged (done) while the feature's effect is unmeasured (open loop). The goal is not done — it is closed.
3. **High performance is consistent loop-closing — not sporadic heroics** — A team member who closes one loop every day for a quarter outperforms one who closes five loops in a sprint and goes quiet for six weeks. High performance is not exclusive to high IQ or high effort — it is the result of intentional, repeated discipline to close loops with evidence.

---

## 02 // Effort–Artifact–Evidence
**What artifact does each class of work produce, and what evidence closes the loop?**

Every category of work has a canonical artifact and a specific evidence condition that closes the loop. Research loops close when a decision is recorded. Bug fix loops close when telemetry confirms the fix. Feature loops close when signals show usage without regression. **The loop closure condition is the part most teams skip — producing artifacts but never verifying they reached their purpose.**

| Effort | Artifact | Loop closes when… |
|---|---|---|
| Research | Spike document | Decision is recorded and shared |
| Incident | RCA / postmortem | Action items have owners and dates |
| Bug fix | Commit + PR | Telemetry confirms fix in production |
| Feature | PR + flag rollout | Signals show usage and no regression |
| Training | Report or write-up | Insight is applied or shared with peers |
| Meeting | Decision record | Updates reach all relevant parties |

1. **Research → Spike: the loop closes when a decision is recorded and shared — not when exploration ends** — A research effort that ends without a decision record produced no lasting value. The spike records the context, the options considered, and the decision made. The loop closes when the relevant decision-makers have acknowledged the path forward.
2. **Feature → PR + flag rollout: the loop closes when signals show usage and no regression — not when the PR merges** — A feature is not shipped when deployed; it is shipped when real users are using it, metrics show engagement, and no upstream signals degraded. Merge velocity without signal velocity is churn disguised as progress.
3. **Bug fix → telemetry: the loop closes when production confirms the symptom is resolved — not when the fix ships** — Merging a PR is deploying a candidate fix. The loop closes when production telemetry confirms the symptom is resolved. Teams that measure fix velocity without measuring fix confirmation are optimizing the wrong metric.
4. **Meeting → decision record: the loop closes when updates reach relevant parties — not when the call ends** — A meeting where every attendee walks away with a different understanding of what was decided is a shared ambiguity event. The meeting loop closes when the decision is written down, action items have owners and dates, and relevant parties who were not in the room have been briefed.

---

## 03 // AI-Assisted Generation
**How does AI change the economics of artifact creation, and what does it not change?**

The bottleneck in artifact creation is almost never writing speed — it is starting. A blank page for a postmortem, a spike, or a meeting summary creates friction that causes the artifact to be deferred, then forgotten. AI eliminates that friction: given context, it produces a structured first draft in seconds. **AI lowers the activation energy. The discipline requirement — to close the loop with real evidence — does not change.**

1. **AI eliminates the blank-page problem — the bottleneck was never writing speed** — The friction in artifact creation is starting, not finishing. Given a brief context dump — what happened, what we checked, what we did — AI produces a structured draft in under a minute. The bottleneck was never writing ability or time. It was the activation energy of the blank page.
2. **Prompt with context, not with the task — artifact quality is proportional to the context provided** — "Write a postmortem" produces generic output. "Here are the timeline, the contributing factors, and the three action items with owners and dates — structure this into a postmortem for internal review" produces a useful draft. Front-loading context is the highest-leverage investment in AI-assisted artifact velocity.
3. **AI-generated artifacts require human review before loop closure — generation is not closure** — An AI-produced spike or RCA is a draft, not a closed loop. The human author must review for factual accuracy, completeness of context, and correctness of the decision record before publishing. The signal is not that an artifact was generated — it is that a human reviewed, approved, and routed it.
4. **Use AI to generate artifacts for efforts that previously produced none — that is the highest-value application** — The highest-value use is not making good artifacts faster — it is generating artifacts for classes of work that historically produced nothing. Training session follow-ups, informal Slack decisions, architectural reasoning documented after the fact — these loops were left open because the artifact cost was too high. AI makes the cost near-zero. The discipline is applying it consistently.

---

## 04 // Loop Closure
**What does it mean for a loop to be closed, and how do you distinguish closed from merely shipped?**

A closed loop has three components: an artifact, an audience, and a signal. The artifact externalizes the work. The audience confirms the right people received it. The signal confirms the impact was observed. Most teams hit the artifact stage and stop — they create the output but never verify it reached the people who needed it. **A loop closed without a signal is an artifact in a void — not a loop at all.**

1. **A closed loop requires an artifact, an audience, and a signal — missing any one leaves it open** — The artifact without an audience is a document in a folder nobody opens. The artifact without a signal is a PR merged without checking if the bug is fixed. The audience without an artifact is a verbal update that leaves no record. All three are required.
2. **If nobody relevant read it, the loop is not closed — routing is not optional** — A postmortem published to a wiki that nobody links or references is not a closed loop. Loop closure requires intentional routing: who needs this, how will it reach them, and how will you know it did. The loop closes when the signal travels, not when the artifact is created.
3. **Define the loop closure condition before starting the work — not after, when the team is tired** — "Write an RCA" has no closure condition. "Write an RCA, share it in #incidents, get acknowledgment from the on-call lead, and add action items to Jira" has one. Closure conditions defined after the fact are chosen to confirm done, not to confirm closed.

---

## 05 // Remote-First Transparency
**What does distributed work demand from artifact culture that co-located work could absorb informally?**

Co-located teams absorb informal communication — the hallway conversation, the overheard decision, the whiteboard that stays up all week. Distributed teams cannot. In async, remote-first environments, the artifact is the only communication channel. There is no ambient awareness of what teammates are working on. **Remote work does not create a higher standard for artifact quality — it creates a minimum viable standard for artifact existence.**

1. **Remote work converts implicit context into explicit artifacts — or loses it permanently** — In an office, context travels informally. In distributed teams, context that is not written down does not exist for anyone who was not in the specific conversation. The artifact is not a bureaucratic add-on — it is the mechanism by which distributed teams maintain shared context.
2. **Artifacts replace the hallway conversation — and last longer than any hallway conversation ever did** — A decision made in a three-message Slack thread will be lost within a week. A decision record takes five minutes to write and serves the same purpose for the next six months. Teams that write down decisions as a habit outperform teams that decide verbally and document only when someone asks.
3. **The artifact is the communication — not a supplement to it** — In async culture, "I finished the spike, let me know if you want to discuss" is not communication — it is an offer to communicate later. The artifact is the communication: the document, with the decision highlighted and the relevant stakeholders tagged. Optimizing for async artifact quality is not process overhead — it is the primary delivery mechanism of distributed work.

---

## 06 // Individual Visibility
**What does it mean to surface your own contribution, and why is it a team responsibility — not a personal one?**

In distributed teams, contribution that is not made visible does not exist in the system. This is not about personal recognition — it is about system completeness. If a team member closes a meaningful loop but nobody else knows it happened, the work cannot be built upon, the decision cannot be referenced, and the impact cannot compound. **Surfacing your own contribution is system hygiene, not self-promotion — and it is a responsibility to the team, not an indulgence of ego.**

1. **Everyone must surface their own contribution — intentionally, not by accident or management prompt** — Waiting for a manager to notice, or assuming completed work will be discovered, is not modesty — it is a failure of the distributed system's signal. In high-trust, high-transparency teams, surfacing your own work is the default behavior. The team cannot coordinate around work it cannot see.
2. **A day with no visible artifact is a signal that something went wrong — and naming it is the right move** — If a day of effort produced no artifact, either the work wasn't worth doing or the output wasn't captured. Both are worth surfacing. Silence is not a signal of productivity — it is the absence of a signal, which in a distributed system reads as the absence of work.
3. **Contribution visibility is distinct from status updates — artifacts close loops, activity logs don't** — "I worked on the auth service today" is an activity report. An artifact closes a loop: "I investigated the auth latency spike — spike doc here — root cause is token validation overhead, recommended fix is X, decision needed from Y by Z." The first describes effort. The second produces a closable loop with an owner and a next step.

---

## 07 // Signals & Telemetry
**How do you know a loop actually closed, and what counts as evidence versus assertion?**

An artifact published is a loop claimed to be closed. Evidence that the artifact reached its purpose is a loop confirmed closed. The signal bridges the gap — the telemetry confirming the bug is fixed, the read receipt confirming the decision was seen, the metric confirming the feature is being used. Without the signal, the artifact is a claim, not a confirmation. **Evidence is not a formality — it is the difference between a closed loop and an open one dressed in documentation.**

1. **Define what counts as evidence before the artifact is created — improvised closure confirms done, not closed** — A spike document closes when stakeholders acknowledge the decision. An RCA closes when action items have owners and dates and are tracked. A bug fix closes when production error rates return to baseline. Closure conditions defined after the fact are chosen to fit what's already true.
2. **Telemetry is the highest-integrity signal — it cannot be socially pressured into confirming done** — A team member reporting "the bug is fixed" is asserting closure. A dashboard showing error rate returning to baseline is confirming it. Telemetry-based closure conditions are not subject to optimism bias, deadline pressure, or social friction. Make telemetry-based closure the default for technical work.
3. **Missing signals are the canary for missing work — treat them as such** — A feature deployed with no usage signal after 30 days is not a feature that nobody used — it is a feature with an uninstrumented loop. When a signal is missing, the question is not "is the work done?" — it is "what is preventing us from knowing whether the work mattered?" That question is worth asking before the next sprint starts.

---

## 08 // Culture & Cadence
**What organizational conditions make consistent loop-closing sustainable rather than exhausting?**

Artifact discipline at individual scale is a habit. At team scale, it is a culture. The conditions that make it sustainable are psychological safety to share imperfect drafts, low-ego ownership where the artifact belongs to the team rather than the author, trust that surfacing problems is rewarded rather than punished, and a daily cadence that makes closing one loop per day the norm. **We all win if we all row the same cadence — toward the same end goal — and the loop closes with evidence, not with a Friday dump of what was done.**

1. **Daily focused progress compounds — weekly dumps do not** — A team where every member closes one loop per day produces compounding signal that a team dumping work on Fridays never will. Daily closure means feedback arrives while context is fresh and blockers surface while they are still small. Weekly reporting is not a cadence — it is a lag disguised as a process.
2. **Low ego: the artifact belongs to the team — the author's name is for accountability, not ownership** — Artifacts in high-performing teams are working documents: draft quality is acceptable and expected, corrections are welcomed, and the goal is accuracy rather than credit. The best artifacts are the ones that improve through multiple sets of eyes before closure.
3. **Culture that penalizes visible mistakes produces work that surfaces only when it is already too late to be useful** — The most dangerous outcome of a low-trust culture is not bad work — it is invisible work. Trust is the prerequisite for the artifact system to function. Psychological safety is what allows people to surface imperfect early work early enough to be redirected.
4. **High collab: the best artifacts are built in public and improved by others before the loop closes** — A spike document written in private and published when finished is less accurate than one written in public where teammates catch errors before they become decisions. Sharing in-progress artifacts for async review is not a sign of uncertainty — it is the mechanism by which distributed teams build shared context without synchronous meetings.

---

## The mental model

> Every effort produces an artifact. Every artifact closes a loop. Every loop closes with evidence.
> Done is a process state. Closed is an evidence state.
> AI lowers the activation energy. The discipline requirement does not change.
> Surfacing your own contribution is system hygiene — not self-promotion.
> We all win if we all row the same cadence, toward the same end goal.

---

*Daniel Brasileiro · [ai-artifacts.w-b.dev](https://ai-artifacts.w-b.dev)*
