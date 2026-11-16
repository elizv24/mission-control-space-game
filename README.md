# MISSION CONTROL — Design. Launch. Fly.

**MISSION CONTROL** is a browser-based space mission design and simulation game created for the **NASA Space Apps Challenge 2026**, under the **Space Game Design** challenge track.

Players take the role of a mission-planning team: choose science objectives and a destination, assemble a spacecraft within budget and mass limits, select a launch vehicle and orbit, and then operate the mission through a sequence of interactive challenges. The goal is to return as much science as possible while keeping the spacecraft operational.

> This project is an independently developed hackathon submission. It is not an official NASA product and is not endorsed by or affiliated with NASA.

## Overview

The game turns the trade-offs involved in planning a space mission into a playable experience. Players must balance science return, spacecraft mass, power generation, data capacity, launch costs, communications and mission risk.

### Mission-planning flow

1. **Choose a mission and science goals** — select up to two objectives and a destination.
2. **Choose the crew and difficulty** — play solo or with up to four players, assign crew roles, and select Easy, Normal or Hard.
3. **Build the spacecraft** — install instruments and spacecraft subsystems while managing funds, mass, power generation and power consumption.
4. **Configure launch** — choose a launch vehicle, orbit and ground communications network.
5. **Operate the mission** — complete a sequence of monthly minigames and respond to mission events for a 12-month simulation.
6. **Review the results** — inspect the science score, mission rating, performance breakdown and crew report.

## Destinations

The game includes four mission scenarios:

- **Moon Watcher** — a lower-risk lunar science mission.
- **CubeSat 101** — a compact, budget-constrained spacecraft mission.
- **Mars Scout** — a longer-range mission with a larger science opportunity.
- **Jupiter Probe** — a high-risk, high-reward mission involving a challenging radiation environment.

These are game scenarios and simplified abstractions, not operational mission plans.

## Science objectives

Choose up to two objectives:

- Oceans
- Atmosphere
- Ice
- Land
- Deep Space

Matching instruments to selected objectives increases science scoring. The game also displays examples of related NASA missions as comparison references; these comparisons are educational context, not official NASA mission endorsements or engineering equivalence claims.

## Spacecraft components

Build a spacecraft from a selection of components, including:

- Cameras and high-definition cameras
- Spectrometer
- Radar
- Telescope
- Solar array and battery pack
- High-gain communications dish
- Onboard CPU
- Attitude control
- Whipple shield
- Spare kit

Each component affects one or more design constraints, such as mass, cost, power use, power generation, science output, data production or buffer capacity.

## Launch and orbit configuration

Select from three launch-vehicle capacity tiers:

- Scout — 500 kg
- Runner — 800 kg
- Titan — 1,200 kg

Choose an orbit based on the trade-off between science return, power requirements, data-buffer capacity and risk:

- Low Orbit
- Polar Orbit
- Deep Ellipse

Choose a ground network to affect downlink performance and data-buffer capacity.

## Gameplay

A mission runs for **12 simulated months**. Each month presents a set of tasks based on the spacecraft and mission state. The minigames include:

| Activity | What the player does |
| --- | --- |
| Collect Data | Pilot the spacecraft to catch science particles. |
| Spectrum ID | Identify a sample by matching its emission-spectrum lines. |
| Send Data Home | Aim and send data packets to Earth's moving communications dish. |
| Signal Decode | Memorise and repeat a signal pattern to upload buffered data. |
| Balance Power | Counter array drift and keep the power beam in its target zone. |
| Power Routing | Rotate conduit tiles to connect the solar feed to the battery. |
| Save the Craft | Aim the point-defence system at incoming meteors. |
| Repairs | Spend mission funds to restore damaged systems or continue with reduced capability. |

Other mission features include:

- **Crew roles:** Commander for solo play; specialised Science, Communications, Power, Systems and Defense roles for multiplayer.
- **Mission Control boosts:** non-active crew members can assist during a mission.
- **Crew decisions:** choose how to respond to mission crises.
- **Difficulty settings:** adjust available funds, score targets and meteor pressure.
- **Mission review:** see the final score, star rating, score analysis and crew performance.
- **Design sharing:** export a spacecraft configuration as a short code and import another player's design.
- **Local high scores:** recent runs and top scores are stored in the current browser.

## Controls

The game supports keyboard, pointer and touch-style interactions where applicable.

- **Arrow keys:** move or balance systems during the relevant minigames.
- **Mouse / pointer / drag:** steer, aim and interact with the simulation.
- **Space / click:** fire or confirm actions in the relevant phases.
- Use the on-screen **?** help control for phase-specific instructions.
- Use the sound control in the top bar to mute or enable game audio.

The game displays the required controls before each minigame.

## Built with

- **HTML5** — application structure
- **CSS3** — responsive layout, interface styling and animations
- **JavaScript** — game state, mission logic, scoring and interactions
- **HTML Canvas** — starfield, spacecraft visuals and minigame rendering
- **Web Audio API** — generated interface and gameplay sound effects
- **localStorage** — local mission history and high scores

The project is contained in a single HTML file and does not require a package manager, build step or external JavaScript framework.

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern web browser.
3. Select a crew size, difficulty, science objectives and destination.
4. Build and configure your spacecraft, then launch the mission.

For the best experience, use an up-to-date version of Chrome, Edge, Firefox or Safari.

### Optional: run with a local web server

From the project directory, run:

```bash
python -m http.server 8000
```

Then open [http://localhost:8000/index.html](http://localhost:8000/index.html).

## Data and scientific context

Mission names, component specifications, budgets, scoring rules and simulation outcomes are simplified game-design values. They are intended to make mission-planning concepts understandable and playable; they should not be interpreted as real spacecraft specifications, NASA cost estimates, launch performance data or mission predictions.

NASA mission names shown in the game are used as educational comparison references. For authoritative mission information, consult NASA's official websites:

- [NASA](https://www.nasa.gov/)
- [NASA Science](https://science.nasa.gov/)
- [NASA Solar System Exploration](https://science.nasa.gov/solar-system/)

## NASA Space Apps Challenge

This project was created for the **NASA Space Apps Challenge 2026**. The team identifies its challenge track as **Space Game Design**.

- [NASA Space Apps Challenge — official website](https://www.spaceappschallenge.org/)

The README describes the submitted implementation. For the official challenge brief, judging criteria and submission requirements, refer to the challenge page on the Space Apps website.

## Project structure

```text
.
├── MissionControl.html   # Complete browser game (HTML, CSS and JavaScript)
├── README.md             # Project overview and instructions
└── LICENSE               # MIT License
```

## Known scope and limitations

- The game is a self-contained educational simulation, not a physics-accurate spacecraft simulator.
- Mission progression, budgets, component statistics, risk and scoring are governed by game logic.
- High scores are stored locally in the browser. They are not synchronised between devices.
- Design codes share a configuration; they do not transfer mission history or scores.
- The game does not connect to NASA systems or fetch live spacecraft telemetry.

## Contributing

Suggestions, bug reports and improvements are welcome. If you plan to contribute, please describe the issue or proposed change clearly and test the game in a modern browser.

## License

This project is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.
