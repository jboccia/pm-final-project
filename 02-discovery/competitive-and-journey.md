# Competitive Analysis & Journey Map

> **Module 2 · Lab 2 — ★ Deliverable 2.** Repo file `02-discovery/competitive-and-journey.md` — part of your submission.
> Do the lab in the **Module 2 · Exercise 2 Guide** (linked from the Module 2 deck), then click **⬇ Download .md** — it saves as this exact file. Commit it here.
> It becomes the **Competitive Analysis & Journey Map** slide of your Module 6 final deck. Builds on your `ai-synthesis.md` and your Module 1 `problem-hook.md`.

## Responses

- **Role, who are you solving for?:** The Real-Time Dispatcher: an operations dispatcher, often on night shift, who reassigns stops and steers drivers through late or failed deliveries as they happen.
- **Goal, what is this user ultimately trying to achieve?:** See where every driver really is and get route changes to them right away, so delays get fixed before customers notice.
- **Friction, the main barrier (moment of misery) stopping them:** The board can't be trusted. Driver status lags 20 to 60 minutes and completed stops still show as "in progress," so the dispatcher runs the fleet from a WhatsApp group. A night-shift dispatcher said outright that the board can't be trusted.
- **External tools the user is forced to use:** A WhatsApp group with drivers, direct texts and phone calls to drivers.
- **The process, the 3–5 manual steps they take:**
  1. Check the dispatcher board, knowing driver status may be 20 to 60 minutes out of date.
  2. Ask drivers in the WhatsApp group or by text where they are and which stops are done.
  3. Reassign stops in RouteLogic, then text or WhatsApp the driver, because the change takes 8 to 15 minutes to arrive with no push notification.
  4. When a driver's app crashes mid-route, read the remaining stops aloud over the phone.
- **Core frustration, where the process feels most "broken":** The dispatcher can neither trust what the board shows nor trust that a change reached the driver, so every reassignment is done twice: once in RouteLogic and again in WhatsApp. The platform's central coordination job has moved to a chat app, and that operational data never makes it back into RouteLogic.
- **The evidence, a quote or behavior from the research:** Dispatchers describe a WhatsApp group as the "real system"; a night-shift dispatcher states the board cannot be trusted; driver status lags 20 to 60 minutes and route changes take 8 to 15 minutes to reach drivers.
- **Journey map, a shareable link or the map file you committed:** See the Future-State Journey Map below.

## Future-State Journey Map: the Real-Time Dispatcher with RouteLogic Velocity

```
 ┌──────────────┐   ┌──────────────┐   ┌──────────────┐   ┌──────────────┐
 │ 1. OPEN THE  │──▶│ 2. SPOT THE  │──▶│ 3. REASSIGN  │──▶│ 4. CONFIRM   │
 │    BOARD     │   │    PROBLEM   │   │    LIVE      │   │    DELIVERY  │
 ├──────────────┤   ├──────────────┤   ├──────────────┤   ├──────────────┤
 │ Live driver  │   │ Late stop    │   │ Few taps;    │   │ Driver taps  │
 │ status, no   │   │ visible on   │   │ driver gets  │   │ delivered;   │
 │ 20-60 min    │   │ the board,   │   │ a push alert │   │ board shows  │
 │ lag          │   │ not via text │   │ in seconds   │   │ it live      │
 ├──────────────┤   ├──────────────┤   ├──────────────┤   ├──────────────┤
 │ Feels:       │   │ Feels:       │   │ Feels:       │   │ Feels:       │
 │ Trusting     │   │ In control   │   │ Confident    │   │ Certain      │
 ├──────────────┤   ├──────────────┤   ├──────────────┤   ├──────────────┤
 │ Kills:       │   │ Kills:       │   │ Kills:       │   │ Kills: check │
 │ WhatsApp     │   │ finding out  │   │ follow-up    │   │ -in calls,   │
 │ roll call    │   │ from texts   │   │ texts        │   │ stops aloud  │
 └──────────────┘   └──────────────┘   └──────────────┘   └──────┬───────┘
        ▲                                                         │
        └────────── repeats for every disruption, all shift ──────┘
```

### Stages

1. **Open the Board**
   - **User action:** Opens the board at shift start → sees where every driver actually is.
   - **Internal state:** Trusts the board over WhatsApp → plans the shift from one screen.
   - **Pain point addressed:** Live status replaces the 20–60 minute lag and stale "in progress" stops.
2. **Spot the Problem**
   - **User action:** Sees a late or failed stop on the board → acts before customers call.
   - **Internal state:** Feels ahead of problems → stops chasing drivers for updates.
   - **Pain point addressed:** Issues surface in RouteLogic, not through driver texts and WhatsApp threads.
3. **Reassign Live**
   - **User action:** Reassigns stops in a few taps → driver gets a push alert immediately.
   - **Internal state:** Knows the change landed → no need to message the driver too.
   - **Pain point addressed:** Changes arrive in seconds, not 8–15 minutes, so drivers don't drive wrong ways.
4. **Confirm Delivery**
   - **User action:** Driver taps delivered once → board updates live for the dispatcher.
   - **Internal state:** Certain the stop is done → moves on to the next disruption.
   - **Pain point addressed:** No check-in calls, and no reading stops aloud after driver app crashes.

> "Live" in Stage 1 and "seconds" in Stage 3 are targets, not research findings; the baselines are a 20–60 minute status lag and an 8–15 minute reassignment delay. The real targets are set in Module 3 (Hypothesis & Success Metrics).

### Competitive advantages over the manual workaround

1. **Live, not lagging:** The board reflects reality; WhatsApp depends on drivers remembering to reply.
2. **One system of record:** Every change is captured in RouteLogic instead of lost in chat threads.
3. **Dispatcher time back:** No double-messaging, roll calls, or reading stops aloud to stranded drivers.
