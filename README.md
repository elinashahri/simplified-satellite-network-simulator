# simplified-satellite-network-simulator

A modular simulation framework for dynamic Low Earth Orbit (LEO) satellite networks.

This project models time-evolving satellite constellations, inter-satellite links (ISLs), temporary links (TLs), ground station connectivity, and propagation-delay-based routing under stochastic traffic conditions.

The simulator is designed as a research-oriented framework for studying dynamic topology effects in large-scale LEO networks.

🚀 Key Features

Dynamic LEO constellation generation based on orbital mechanics

Intra-orbit and inter-orbit ISL construction

Temporary inter-satellite link (TL) modeling

Propagation-delay-based weighted routing (Dijkstra)

Ground station to nearest satellite mapping

Poisson-based GS-to-GS traffic generation

Multi-timeslot simulation support

🏗 Architecture Overview

The simulator follows a layered design:

Constellation Layer
Orbital modeling and time-dependent satellite positioning.

Topology Layer
Construction of intra-orbit, inter-orbit, and temporary ISLs.

Network Layer
Weighted graph construction and shortest-path routing.

Traffic Layer
Stochastic GS-to-GS demand modeling (hot/cold differentiation).

Simulation Engine
Multi-timeslot execution and performance metric collection.

This modular structure enables controlled experimentation and future extensions.


The output includes:

Number of flows

Successful routes

Blocking rate

Average delay

Average hop count

📊 Output Metrics

For each simulation time slot, the following metrics are computed:

Total traffic demands

Successfully routed flows

Blocking rate (%)

Average end-to-end delay (seconds)

Average hop count

📌 Project Status

Status: Ongoing research project.

A journal/conference manuscript based on extended versions of this simulator is currently under preparation.

Advanced physical-layer modeling and adaptive routing extensions will be released after formal publication.

🔭 Future Work

Planned extensions include:

Capacity-aware routing

Adaptive physical-layer modeling

Resource allocation under dynamic traffic

Scalability optimization for large constellations

Integration of advanced performance metrics

## Requirements

- Python 3.9+
- Jupyter Notebook or Google Colab
- numpy
- pandas
- scipy
- scikit-learn
