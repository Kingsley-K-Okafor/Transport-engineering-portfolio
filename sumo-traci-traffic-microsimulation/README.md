# Traffic Microsimulation (SUMO / TraCI)

![Python](https://img.shields.io/badge/Python-3.x-blue) ![SUMO](https://img.shields.io/badge/SUMO-TraCI-green) ![Status](https://img.shields.io/badge/Status-Complete-brightgreen)


### 🔍 Project Summary
Development of a traffic microsimulation model using SUMO and TraCI to analyse traffic flow, signal control strategies, and network performance.

| Metric | Result |
|---|---|
| Average vehicle delay | −17% |
| Intersection throughput | +12% |
| Intersection modelled | 4-arm multi-lane |

---

### 🛠️ Key Responsibilities
- Built a four-arm signalised intersection network in SUMO  
- Defined nodes, edges, connections, and routing logic  
- Developed traffic demand scenarios  
- Controlled signal phases dynamically using TraCI (Python)  
- Extracted trip, speed, and flow data from simulation outputs  

---

### 📈 Engineering Value
- Enabled performance comparison of traffic control strategies  
- Provided data-driven insight into congestion and flow efficiency  
- Demonstrated practical application of simulation in transport engineering  

---

### 🧠 Skills Demonstrated
- Traffic modelling and microsimulation  
- Python scripting (TraCI API)  
- Data extraction and analysis  
- Systems modelling


## How It Works
- SUMO generates a traffic network with configurable vehicle flows
- TraCI connects Python to the live simulation at each timestep
- A control script reads real-time queue lengths per lane
- Signal phases are extended or cut short based on demand thresholds
- Results (delay, speed, throughput) are logged and visualised

## Tech Stack
| Tool | Purpose |
|---|---|
| `SUMO-GUI` | Traffic network simulation environment |
| `TraCI` | Python API to control SUMO in real time |
| `Python 3.x` | Control logic, data collection, visualisation |
| `Matplotlib` | Plotting delay and throughput over time |

## Getting Started

### Prerequisites
```bash
pip install traci matplotlib
# SUMO must be installed separately: https://sumo.dlr.de/docs/Installing/
```

### Run the Simulation
```bash
git clone https://github.com/yourusername/sumo-signal-optimisation
cd sumo-signal-optimisation
python run_simulation.py
```

## Results
| Metric | Fixed Timing | Adaptive (this system) | Change |
|---|---|---|---|
| Avg vehicle delay | 42s | 35s | −17% |
| Intersection throughput | 850 veh/hr | 952 veh/hr | +12% |

---

### 🖼️ Sample Work

![Network View](network-view.png)  
*SUMO network showing four-arm signalised intersection layout*

![Signal Control](signal-control.png)  
*Traffic signal control using TraCI-based Python scripting*

![Output Analysis](output-graph.png)  
*Simulation output showing performance metrics such as speed and flow*

---

### 📌 Note
This project demonstrates simulation workflows and analysis. Full datasets and extended models available on request.
