# Low-Noise RF Amplifier for Wireless Communication

**Status:** Completed  
**Technology:** GPDK090 (90 nm CMOS)[cite: 2]  
**Tools:** Cadence Virtuoso[cite: 2]  

[![Full Project Report](https://img.shields.io/badge/📄_Read_Full_Report-PDF-blue)](EEE466_Group_03_Project_Report.pdf)
[![Video Demonstration](https://img.shields.io/badge/📺_Watch_Demo-YouTube-red)](https://www.youtube.com/watch?v=tXrC75GiM9c)

## 📌 Project Overview
This project presents the design and simulation of a high-performance Low-Noise Amplifier (LNA) optimized for operation at 1.8 GHz[cite: 2]. The primary objective is to achieve a combination of high gain, low noise figure, and excellent input-output matching while ensuring unconditional stability[cite: 2]. The proposed LNA is implemented using GPDK090 CMOS technology, offering a cost-effective and compact solution for RF front-end applications[cite: 2].

## 🎯 Design Specifications
The LNA was designed to meet the following target parameters for modern RF receiver front-ends:
*   **Operating Frequency:** 1.8 GHz[cite: 2]
*   **Gain (S21):** > 13 dB[cite: 2]
*   **Noise Figure (NF):** <= 1 dB[cite: 2]
*   **Input Return Loss (S11):** <= -13 dB[cite: 2]
*   **Stability Factor (K):** > 1[cite: 2]

## 🛠️ Architecture & Methodology
The design utilizes a two-stage CMOS Low-Noise Amplifier topology[cite: 2]. 
*   **Input Matching & Noise:** Uses inductive source degeneration for input matching and to maintain a low noise figure (NF)[cite: 2]. 
*   **Matching Networks:** An online RF Impedance Matching calculator was utilized to determine the initial values for the inductors and capacitors in the input and output matching networks[cite: 2]. 
*   **Inter-stage Design:** Features RF choke inductors and an AC coupling capacitor between the first and second amplifying stages[cite: 2].

## 📊 Simulation Results
Extensive parametric sweeps and simulations were conducted in Cadence Virtuoso[cite: 2]. The final design successfully met and exceeded all target specifications at 1.8 GHz:
*   **Input Reflection Coefficient (S11):** Achieved -14.4699 dB, indicating strong input matching and reduced signal loss[cite: 2].
*   **Output Reflection Coefficient (S22):** Achieved -10.0554 dB, ensuring efficient signal transfer to the next stage[cite: 2].
*   **Forward Transmission Coefficient (S21):** Achieved a high gain of 34.0766 dB[cite: 2].
*   **Reverse Transmission (S12):** Achieved -39.3075 dB, indicating excellent reverse isolation[cite: 2].
*   **Noise Figure (NF):** Achieved 0.246826 dB, well below the 1 dB target, ensuring minimal added noise[cite: 2].
*   **Stability Factor (K):** Achieved 1.008726, ensuring the amplifier is unconditionally stable across the operating frequency range[cite: 2].

## 🚀 Future Work
*   **Physical Layout:** Completing the physical layout design using Cadence Virtuoso and performing post-layout simulations with DRC and LVS verifications[cite: 2].
*   **Power Optimization:** Refining the biasing networks to reduce overall power consumption for battery-powered applications[cite: 2].
*   **Technology Scaling:** Adapting the design approach to smaller process nodes, such as 65 nm CMOS, for higher integration and improved frequency response[cite: 2].
