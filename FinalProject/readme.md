# Urban Trash Collection Simulation with Agents - NetLogo

Final project for the **Multi-Agent Systems** course, developed using **NetLogo**. The main goal of this project is to model and simulate the **accumulation of trash in urban storm drains** and its impact on **flooding**, using agents (garbage collectors) to mitigate this issue.

## 🧠 Simulation Goal

This simulation represents a **simplified urban environment** with streets, buildings, and storm drains. It focuses on showing how **trash buildup can lead to flooding** and how agent-based garbage collectors can be **deployed to prevent or resolve** such situations.

---

## 🔧 How It Works

- **Streets** are represented by horizontal and vertical bands of patches.
- **Buildings** occupy fixed regions and are static elements of the environment.
- **Storm drains** (drains) accumulate trash over time.
- **Rainfall** occurs periodically. If drains are clogged, streets become flooded.
- **Garbage collectors (agents)** are created in regular intervals to visit and clean clogged drains.

---

## 🧩 Key Variables

### Global Variables

- `dias`: Simulated day counter.
- `chovendo?`: Indicates whether it is currently raining.
- `total-entupidos`: Cumulative count of clogged drains.
- `lixo-removido`: Total amount of trash removed by agents.
- `cor-rua`, `cor-alagada`: Color codes for streets and flooded areas.
- `proxima-chuva`: Tick value when the next rain will occur.
- `ruas-alagadas?`: Flag indicating if any streets are currently flooded.

### Patch Variables

- `is-building?`: Marks if a patch is part of a building.
- `is-drain?`: Marks if a patch is a storm drain.
- `lixo`: Amount of trash on the drain.
- `entupido?`: Indicates if the drain is clogged.
- `tempo-entupido`: Time the drain has been clogged (can be used for metrics).

### Turtle Variables

- `destino`: Target drain patch for the garbage collector.
- `carga-lixo`: Amount of trash collected by the agent.

---

## ▶️ How to Run

1. Open the NetLogo model file.
2. Click **Setup** to initialize the simulation.
3. Click **Go** to start running the simulation loop.
4. Use the optional `add-trash` button to simulate trash surges.

---

## 📊 Metrics & Analysis

During the simulation, the following behaviors can be observed and analyzed:

- Frequency of drain clogging (`total-entupidos`)
- Efficiency of trash removal (`lixo-removido`)
- Rain-triggered flooding events (`ruas-alagadas?`)
- Effectiveness of agent deployment (`numero-garis`)

These metrics can be used to explore **emergent behavior**, **agent coordination**, and **urban resilience** in a multi-agent system.

---

## 🧠 Learning Outcome

This project demonstrates how **multi-agent systems** can model real-world urban problems and test adaptive solutions in a simulated environment. It provides insights into **coordination, resource allocation**, and **emergent behaviors** resulting from agent interactions.

---


