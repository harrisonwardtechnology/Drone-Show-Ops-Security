# The Ground Station

> [!NOTE]
> Draft. One laptop commands the sky. Treat it accordingly.

**Purpose.** Securing the ground control station, the single most consequential computer in the operation, the [engineering workstation of the flying plant](https://github.com/HarrisonWard/OT-Security-for-IT-People).

## Dedicated Hardware, Boring on Purpose

The GCS is a show instrument, not a crew laptop: dedicated machines that run the control software and nothing else, no email, no browsing, no side duties between shows. The reasoning is the [admin-account logic](https://github.com/HarrisonWard/Least-Privilege-and-RBAC) at altitude: phishing lands where email lands, so the machine that commands the fleet must not be the machine that reads the internet. Disk encryption on, screen lock on, updates applied on the operator's tested schedule rather than auto-landing mid-tour, and a hardened spare imaged identically, because a dead GCS an hour before doors is otherwise a cancelled show.

## Access, Named and Narrow

Named accounts per crew member on the control software where it supports them, no shared logins, and the roster of who can command a show kept as deliberately as [any admin count](https://github.com/HarrisonWard/Least-Privilege-and-RBAC): pilots and designated backups, and nobody else, not the client, not the venue, not the videographer who would like a better angle. Physical control matters as much as logical: the GCS travels in custody, sits behind the crew perimeter on site, and is never left logged in and unattended in a production trailer full of strangers, which describes every production trailer.

## The Show File Pipeline

Choreography moves from design workstation to GCS through a controlled path: versioned, integrity-checked, transferred on trusted media or connections, with the final loaded version verified against the version that rehearsed. Last-minute changes are where discipline dies, the 6pm music edit, the hurried re-export, so the rule is written in advance: what changes are permitted inside the final hours, who approves them, and what triggers a full re-verification instead. A show file is [production code that flies](https://github.com/HarrisonWard/Security-Program-Starter/blob/main/policies/21-secure-development.md); ship it like you mean it.

## Backups and the Second Site

The GCS holds the show, the fleet configuration, and the logs that reconstruct any incident: all of it backed up before and after every show night, off the machine, per the [backup discipline](https://github.com/HarrisonWard/Security-Program-Starter/blob/main/policies/09-backup-recovery.md) everything else in this library preaches. The logs deserve respect on their own, they are your flight recorder, your dispute evidence when a client claims a drift that did not happen, and your [incident reconstruction](show-day.md) when one did.

## Connectivity, Minimal and Deliberate

The GCS network posture is allowlist thinking: the links the show requires, and nothing else, no venue guest wifi, no hotspot conveniences, no remote-support tunnel left warm because the vendor once asked. Where the platform vendor genuinely needs remote access for support, it follows the [same rules as any integrator](https://github.com/HarrisonWard/OT-Security-for-IT-People): on-request, logged, disabled after, owned by a name.

---

**Owner:** _name a person_
**Last Reviewed:** not yet
**Review Cycle:** annual, and at every platform change
