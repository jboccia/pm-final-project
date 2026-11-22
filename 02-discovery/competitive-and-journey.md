# Competitive Analysis & Journey Map

> **Module 2 · Lab 2 — ★ Deliverable 2.** Repo file `02-discovery/competitive-and-journey.md` — part of your submission.
> Do the lab in the **Module 2 · Exercise 2 Guide** (linked from the Module 2 deck), then click **⬇ Download .md** — it saves as this exact file. Commit it here.
> It becomes the **Competitive Analysis & Journey Map** slide of your Module 6 final deck. Builds on your `ai-synthesis.md` and your Module 1 `problem-hook.md`.

## Responses

- **Role, who are you solving for?:** The Frontline Delivery Driver: a driver on a long, often rural or low-signal route who uses the app dozens of times a day to start routes, mark deliveries, and upload proof of delivery.
- **Goal, what is this user ultimately trying to achieve?:** Get route changes instantly and finish each stop in one quick action, without wondering whether the app saved it.
- **Friction, the main barrier (moment of misery) stopping them:** Reassignments take 8 to 15 minutes to arrive, with no push notification, so drivers drive the wrong way on old routes. On routes over about 40 stops, the app can crash on Android and lose the rest of the route. One driver lost about twenty minutes while the office read the stops aloud. Five of seven focus-group drivers carry a paper manifest in case this happens.
- **External tools the user is forced to use:** Paper manifests, morning screenshots of the stop list, phone calls to the office, and texts or a WhatsApp group with dispatchers.
- **The process, the 3–5 manual steps they take:**
  1. Carry a paper manifest and screenshot the stop list before leaving, in case the app crashes or loses signal.
  2. When the app crashes on a 40+ stop route, switch to the paper list or call the office to have stops read aloud.
  3. Text the dispatcher or post in WhatsApp to confirm route changes, because in-app reassignments arrive 8 to 15 minutes late.
  4. Retake proof-of-delivery photos repeatedly, because about 35% of uploads fail silently on weak signal.
- **Core frustration, where the process feels most "broken":** The app fails exactly when the driver needs it most: mid-route on a long or low-signal route. Every backup (paper, screenshots, WhatsApp) is frozen or off-platform, so the driver still acts on stale information and RouteLogic stops being the system of record.
- **The evidence, a quote or behavior from the research:** Five of seven focus-group drivers carry a paper manifest in case the app dies; one driver lost about twenty minutes after a mid-route crash while the office read stops aloud; dispatchers describe a WhatsApp group as the "real system."
- **Journey map, a shareable link or the map file you committed:** See the Future-State Journey Map below.

## Future-State Journey Map: the Frontline Delivery Driver with RouteLogic Velocity

```
 ┌──────────────┐   ┌──────────────┐   ┌──────────────┐   ┌──────────────┐
 │ 1. START     │──▶│ 2. DRIVE     │──▶│ 3. RE-ROUTE  │──▶│ 4. COMPLETE  │
 │    ROUTE     │   │    THE ROUTE │   │    LIVE      │   │    THE STOP  │
 ├──────────────┤   ├──────────────┤   ├──────────────┤   ├──────────────┤
 │ One tap from │   │ Stable past  │   │ Push alert,  │   │ One tap,     │
 │ home screen; │   │ 40 stops;    │   │ new route    │   │ photo queued,│
 │ route cached │   │ works with   │   │ arrives in   │   │ dispatcher   │
 │ offline      │   │ no signal    │   │ seconds      │   │ sees it live │
 ├──────────────┤   ├──────────────┤   ├──────────────┤   ├──────────────┤
 │ Feels:       │   │ Feels:       │   │ Feels:       │   │ Feels:       │
 │ Prepared     │   │ Secure       │   │ Informed     │   │ Certain      │
 ├──────────────┤   ├──────────────┤   ├──────────────┤   ├──────────────┤
 │ Kills: paper │   │ Kills: call  │   │ Kills: wrong │   │ Kills: texts │
 │ manifest,    │   │ to office,   │   │ -way driving,│   │ to dispatch, │
 │ screenshots  │   │ lost route   │   │ WhatsApp     │   │ photo retakes│
 └──────────────┘   └──────────────┘   └──────────────┘   └──────┬───────┘
        ▲                                                         │
        └───────────── repeats for every stop, all day ───────────┘
```

### Stages

1. **Start Route**
   - **User action:** Taps Start Route on a simplified home screen → route loads in one step.
   - **Internal state:** Opens the app, not a paper manifest → starts the day prepared.
   - **Pain point addressed:** Stop list saved for offline use → no screenshots or paper backup needed.
2. **Drive the Route**
   - **User action:** Works through 40+ stops on Android → app stays stable and keeps the route.
   - **Internal state:** Stops worrying about crashes → focuses on driving, not on backup plans.
   - **Pain point addressed:** Crash protection and offline mode → no twenty-minute call for stops read aloud.
3. **Re-Route Live**
   - **User action:** Gets a push notification when reassigned → updated route appears straight away.
   - **Internal state:** Trusts the app over WhatsApp → acts on the change without double-checking.
   - **Pain point addressed:** Changes arrive in seconds, not 8–15 minutes → no more driving the wrong way.
4. **Complete the Stop**
   - **User action:** Marks delivered with one tap → photo uploads automatically when signal returns.
   - **Internal state:** Sees a clear "saved" confirmation → moves on without retaking photos.
   - **Pain point addressed:** Replaces 3 taps across 3 screens, silent upload failures and status texts to dispatch.

> "Seconds" in Stage 3 is a target, not a research finding; the baseline is 8–15 minutes. The real target is set in Module 3 (Hypothesis & Success Metrics).

### Competitive advantages over the manual workaround

1. **Always current:** Paper and screenshots are frozen at dawn; Velocity updates live, even mid-route.
2. **One system of record:** Every stop is captured in RouteLogic, so the dispatcher board becomes trustworthy again.
3. **No extra people pulled in:** Drivers recover on their own, so dispatchers coordinate instead of reading stops aloud.
