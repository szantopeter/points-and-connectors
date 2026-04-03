# Points & Connections

An interactive visualisation that demonstrates how the number of connections between points grows **quadratically** — and how introducing intermediate **hub rings** dramatically reduces that number.

**Live demo: https://szantopeter.github.io/points-and-connectors/**

## What it shows

When every point connects directly to every other point, the number of connections follows the formula **n × (n − 1) / 2**, which grows as O(n²). With 30 points that's already 435 connections; with 60 it's 1,770.

By routing connections through one or more intermediate rings of hub points, the total connection count drops sharply. Each outer point connects only to its nearest hub, and hubs connect to the next ring inward — with only the innermost ring fully meshed.

## Features

- Adjust **outer points** (up to 60) with a slider or +/− buttons (hold to repeat)
- Add up to **5 inner rings**, each independently configurable
- Per-ring **auto-increment** to animate the effect
- Live stats showing total connections and connections saved vs direct
- Colour-coded rings for easy visual distinction
