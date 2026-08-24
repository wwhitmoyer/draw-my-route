# Draw My Route — Product Roadmap

## Product vision

Draw My Route is an Android-only, tablet-and-stylus application for bus drivers. A driver can either sketch a route directly on a map or record the route while riding in the bus with the tablet's GPS. The app matches the resulting trace to roads, produces turn-by-turn directions, and lets the driver review and approve the result before sharing it.

The product should prioritize driver control, clear map-based verification, bus-safe routing context, and a dependable record of every approved route.

## Phase 1 — Product definition

- Define the two primary route-capture workflows: draw a route and record a route while driving.
- Document driver, dispatcher, and administrator needs without expanding beyond Android tablets.
- Establish route, GPS trace, turn, segment, note, restriction, assigned-route, and version data models.
- Define success criteria for road matching, GPS capture quality, travel estimates, review accuracy, and PDF output.
- Identify map, routing, geocoding, location, and email integrations, including cost, privacy, battery, and offline constraints.

**Outcome:** An agreed product specification, initial UX flow, technical architecture, and acceptance criteria.

## Phase 2 — Android and route-capture foundation

- Build a tablet-first Android application with responsive landscape and portrait layouts.
- Support precise stylus drawing, erasing, undo/redo, panning, and zooming without gesture conflicts.
- Add GPS route recording for a tablet carried on the bus, including start, pause, resume, finish, and recovery controls.
- Let drivers mark stops, detours, or issues during a recording and clearly surface weak or missing GPS segments.
- Display captured traces over the map and save editable route drafts locally.
- Add route naming, basic metadata, autosave, recovery, and draft management.
- Establish location permission, accessibility, crash-reporting, and automated-test foundations.

**Outcome:** Drivers can reliably draw or record, edit, save, reopen, and manage route captures on an Android tablet.

## Phase 3 — Map matching and directions

- Convert drawn and GPS-recorded traces into road-matched routes while preserving the driver's intended path.
- Generate ordered turn-by-turn directions and identify each detected turn on the map.
- Calculate distance and estimated road travel time between consecutive turns.
- Show confidence or ambiguity where a trace could match more than one road, especially in areas with weak GPS.
- Allow drivers to correct the matched path and recalculate affected directions and estimates.
- Capture bus-safety restrictions and warnings, such as height, weight, width, turn, and road-access concerns.

**Outcome:** A route capture becomes an editable, map-aligned route with usable directions, segment distances, travel estimates, and safety context.

## Phase 4 — Review and approval

- Guide the driver through every detected turn with synchronized map and instruction views.
- Support editing instructions, moving or adding turns, correcting geometry, and attaching notes.
- Compare the proposed route with an imported or assigned route and clearly highlight differences.
- Require acknowledgement of unresolved matching ambiguities, GPS gaps, and flagged bus-safety restrictions.
- Preserve immutable versions with timestamps, authorship, notes, and approval status.
- Provide a final approval summary before a route is marked ready to share.

**Outcome:** Every approved route has been reviewed turn by turn, reconciled as needed, and preserved as an auditable version.

## Phase 5 — PDF and email sharing

- Generate a polished turn-by-turn PDF from an approved route.
- Include route identity, version, approval details, capture source, ordered directions, segment distance and estimated time, notes, and safety flags.
- Add useful map snapshots where they improve turn clarity.
- Preview the PDF before sharing and prevent unapproved drafts from being presented as final.
- Share the approved PDF through Android's email/share workflow with a clear filename and subject.

**Outcome:** Drivers can confidently email a consistent, readable, approved route document from the tablet.

## Phase 6 — Operational improvements

- Improve matching accuracy and review speed using real-world feedback and anonymized diagnostics.
- Add configurable restriction types, organization templates, approval policies, and route libraries.
- Strengthen offline behavior, background synchronization, import/export, backup, and recovery.
- Add change summaries, richer assigned-route comparisons, search, filtering, and version restoration.
- Improve GPS reliability, battery use, accessibility, security, privacy, and fleet-scale device management.
- Evaluate optional dispatcher collaboration only after the core driver workflow is dependable.

**Outcome:** The product becomes easier to operate, administer, support, and scale without compromising driver verification.
