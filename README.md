# RTL-SDR Based Modulation Classification

A communication systems and machine learning project focused on **modulation classification using RTL-SDR, GNU Radio, MATLAB/Simulink, and Python-based machine learning algorithms**.

The project combines **Software Defined Radio (SDR)**, digital communication systems, signal processing, and machine learning to analyze and classify different modulation schemes.

---

## 🚀 Technologies Used

- Python
- NumPy
- Pandas
- Scikit-learn
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- XGBoost
- Google Colab
- MATLAB
- Simulink
- GNU Radio Companion
- RTL-SDR

---

## 📡 Modulation Schemes

The project covers practical experimentation with:

- **FSK** — Frequency Shift Keying
- **BFSK** — Binary Frequency Shift Keying
- **FM** — Frequency Modulation
- **SSB** — Single Sideband
- **LSB** — Lower Sideband

---

## 📖 Project Overview

This project consists of two major components:

### 1. Communication System Simulation

Communication systems were designed and simulated using **MATLAB and Simulink**.

The simulation focuses mainly on FSK/BFSK modulation and demodulation.

Topics covered include:

- Digital modulation
- Signal generation
- FSK modulation
- BFSK modulation
- FSK demodulation
- Signal analysis
- Communication system simulation

---

### 2. SDR-Based Signal Processing and Classification

An **RTL-SDR** device was used as a Software Defined Radio receiver to capture real-world RF signals.

The received signals are represented using **I/Q (In-phase and Quadrature) samples** and processed for further analysis and machine-learning-based modulation classification.

The machine-learning component explores several classification algorithms:

- K-Nearest Neighbors
- Decision Tree
- Random Forest
- XGBoost

---

## 🧠 Machine Learning Pipeline

The general machine-learning workflow is:

```text
Signal Data
     │
     ▼
Signal Preprocessing
     │
     ▼
Feature Extraction
     │
     ▼
Machine Learning
     │
     ├── KNN
     ├── Decision Tree
     ├── Random Forest
     └── XGBoost
     │
     ▼
Modulation Classification
```
The objective is to investigate how effectively machine-learning algorithms can distinguish between different modulation schemes based on signal characteristics.

📊 I/Q Signal Representation

Software Defined Radios commonly represent RF signals using two components:

I — In-phase
Q — Quadrature

Together, these components form the complex baseband representation:

x(t) = I(t) + jQ(t)

I/Q samples preserve important information about the amplitude and phase of the received signal, making them useful for signal processing and modulation classification.

🔧 GNU Radio Flowgraphs

The project includes GNU Radio Companion (.grc) flowgraphs.

GNU Radio Companion (GRC) is required to open and run these files.

SSB / LSB Experiment

Open:

SSB.grc

This flowgraph is used for the SSB/LSB signal reception and processing experiment.

FM Experiment

Open:

fm.grc

This flowgraph is used for the FM signal reception and processing experiment.

Note: An RTL-SDR device is required if the flowgraphs are used for live signal reception.

The frequency and sampling parameters may need to be adjusted depending on:

Receiving environment
Target signal
Antenna
RTL-SDR device
Available RF spectrum
Required bandwidth
📻 RTL-SDR
```
```
An RTL-SDR receiver can be used to capture real-world RF signals for analysis.

Typical parameters that may need to be configured include:

Center frequency
Sample rate
Frequency correction (PPM)
Gain
Bandwidth
```
```
The appropriate values depend on the receiving environment and the signal being investigated.

🔬 Project Workflow

The overall workflow can be summarized as:

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
                     Machine Learning
                              │
              ┌───────────────┼───────────────┐
              │               │               │
             KNN        Decision Tree    Random Forest
              │               │               │
              └───────────────┼───────────────┘
                              │
                           XGBoost
                              │
                              ▼
                   Modulation Classification
💻 Python Environment

The machine-learning experiments can be executed using Google Colab or a local Python environment.

Required Python Libraries
numpy
pandas
scikit-learn
xgboost

Install the required packages using:

pip install numpy pandas scikit-learn xgboost
🧪 Machine Learning Models
K-Nearest Neighbors

KNN classifies signal samples based on their similarity to neighboring training samples.

Decision Tree

A Decision Tree uses a sequence of decision rules based on extracted signal features.

Random Forest

Random Forest combines multiple decision trees to improve classification robustness and generalization.

XGBoost

XGBoost is a gradient-boosting algorithm that builds an ensemble of decision trees sequentially to improve predictive performance.

📈 Key Observations

One of the main observations from the project was that signal representation and feature selection are important for modulation classification.

Machine-learning models can classify signal data effectively, but their performance strongly depends on the quality of the information supplied to the classifier.

Important factors include:

Quality of the captured signal
Signal-to-noise conditions
I/Q representation
Feature selection
Feature quality
Preprocessing
Choice of machine-learning algorithm
📚 What We Learned

This project provided practical experience in both communication systems and machine learning.

Communication Systems
Software Defined Radio
RTL-SDR hardware
GNU Radio Companion
I/Q signal representation
SSB/LSB processing
Wideband FM
RF signal capture
FSK modulation
BFSK modulation
FSK demodulation
MATLAB
Simulink
Machine Learning
Signal preprocessing
Feature extraction
Classification
KNN
Decision Trees
Random Forest
XGBoost
Modulation classification
🛠️ Requirements
Hardware
RTL-SDR receiver
Suitable antenna
Computer/Laptop
USB connection
Software
Python 3.x
Google Colab or local Python environment
GNU Radio Companion
MATLAB
Simulink
👥 Team
V. Sidharrth
B G Rajath Siddarth
Venkat Dharaneswar
📌 Project Purpose

This project was developed for educational and academic purposes to explore the integration of:

Software Defined Radio + Digital Communication + Signal Processing + Machine Learning

The project demonstrates how real-world RF signals can be captured, represented, processed, and analyzed using machine-learning techniques.

📜 License

This project is intended for educational and academic purposes.

If this repository is publicly distributed, an appropriate open-source license can be added here.

can the whole thing be in readme.md

Yes. The entire content should be saved as a single README.md file. You can copy the following directly into README.md:

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
