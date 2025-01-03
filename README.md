# Emergency Department Simulation

## Project Overview

The **Emergency Department (ED) Simulation** project models patient flow through two areas of a hospital's emergency department:

- **Fast Track**: Designed for minor injuries and illnesses.
- **Main ED**: Designed for more critical and complex cases.

This simulation helps evaluate system performance by analyzing metrics such as **wait times**, **resource utilization**, and **system bottlenecks**. The results provide insights into how the system performs under varying conditions (e.g., increased patient volume) and help design an appropriate **system capacity** to meet future demands.

---

## Features

- **Discrete-Event Simulation (DES)**: Models patient arrivals, triage, treatment, and discharge.
- **Performance Metrics**: Evaluates wait times, throughput, and resource utilization.
- **Scenario Analysis**: Tests different staffing and resource allocation strategies to identify optimal system performance.
- **Visualization**: Generates histograms and 3D surface plots to visualize wait times and resource utilization.

---

## Prerequisites

Ensure that you have **Python 3.7** or higher installed on your machine. The following Python libraries are required to run the simulation:

- `numpy`
- `scipy`
- `pandas`
- `matplotlib`
- `seaborn`
- `simpy`


## Installation Instructions

First, clone the repository to your local 
machine:

```
git clone https://github.com/wongwenhui262/HTX_Test.git
cd HTX_Test
```

## Install Python libraries

After activating the virtual environment, install the necessary Python libraries by running:

```
pip install -r requirements.txt
```

## Run the Simulation

Run the simulation by executing the script on jupyter notebook:

```
Emergency_Department_Simulation.ipynb
```

This will run the discrete-event simulation and generate output files, including performance metrics and visualizations.

---

## Usage

### Customizing the Simulation

You can adjust various parameters in the Emergency_Department_Simulation.ipynb script to modify how the simulation runs:

- **Patient Arrival Rates:** How often patients arrive in the ED (can be adjusted for both Fast Track and Main ED).
- **Service Times:** Average time taken for treatment in the Fast Track and Main ED.
- **Staffing Levels:** Number of doctors, nurses, and other medical staff available.
- **Resource Availability:** Number of treatment cubicles available.

For example, adjusting the number of doctors in the Main ED and Fast Track might look like this:

```python
# Adjust staffing levels
number_nurses_miu = 3
number_docs_miu = 2
number_nurses = 5
number_docs = 4
```

### Running Different Scenarios

Run different scenarios to see how changes to staffing levels or patient volume affect performance to optimize resource allocation and plan for future demand increases.

---

## Simulation Outputs

After running the simulation, you will see several outputs:

### Performance Metrics:
- Average wait times for triage, cubicle assignments, and doctor consultations.
- Resource utilization rates, such as the percentage of time nurses, doctors, and cubicles are in use.
- Throughput: The number of patients treated (discharged or admitted).

### Visualizations:
- **Wait Time Histogram:** Displays the distribution of patient wait times in the ED.
- **3D Surface Plots:** Shows the impact of staffing levels on wait times and resource utilization.
- **Utilization Rates:** Visual representation of how well resources are being used.

---


### File Descriptions:
- **requirements.txt:** Contains the required dependencies for the project.
- **Emergency_Department_Simulation.ipynb:** The script that runs the simulation and generates results.
- **Simulation_Model_Algorithm_Writeup.pdf:** File with the writeups on simulation outputs (such as plots).
- **README.md:** This file with instructions and documentation.
- **ED_Process_Flowchart.drawio.png:** This file contains the process flowchart.

