# Drone Show Ops Security

Operational security for drone light shows: a thousand networked flying computers, a crowd underneath, and the ground station that commands it all. Nobody has published this playbook. Here it is.

A drone show is an OT environment that flies. The fleet is the plant floor, the ground control station is the engineering workstation, the RF links are the network, and the audience below is why every decision defers to safety. The industry has grown from novelty to headline act in a few years, and its security practices are wherever each operator happened to land. This repo is the baseline: for show operators who fly, and for the venues and brands who hire them.

---

## The Priority Order

Same [inversion as any plant](https://github.com/HarrisonWard/OT-Security-for-IT-People): safety, then the show, then everything else, and safety is a wall, not a tiebreaker. A scrubbed show is a refund. A drone in the crowd is the end of the company, and possibly worse. Every page here is written under that ranking.

**Security Is a Team Sport**, and on show night the team is pilots, spotters, venue security, and a crowd that never knows any of it happened. More in [PRINCIPLES.md](https://github.com/HarrisonWard/.github/blob/main/PRINCIPLES.md).

---

## Who It's For

- Drone show operators, from three-person outfits to arena-scale fleets
- Venues, municipalities, and brands hiring a show and wondering what to ask
- Event security teams with a new airborne thing on the risk register
- Aviation-adjacent security folks who suspect, correctly, that this niche has no literature

## Who It's Not For

Counter-drone and C-UAS practitioners, that is defense against hostile drones, a different field with different lawyers.

Anybody seeking exploitation detail. This repo is defensive by design: what to protect and verify, never how to attack a show. Requests otherwise get the [same answer the OT repo gives](https://github.com/HarrisonWard/OT-Security-for-IT-People): no.

---

## What's in Here

| File | What it is |
|---|---|
| `the-threat-model.md` | What can actually go wrong, ranked by consequence |
| `the-ground-station.md` | The crown jewel: one laptop commands the sky |
| `the-fleet.md` | Firmware, batteries, chain of custody, and the show file |
| `show-day.md` | The runbook: roles, abort authority, and the incident nobody claps for |
| `for-venues.md` | The questions to ask an operator before they fly over your crowd |

The 15 distilled lessons that seeded this repo live in the [Security-Lessons drone collection](https://github.com/HarrisonWard/Security-Lessons/blob/main/collections/drone-shows.md).

---

## The Regulatory Line

Your aviation authority outranks this repo everywhere it speaks. In the US that means the FAA: show operations run under specific waivers and authorizations, and the paperwork, airspace, and pilot requirements are aviation law, not security guidance. This repo covers the security of the operation, not the legality of the flight, and any conflict resolves in favor of the regulator and the safety case you filed.

---

## What This Isn't

Not aviation law, not a flight operations manual, not a substitute for your manufacturer's guidance or your own safety management system. Not counter-drone. And not a place to learn how to interfere with anybody's show.

Nothing here comes from a client engagement.

---

## Contributing

Want: operator field notes, scrubbed. Venue-side experiences. Near-miss patterns the industry should learn from, anonymized to the lesson.

Nothing attack-enabling, nothing show-identifiable without permission. See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Use it, adapt it, fly safer with it. Just say where you got it.

© 2026 Harrison Ward

---

## Me

Cyber risk and technology exec with a foot in drone show operations, which is how this repo exists: the security literature for this industry was a blank page, and I happened to be standing on both sides of it.

[github.com/HarrisonWard](https://github.com/HarrisonWard) · [LinkedIn](https://linkedin.com/in/harrisonaward)

---

*Published under [these principles](https://github.com/HarrisonWard/.github/blob/main/PRINCIPLES.md). Security Shouldn't Be Paywalled.*
