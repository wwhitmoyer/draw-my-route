# Draw My Route

**Draw My Route** is an Android tablet application that helps bus drivers create accurate, practical turn-by-turn directions from the route they actually drive.

A driver draws a route directly on a map with a stylus. The app matches that drawing to real roads, generates turn-by-turn directions, and then guides the driver through each detected turn for review. Once approved, the completed route can be shared as a clean PDF by email.

## Why it exists

Assigned routes and existing turn-by-turn instructions are not always accurate, efficient, or safe for a bus. Drivers have valuable local knowledge about the roads they use every day. Draw My Route makes it easy to capture that knowledge, correct a route, and produce a clear, reusable route document.

## How it works

1. **Draw** — The driver opens a map and traces the route with a finger or stylus.
2. **Match** — The app aligns the drawn trace with the road network and generates an editable route.
3. **Review** — The driver verifies every turn on the map, confirms it, or corrects the route where needed.
4. **Approve** — The app saves an approved, versioned route with notes and safety information.
5. **Share** — The app creates a turn-by-turn PDF and opens the device's email/share workflow.

## Planned first-release features

- Tablet-first Android interface with stylus drawing
- Map-based route drawing, editing, erase, undo, and redo
- Road matching and generated turn-by-turn directions
- Turn-by-turn map review with confirmation and correction
- Distance and estimated travel time between turns
- Driver notes, route versions, and assigned-route comparison
- Bus-safety warnings for restrictions such as clearance, weight, tight turns, or prohibited roads
- Approved turn-by-turn PDF generation and email sharing

## Technology direction

The first release is planned as a native Android application built with Kotlin. Mapbox is the intended mapping foundation for map display, drawn-route matching, and directions.

## Project status

This repository currently contains the product definition and roadmap. The next step is to define the first-release user flows and screen designs before implementation begins.

- [Read the product roadmap](docs/ROADMAP.md)

## Contributing

This is an early-stage project. Product feedback is especially valuable from bus drivers, dispatchers, and transportation operations staff who work with real-world route constraints.
