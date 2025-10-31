# NetworkAware-AgentPy

[![Python Version](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/)  
[![License](https://img.shields.io/github/license/yomex96/NetworkAware-AgentPy)](https://github.com/yomex96/NetworkAware-AgentPy/blob/main/LICENSE)  
[![Documentation Status](https://readthedocs.org/projects/agentpy/badge/?version=latest)](https://agentpy.readthedocs.io/en/latest/?badge=latest)  
[![GitHub stars](https://img.shields.io/github/stars/yomex96/NetworkAware-AgentPy?style=social)](https://github.com/yomex96/NetworkAware-AgentPy/stargazers)  
[![GitHub forks](https://img.shields.io/github/forks/yomex96/NetworkAware-AgentPy?style=social)](https://github.com/yomex96/NetworkAware-AgentPy/network/members)  
[![Build Status](https://img.shields.io/github/actions/workflow/status/yomex96/NetworkAware-AgentPy/python-package.yml?branch=main)](https://github.com/yomex96/NetworkAware-AgentPy/actions)



**NetworkAware-AgentPy** is a **research-grade Python framework for network-aware, resilient multi-agent autonomous systems**. Built on **agent-based modeling**, this project allows researchers to **simulate, analyze, and visualize autonomous agents under network constraints**, with applications in **urban systems, IoT networks, smart infrastructure, and distributed autonomous workflows**.

> A Python framework to model, simulate, and analyze network-aware, resilient multi-agent autonomous systems for urban and IoT applications.

This repository includes a **ready-to-run demo simulation notebook** to showcase research contributions visually.

---

## 🔹 Framework Capabilities

- **Model design:** Define agents, environments, and interaction rules  
- **Scenario simulation:** Test agents under network constraints, failures, and dynamic conditions  
- **Numerical experiments & metrics:** Evaluate coordination, resilience, and system efficiency  
- **Visualization:** Track agent behavior and system-level outcomes  

---

## 🔹 Installation

```bash
git clone https://github.com/yomex96/NetworkAware-AgentPy.git
cd NetworkAware-AgentPy
pip install -r requirements.txt
````

---

## 🔹 Key Features

* Multi-agent simulation with customizable agents and behaviors
* **Network-aware environments:** latency, bandwidth constraints, link failures
* **Resilience modeling:** agents adapt to failures or communication interruptions
* Scenario examples: traffic coordination, IoT sensor networks, autonomous drone fleets
* **Data analysis & visualization** for performance metrics and emergent behaviors

---

## 🔹 Demo Simulation: Network-Aware Traffic Coordination

This demo illustrates **autonomous vehicles coordinating under network constraints** in a simulated urban environment.

### Objective

* Simulate autonomous vehicles navigating a city grid
* Agents communicate through a limited network with **latency and packet loss**
* Evaluate how agents **adapt to network failures** and coordinate efficiently

### Key Features Demonstrated

* **Multi-Agent Coordination**: Vehicles operate autonomously and interact with neighbors
* **Network Awareness**: Agents respond to messages simulating communication constraints
* **Resilience**: Packet loss and network failures tested
* **Visualization & Metrics**: Agent positions and performance metrics tracked

### Getting Started

```bash
jupyter notebook notebooks/demo_simulation.ipynb
```

---

## 🔹 Research Motivation

This project demonstrates the **design of resilient, collaborative, and network-aware multi-agent autonomous systems**. It bridges theory and practical applications in **urban infrastructure, IoT, and distributed systems**, supporting research in **autonomous workflows, agentic AI, and network-aware decision-making**.

**Relevance to PhD research:**
The framework aligns with current trends in **agentic AI, multi-agent orchestration, and autonomous systems**, providing hands-on experiments relevant to **MIT IDSS** and interdisciplinary autonomous systems research.

---

## 🔹 Future Work

* Integration of **reinforcement learning policies** for adaptive agent behavior
* Large-scale simulation of **societal infrastructures** under realistic network conditions
* Comparative experiments on **coordination strategies and resilience mechanisms**

## 🔹 Analysis & Metrics

This project supports analysis of:

* **Communication success rate:** Messages successfully delivered under packet loss
* **Coordination efficiency:** How effectively agents complete tasks under network constraints
* **Resilience:** Performance under simulated network failures
* **Emergent behavior:** Patterns that arise from decentralized agent interactions

### Example Python Snippet

```python
import numpy as np
import random

success_counts = []
for _ in range(steps):
    successes = sum(random.random() > env.packet_loss for _ in links)
    success_counts.append(successes)

success_rate = np.array(success_counts) / len(links)
print("Communication success rate:", success_rate)
```

*Visualization of metrics is included in the demo notebook.*

---

## 🔹 Demo Notebook Structure

`notebooks/demo_simulation.ipynb` includes:

* Introduction & Objective
* Environment Setup (agents, network constraints)
* Simulation Run (time-steps, agent actions)
* Visualization (graphs of agent positions and network status)
* Metrics & Analysis (resilience, coordination efficiency)
* Conclusion & Next Steps

---

## 🔹 Citing this Work

If you use this project in your research, please cite as:

```
Onawole, A.R., (2025). NetworkAware-AgentPy: A Python framework for network-aware multi-agent autonomous systems. GitHub Repository, https://github.com/yomex96/NetworkAware-AgentPy
```



