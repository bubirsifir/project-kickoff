# Platform and Product-Surface Routing

Resolve platforms after understanding the user, problem, and usage context but before committing architecture.

## Separate three concepts

1. **Device:** phone, tablet, desktop, kiosk, television, wearable, or special hardware.
2. **Delivery platform:** responsive web, PWA, iOS, Android, desktop app, browser extension, API, or embedded experience.
3. **Product surface:** public website, customer product, employee app, admin console, partner portal, support console, or developer API.

“Web + mobile” is ambiguous until all three are understood.

## Core questions

Ask only those not answered:

- Where will each user group use the product?
- Which devices and environments are primary rather than merely supported?
- Does mobile mean responsive web, installable PWA, or app-store distribution?
- Which device capabilities are essential: push, camera, location, Bluetooth, NFC, biometrics, contacts, calendar, background tasks, or offline storage?
- Must the product be discoverable in App Store or Google Play?
- Can platforms be delivered in phases?
- Which surfaces share data, identity, roles, and workflows?

## Recommendation logic

Recommend responsive web first when rapid validation, broad access, simple updates, and ordinary browser capabilities dominate.

Consider PWA when installation, limited offline behavior, or a more app-like launch experience matters without requiring full store-native capabilities. Verify current platform limitations before promising specific behavior.

Consider cross-platform mobile when store distribution and mobile APIs matter, the experiences can largely share behavior, and a shared codebase fits the team.

Consider native apps when platform-specific performance, deep OS integration, complex background work, or distinct platform experiences justify the added cost.

Do not assume all platforms must launch together. Recommend phased delivery when it reduces risk without undermining the core use case.

## Surface matrix

Record each required surface:

| Surface | Primary user | Platform/device | Main job | Phase | Data shared with |
|---|---|---|---|---|---|
| Example: Staff console | Operations team | Responsive web/desktop | Manage accounts | MVP | Customer app |

## Architecture gate

Do not finalize framework, repository strategy, authentication topology, notification architecture, or release workflow until the priority surfaces and delivery sequence are confirmed.
