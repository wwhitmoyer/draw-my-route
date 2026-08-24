# Draw My Route — Product Roadmap

## Product vision

Draw My Route is an Android-only, tablet-and-stylus application for bus drivers. A driver sketches a route directly on a map, the app matches that drawing to roads and produces turn-by-turn directions, and the driver reviews and approves the result before sharing it.

The product should prioritize driver control, clear map-based verification, bus-safe routing context, and a dependable record of every approved route.

## Phase 1 — Product definition

- Define the primary workflow: create, review, correct, approve, and share a route.
- Document driver, dispatcher, and administrator needs without expanding beyond Android tablets.
- Establish route, turn, segment, note, restriction, assigned-route, and version data models.
- Define success criteria for road matching, travel estimates, review accuracy, and PDF output.
- Identify map, routing, geocoding, and email integrations, including cost and offline constraints.

**Outcome:** An agreed product specification, initial UX flow, technical architecture, and acceptance criteria.

## Phase 2 — Android and stylus foundation

- Build a tablet-first Android application with responsive landscape and portrait layouts.
- Support precise stylus drawing, erasing, undo/redo, panning, and zooming without gesture conflicts.
- Display the drawn path over the map and save editable route drafts locally.
- Add route naming, basic metadata, autosave, recovery, and draft management.
- Establish accessibility, permission, crash-reporting, and automated-test foundations.

**Outcome:** Drivers can reliably draw, edit, save, reopen, and manage route sketches on an Android tablet.

## Phase 3 — Map matching and directions

- Convert the hand-drawn path into a road-matched route while preserving the driver's intended path.
- Generate ordered turn-by-turn directions and identify each detected turn on the map.
- Calculate distance and estimated road travel time between consecutive turns.
- Show confidence or ambiguity where the sketch could match more than one road.
- Allow drivers to correct the matched path and recalculate affected directions and estimates.
- Capture bus-safety restrictions and warnings, such as height, weight, width, turn, and road-access concerns.

**Outcome:** A route sketch becomes an editable, map-aligned route with usable directions, segment distances, travel estimates, and safety context.

## Phase 4 — Review and approval

- Guide the driver through every detected turn with synchronized map and instruction views.
- Support editing instructions, moving or adding turns, correcting geometry, and attaching notes.
- Compare the proposed route with an imported or assigned route and clearly highlight differences.
- Require acknowledgement of unresolved matching ambiguities and flagged bus-safety restrictions.
- Preserve immutable versions with timestamps, authorship, notes, and approval status.
- Provide a final approval summary before a route is marked ready to share.

**Outcome:** Every approved route has been reviewed turn by turn, reconciled as needed, and preserved as an auditable version.

## Phase 5 — PDF and email sharing

- Generate a polished turn-by-turn PDF from an approved route.
- Include route identity, version, approval details, ordered directions, segment distance and estimated time, notes, and safety flags.
- Add useful map snapshots where they improve turn clarity.
- Preview the PDF before sharing and prevent unapproved drafts from being presented as final.
- Share the approved PDF through Android's email/share workflow with a clear filename and subject.

**Outcome:** Drivers can confidently email a consistent, readable, approved route document from the tablet.

## Phase 6 — Operational improvements

- Improve matching accuracy and review speed using real-world feedback and anonymized diagnostics.
- Add configurable restriction types, organization templates, approval policies, and route libraries.
- Strengthen offline behavior, background synchronization, import/export, backup, and recovery.
- Add change summaries, richer assigned-route comparisons, search, filtering, and version restoration.
- Improve performance, battery use, accessibility, security, privacy, and fleet-scale device management.
- Evaluate optional dispatcher collaboration only after the core driver workflow is dependable.

**Outcome:** The product becomes easier to operate, administer, support, and scale without compromising driver verification.
