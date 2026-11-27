# Hypothesis & Success Metrics

> **Module 3 · ★ Deliverable 3.** Repo file `03-analytics/hypothesis-and-metrics.md` — part of your submission.
> Do the lab in the **Module 3 · Exercise Guide** (linked from the Module 3 deck), then click **⬇ Download .md** — it saves as this exact file. Commit it here.
> It feeds the **Problem, Value & Hypothesis** slide of your Module 6 final deck.

## Finalized product hypothesis

> Based on a night-shift dispatcher's report that the board can't be trusted, which forces fallback calls and texts, and reporting coordinator CSAT of 1.3, I believe that making live driver location and route-change delivery reliable for real-time dispatchers will result in delays being corrected before customers notice them, as measured by a 30% improvement in CSAT. I will protect on-time delivery rate, dispatcher time-to-resolve per exception, and driver app battery and data usage, and will make a go/no-go decision after a 4-week pilot (with a checkpoint at week 2).

## Success metrics

| Metric | Type | Target | Why it matters |
|---|---|---|---|
| _North-star_ CSAT (reporting coordinators) | Outcome | +30% (from 1.3) | Dispatchers can act on delivery problems before customers experience them, because they have trustworthy live visibility into every driver and a dependable channel to get changes to them. |
| _Leading indicator_ [workflow completion after Route Assignment] | Initiative signal | [target, from 31% completion today] | 69% of Coordinators abandon the workflow after Route Assignment; this should move first if the board becomes trustworthy. |
| _Guardrail_ Scheduling CSAT for coordinators; on-time delivery rate; dispatcher time-to-resolve per exception; driver app battery and data usage | Product signal | Must not drop | Protects the existing base while live tracking and route-change delivery change. |

## Pre-work · Hypothesis check

- **Role, who you are solving for (from M2):** The Real-Time Dispatcher: an operations dispatcher, often on night shift, who reassigns stops and steers drivers through late or failed deliveries as they happen.
- **Goal, what this user is ultimately trying to achieve:** See where every driver really is and get route changes to them right away, so delays get fixed before customers notice.
- **Friction / moment of misery, the specific pain blocking their goal:** The board can't be trusted. Driver status lags 20 to 60 minutes and completed stops still show as "in progress," so the dispatcher runs the fleet from a WhatsApp group. A night-shift dispatcher said outright that the board can't be trusted.
- **Current workaround, the external tool or manual process they rely on (M2):** A WhatsApp group with drivers, direct texts and phone calls to drivers.
- **Problem Hook, your one-sentence framing of the business crisis (M1):** We must stop our largest enterprise account and others from leaving for competitors by fixing the slow workflows that force dispatchers to use WhatsApp and texts just to coordinate their fleet in real time.
- **Value Proposition, the outcome your initiative promised to deliver (M1):** For dispatchers and fleet managers responsible for real-time fleet coordination, we will make RouteLogic the fastest way to coordinate a fleet in real time, so they can re-route, reassign, and resolve issues without leaving the product for WhatsApp, texts, or other outside tools. We'll get there by reclaiming the product's operational simplicity: using existing user research to audit the current experience, keep what's essential to the core coordination workflow, and cut the legacy noise that slows it down, because our largest enterprise account is already evaluating competitors, and others are likely to follow.

## Read your data snapshots

- **Does the funnel data confirm your M2 friction point, or does it tell a different story? Note where the numbers align with the qualitative pain you found and where they diverge.:** _(not filled in)_
- **Do the retention patterns align with the workaround your M2 persona used to find content? Note what the Mo. 0→1 drop suggests about the onboarding experience your persona described as frustrating.:** _(not filled in)_
- **Does the LTV gap and the content mix (61% trending for Wanderers) confirm the moment of misery your persona described? Note which segment your persona is in and whether the data confirms their pain.:** _(not filled in)_
- **Does the low adoption confirm your persona is burdened by tools they don't use? Note whether the low scheduling adoption (42%) for coordinators matches your M2 moment of misery.:** Yes it does
- **Does the workflow data match the manual process or hack you documented in M2? Note whether the specific drop-offs or time gaps explain why your persona avoids the digital tool.:** Yes absolutely
- **Look at the CSAT heatmap. Which specific cell most directly maps to your persona's friction? Note how the NPS trend justifies the urgency of your M1 Problem Hook.:** Reporting coordinators - 1.3

## Step 3 · Craft your hypothesis

- **Qualitative evidence (from M2), quote the specific friction / moment of misery for your persona:** A night-shift dispatcher states the board cannot be trusted: driver status lags 20 to 60 minutes and completed stops still show as "in progress," so dispatchers describe a WhatsApp group as the "real system."
- **Quantitative evidence (from M3), name the metric or data point that confirms the pain; cite the number:** 69% of Coordinators abandon the workflow after Route Assignment.
- **Persona, role, goal, and the friction you confirmed in the reconciliation steps:**
  - Role: The Real-Time Dispatcher: an operations dispatcher, often on night shift, who reassigns stops and steers drivers through late or failed deliveries as they happen.
  - Goal: See where every driver really is and get route changes to them right away, so delays get fixed before customers notice.
  - Friction point: unreliable app
- **Problem you are solving, one sentence describing the specific friction this initiative removes:** Dispatchers can't trust the driver app to show where drivers actually are or to deliver route changes promptly, so they can't fix delays before customers feel them.
- **Strategic outcome, what behaviour change do you expect, and how does it map to retention / revenue / churn?:** Dispatchers stop running the fleet from WhatsApp and texts and coordinate inside RouteLogic, because the board shows where drivers really are and route changes reach drivers right away. That moves RouteLogic back to being the system of record for daily operations, which protects retention: it answers the main complaint of the enterprise account now trialing a leaner competitor and the renewal at risk from low frontline adoption. Measured by saved churn through the renewal of the largest enterprise account at risk.
- **Primary success metric (initiative signal), the leading indicator that tells you the gap is closing:** Dispatchers can act on delivery problems before customers experience them, because they have trustworthy live visibility into every driver and a dependable channel to get changes to them.
- **Guardrail metric (product signal), the metric that must NOT drop; it protects your existing base:** Scheduling CSAT for coordinators
- **Decision window, how much time or data before you scale, pivot, or kill? minimum threshold to proceed?:** A 4-week pilot, including the largest enterprise account, with interviews running alongside it.
  - **Week 2:** stop or change course if average daily time lost to manual workarounds does not decrease by 10 minutes or if the Assign Routes via Optimizer step does not decrease by 3 minutes.
  - **Week 4 go/no-go:** scale if at least [X%] of reassignments go through RouteLogic without a follow-up WhatsApp message or text, and CSAT is trending toward the +30% target, with no guardrail drop. Pivot if the board is trusted but WhatsApp use doesn't fall. Kill if neither moves.
  - Churn impact can't be proven in 4 weeks; we use in-app coordination as the leading signal and track renewal of the pilot accounts after that.
