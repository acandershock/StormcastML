[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/jfIvZbKc)
# COSC 526-426 Project: Scientific Visualization with Climate Data

This project focuses on exploring and visualizing large-scale climate datasets from the [IEEE SciVis 2026 Contest](https://sciviscontest2026.github.io/). The contest provides real scientific data used in climate and ocean modeling, giving you the opportunity to analyze complex environmental phenomena and communicate insights through visualization.

# Table of Contents

- [SciVis Tasks Overview](#scivis-tasks-overview)
- [Python Environment Installation on JetStream2](#python-environment-installation-on-jetstream2)
- [Installing New Python Libraries into the Environment](#installing-new-python-libraries-into-the-environment)

# SciVis Tasks Overview

In this project, you will work with large climate datasets commonly used in scientific research. This repository includes initial Jupyter notebooks for reading SciVis datasets using the OpenVisus framework.
There are four tasks available in the SciVis Contest. Your project will focus on **one scientific question from the SciVis contest tasks**. See the task descriptions [here](https://sciviscontest2026.github.io/tasks/home) to explore each option.
The available tasks are as follows:

### `task0_climate_exploration/`  
Analyze climate projections using the NEX-GDDP CMIP6 dataset.

**Focus:**
- Visualize temperature changes over time 
- Explore regional humidity patterns

**Variables:**
- Air temperature
- Humidity

### `task1_wind_patterns`  
Analyze global wind patterns using DYAMOND GEOS data.

**Focus:**
- Visualize wind direction and magnitude
- Explore atmospheric circulation patterns

**Variables:**
- U, V, and W wind components

### `task2_weather_events`  
Study atmosphere–ocean interactions during storms and extreme weather events using DYAMOND data.

**Focus:**
- Hurricanes
- Cyclones
- Monsoons

**Possible variables include:**
- Wind
- Pressure
- Temperature
- Sea surface temperature
- Ocean currents
- Salinity

### `task3_ocean_circulation`  
Visualize deep ocean circulation using the ECCO LLC4320 dataset.

**Focus:**
- Ocean circulation across depth
- Thermohaline circulation patterns

**Variables:**
- Vertical velocity
- Temperature
- Salinity

# Python Environment Installation on JetStream2

**Requirements:** Access to a Jetstream2 instance via SSH or WebShell.

### 1. Initial Setup (Skip if you already have an instance for the course)

If you do not already have a Jetstream2 instance, follow the instructions in the [Jetstream2 Setup Manual](./jetstream2_manual.pdf) to create and connect to one.

### 2. Connect to your Jetstream2 instance

### 3. Clone the project repository

### 4. Build the Python environment `Python (NSDF-SciVis)`
```
module load miniforge
./build_jetstream_environment.sh
```

### 5. Start JupyterLab
```
jupyter-ip.sh
```

### 6. Open JupyterLab

Open the URL printed in the terminal in your web browser.

### 7. Select the correct kernel

In JupyterLab, select the kernel named: `Python (NSDF-SciVis)`

### 8. Open the notebook for your selected task

Navigate to the Jupyter notebook corresponding to the task you selected and begin working on your project.

# Installing New Python Libraries into the Environment

### 1. Activate the SciVis environment

From the terminal, run: 
```
conda activate nsdf-scivis
```

### 2. Verify the Python path

Confirm that your Python path points to the activated environment:
```
which python
```

### 3. Install the desired library

Replace `<library_name>` with the name of the library you want to install:
```
python -m pip install <library_name>
```

### 4. Restart the Jupyter kernel 

If you already have a JupyterLab session open, you may need to restart the kernel for the newly installed libraries to become available.