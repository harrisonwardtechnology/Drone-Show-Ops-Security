# The Threat Model

> [!NOTE]
> Draft. Ranked by consequence, not by how cinematic the attack sounds. Defensive framing throughout, this page names what to protect, never how to break it.

**Purpose.** What can actually go wrong with a drone show, so the [ground station](the-ground-station.md), [fleet](the-fleet.md), and [show day](show-day.md) pages have something to defend against.

## The Consequence Ladder

Order everything by outcome, worst first: people hurt, then aircraft where they must not be, airports, roads, restricted airspace, then the show fails publicly, then data and reputation. The ladder matters because controls compete for attention, and the flashy threat is rarely the top rung: most real drone show incidents to date are operational, weather pushed, batteries misjudged, links degraded, not adversarial, and a security program that forgets that balance protects against movie plots while the ordinary failure modes fly the show.

## The Command Channel

One ground station commanding hundreds of aircraft makes the C2 link the crown jewel: whoever influences it influences the sky. The defensive posture is the [OT lesson](https://github.com/HarrisonWard/OT-Security-for-IT-People) verbatim, the network is the authentication, so the link gets encryption and authentication where the platform supports it, spectrum planning where it cannot, and above all a failsafe posture defined in advance: what every airframe does on link loss, hold, land, return home, decided and tested before there is a crowd to decide over.

## Position Truth

The fleet believes what GPS tells it, and urban RF environments degrade that truth accidentally more often than anyone attacks it deliberately. The defense is not exotic: know your site's RF and GPS reality from the [site survey](show-day.md), set geofence and altitude floors that assume degradation, and treat position-confidence warnings as abort criteria rather than nuisances. Interference of any flavor, deliberate or ambient, produces the same operational question, do we trust the sky picture, and the answer must be rehearsed, not improvised.

## The Supply Chain That Flies

Every airframe runs firmware, and one update reaches the whole fleet: your own [fleet management](the-fleet.md) is the supply chain risk. Staged rollouts, verified sources, and a known-good version to fall back to are the whole defense, plus the quieter half, the show file itself, the choreography that tells a thousand aircraft where to be, which deserves the same integrity care as any production deployment, versioned, checksummed, and loaded through a controlled path.

## The Human Ring

Insider and social paths mirror every other industry: crew access to the ground station, the vendor tech with a laptop, the enthusiastic volunteer nobody vetted, the USB stick of last-minute music changes. The [show-day roles](show-day.md) and simple crew discipline, named accounts, no shared logins on the GCS, physical control of the command hardware, close most of it, and the [venue's questions](for-venues.md) exist because operators who cannot answer them have not closed any of it.

---

**Owner:** _name a person_
**Last Reviewed:** not yet
**Review Cycle:** annual, and after any industry incident
