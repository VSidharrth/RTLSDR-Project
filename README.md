# RTL-SDR Based Modulation Classification

A communication systems and machine learning project focused on **modulation classification using RTL-SDR, GNU Radio, MATLAB/Simulink, and Python-based machine learning algorithms**.

The project combines **Software Defined Radio (SDR)**, digital communication systems, signal processing, and machine learning to analyze and classify different modulation schemes.

---

## 📡 Project Overview

This project explores the use of **Software Defined Radio (SDR)** and **machine learning** for signal analysis and modulation classification.

The project consists of two main components:

1. **Communication System Simulation** using MATLAB and Simulink
2. **SDR-Based Signal Processing and Machine Learning** using RTL-SDR, GNU Radio, and Python

The project covers both simulated communication signals and real-world RF signal reception.

---

## 🧰 Technologies Used

### Programming & Data Science

- Python
- NumPy
- Pandas
- Scikit-learn
- XGBoost
- Google Colab

### Machine Learning

- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- XGBoost

### Communication Systems

- MATLAB
- Simulink
- FSK
- BFSK

### Software Defined Radio

- GNU Radio
- GNU Radio Companion
- RTL-SDR

---

## 📻 Modulation Schemes

The project covers practical experimentation with the following modulation schemes:

| Modulation | Description |
|------------|-------------|
| FSK | Frequency Shift Keying |
| BFSK | Binary Frequency Shift Keying |
| FM | Frequency Modulation |
| SSB | Single Sideband |
| LSB | Lower Sideband |

---

## 🔬 Project Workflow

The overall project workflow is:

```text
                    Communication System Simulation
                              │
                              ▼
                       MATLAB / Simulink
                              │
                       ┌──────┴──────┐
                       │             │
                      FSK           BFSK
                       │             │
                       └──────┬──────┘
                              │
                              ▼
                       Signal Analysis
                              │
                              ▼
                       RTL-SDR / GNU Radio
                              │
                    ┌─────────┴─────────┐
                    │                   │
                  SSB / LSB             FM
                    │                   │
                    └─────────┬─────────┘
                              │
                              ▼
                        I/Q Capture
                              │
                              ▼
                       Signal Processing
                              │
                              ▼
                       Feature Extraction
                              │
                              ▼
                     Machine Learning Models
                              │
              ┌───────────────┼────────────────┐
              │               │                │
             KNN       Decision Tree      Random Forest
              │               │                │
              └───────────────┼────────────────┘
                              │
                           XGBoost
                              │
                              ▼
                   Modulation Classification
```
# RTL-SDR Based Modulation Classification

## 1. Communication System Simulation

This project includes communication system simulations using **MATLAB and Simulink**.

The simulations focus on digital modulation techniques such as:

- FSK (Frequency Shift Keying)
- BFSK (Binary Frequency Shift Keying)
- FSK modulation and demodulation
- Signal generation and analysis

The communication system simulations provide a foundation for understanding how different modulation techniques behave before applying signal-processing and machine-learning methods.

---

## 2. Software Defined Radio

An **RTL-SDR receiver** is used to capture real-world RF signals.

The captured signals can be processed using **GNU Radio Companion** and represented as I/Q data for further analysis.

The project includes experiments involving:

- SSB / LSB
- FM
- RF signal reception
- I/Q signal representation
- Signal processing

---

## 3. GNU Radio Flowgraphs

GNU Radio Companion is required to open the `.grc` files.

### SSB / LSB Experiment

Open:

```text
SSB.grc
This flowgraph is used for the **SSB/LSB signal-processing experiment**.
```
### **FM Experiment**

Open the following file:

```text
fm.grc
```
This flowgraph is used for the **FM signal-processing experiment**.
```
```
### **💻 Hardware Requirement**

An **RTL-SDR device** is required if the flowgraphs are going to be used for live signal reception.

The **frequency** and **sampling parameters** may need to be adjusted depending on the receiving environment and available signals.

---

## **📚 What We Learned**

This project gave us practical experience in both **communication systems and machine learning**.

During the project, we worked with:

- 📡 Software Defined Radio
- 🔌 RTL-SDR hardware
- 🧩 GNU Radio Companion
- 📊 I/Q signal representation
- 📻 SSB/LSB processing
- 📻 Wideband FM
- 💾 Signal capture
- 🤖 Machine-learning-based modulation classification
- 📶 FSK modulation
- 📶 FSK demodulation
- 🧮 MATLAB/Simulink

One of the main observations from the project was that **signal representation and feature selection are important for modulation classification**.

Even though machine-learning models can classify signal data, the **quality of the information supplied to the classifier strongly affects the final performance**.

---

## **📁 Repository Contents**

| File | Description |
|---|---|
| `SSB.grc` | GNU Radio flowgraph for the SSB/LSB experiment |
| `fm.grc` | GNU Radio flowgraph for the FM experiment |
| `LSB_File_Sink.csv` | Captured LSB signal data |
| `WBFM_File_Sink.csv` | Captured WBFM signal data |
| `SDCS REPORT.docx` | Detailed project report |
| `SDCProject.pptx` | Project presentation |
| `README.md` | Project documentation |

---

## **👥 Team**

- **V. Sidharrth**
- **B G Rajath Siddarth**
- **Venkat Dharaneswar**
📜 License

This project is intended for educational and academic purposes.
