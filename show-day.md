# Show Day

> [!NOTE]
> Draft. The runbook. By show day, security is either already done or already absent; this page is about not undoing it.

**Purpose.** Roles, abort authority, and the operational security of the hours when the crowd is real.

## The Site Survey Came First

Show day inherits the survey: the RF environment mapped, GPS confidence characterized, geofences and altitude floors set against the site's actual geometry, crowd lines and exclusion zones agreed with the venue, and the failsafe behaviors, link loss, position loss, low battery, configured for this site, not the last one. The survey is where most show-day surprises go to die in advance, which is why it is a deliverable, not a walk.

## Roles, Named Out Loud

Before doors: who flies, who watches the sky, who watches the [ground station](the-ground-station.md), who owns the perimeter, and who speaks to the venue and, if needed, the public. Spotters are a security control, human eyes catching what telemetry cannot, and the GCS watch matters because show night is when a production trailer is busiest and least attended. One briefing, everyone hears the same plan, including the venue's security lead, whose radios and eyes are force multipliers if they know what abnormal looks like.

## Abort Authority, the Stop-the-Line Rule

The single most important sentence of the briefing: who can call an abort, and the answer includes the most junior spotter. Abort criteria are written, weather limits, loss counts, link degradation, position confidence, airspace intrusion, anything unexplained near the crowd line, and the culture rule is borrowed [straight from the plant floor](https://github.com/HarrisonWard/OT-Security-for-IT-People): a conservative abort is always right, nobody is ever second-guessed for calling one, and the show that scrubs safely gets rescheduled while the one that should have does not. Rehearse the abort like choreography, because it is.

## During the Show

Quiet discipline: the GCS crew flies, everyone else buffers them, no client requests, no last-minute creative thoughts, no handing the videographer a better angle inside the perimeter. Comms on the crew channel follow closed-loop habits, heard, repeated, done, and anything anomalous, unexpected aircraft, RF weirdness, a drone behaving oddly, goes to the abort-authority holder immediately rather than being diagnosed collaboratively while the clock runs. The [threat model's](the-threat-model.md) consequence ladder governs in real time: when in doubt, the crowd wins, the show loses, every time.

## When Something Happens Anyway

A drone down, a scrub, an intrusion: the incident rhythm is the [same one everywhere](https://github.com/HarrisonWard/IR-First-24-Hours), stabilize, preserve, log, then talk. Secure the aircraft and the scene, preserve GCS logs and telemetry untouched, one person keeps times, and the pre-agreed voice handles the venue and any public statement with [holding-statement discipline](https://github.com/HarrisonWard/IR-First-24-Hours), true, short, no speculation. Regulatory reporting obligations, if the event meets them, are aviation law and get handled per your ops manual, with the logs you preserved doing the talking. Then the after-action, within days, blameless, findings with owners, because the industry is young enough that every honest lesson written down makes the whole field safer.

---

**Owner:** _name a person_
**Last Reviewed:** not yet
**Review Cycle:** every show season
