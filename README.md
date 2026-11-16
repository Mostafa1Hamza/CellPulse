<div align="center">
  <img src="https://github.com/user-attachments/assets/17cf0494-c1a8-40c8-b5c7-9fef940119db" alt="CellPulse Logo" width="180" />
  
  <h1>CellPulse Analytics</h1>
  
  <p>
    <strong>Enterprise-Grade Telecom KPI Intelligence & Automated Network Diagnostics</strong><br>
    <em>Specialized for Ericsson Sybase IQ & Cross-Vendor (Huawei) Integration</em>
  </p>
</div>

<hr> CellPulse Analytics: Enterprise Telecom Performance & Intelligence Platform

**CellPulse** is an enterprise-grade telecommunications analytics platform designed to transform massive volumes of raw network data into instant, actionable intelligence. 

<img width="1442" height="964" alt="image" src="https://github.com/user-attachments/assets/27f90ccd-10bc-4f7b-a0a3-4d3564deb589" />


Specially engineered as a unified command center for **Ericsson** network environments (via direct Sybase IQ integration), CellPulse also features robust cross-vendor support. **Huawei (HU)** engineers can seamlessly ingest data exports to leverage the platform's advanced multi-dimensional charting, automated benchmarking, and presentation modes.

For telecom managers and engineering directors, CellPulse eliminates the bottleneck of manual data processing, turning millions of network logs into executive-ready dashboards in seconds.

---

## 🎯 Executive Summary & Business Value

* **Accelerated Decision Making:** Replaces hours of manual Excel crunching with instant, automated data visualization. Engineers spend less time formatting data and more time optimizing the network.
* **Unified Vendor Strategy:** A single pane of glass for both Ericsson (Database) and Huawei (CSV/XLSX) performance metrics, ensuring standard reporting practices across different network regions.
* **Automated Change Assessment:** Built-in A/B testing ("Assess Action" & "Benchmark Action") mathematically evaluates network interventions, providing definitive proof of improvement or degradation after a change.
* **Zero-Latency Reporting:** Designed to handle millions of rows locally without crashing, ensuring the Network Operations Center (NOC) and optimization teams have real-time visibility.

---

## ✨ Core Platform Capabilities

### 📈 1. Dynamic, Multi-Dimensional Dashboards
* **Flexible Viewing Modes:** Users can seamlessly toggle between "One KPI - One Cell", "Multi KPI - One Cell", and complex "Multi KPI - Multi Cell" combinations to identify hidden network correlations.
* **Smart Aggregation Engine:** Instantly rolls up raw cell-level data into Site, Sector, Band, or Entire Network-level views with a single click.
* **Intelligent Visualization:** The system automatically recognizes data types (e.g., displaying Erlang/Traffic volume as background bars while rendering Quality metrics as overlay trend lines).

<p align="center">
  <img src="https://github.com/user-attachments/assets/0d414234-738b-4369-9da9-119cef5e8327" alt="Description 1" width="48%" />
  <img src="https://github.com/user-attachments/assets/5603d5c2-9564-4529-8573-2c26a2568069" alt="Description 2" width="48%" />
</p>

### ⚖️ 2. Automated Network Change Assessment 
* **Assess Action Module:** When an engineer optimizes a site, this module overlays the "Before" (T-7 baseline) and "After" performance on a synchronized timeline.
* **Statistical Benchmarking:** The engine automatically calculates the P10, P50 (Median), and P90 Deltas, providing an unbiased, mathematical verdict on whether the change *Improved*, *Degraded*, or remained *Stable*.

<p align="center">
  <img src="https://github.com/user-attachments/assets/9f45af42-8595-4b7a-b58c-b54aca74070f" alt="Description 1" width="48%" />
  <img src="https://github.com/user-attachments/assets/49870d61-7ecf-4c63-824b-d0a2d6586243" alt="Description 2" width="48%" />
</p>

### 🔍 3. Advanced Mobility Diagnostics (HO Investigation)
* **Root-Cause Isolation:** Replaces tedious log parsing by automatically mapping complex Handover (HO) and 5G ENDC relations.
* **Automated Offender Ranking:** Instantly ranks mobility corridors, generating ready-to-use tables of "Top Successes" and "Worst Offenders" to immediately direct field teams and RF engineers to problem areas.

<img width="1392" height="348" alt="image" src="https://github.com/user-attachments/assets/95e774fa-e55f-4a48-bdd6-b87fce6879ae" />


### 📊 4. Executive Reporting & Workflow Automation
* **Auto Slideshow Mode:** Transforms the dashboard into an automated presentation, cycling through hundreds of worst-performing cells automatically—ideal for morning NOC briefings or daily management stand-ups.
* **High-Res "Snaps" Export:** A custom rendering engine that captures presentation-ready, high-definition images of the dashboard with a single click, perfectly formatted for management emails or PowerPoint reports.

---

## ⚙️ Under the Hood: Engineering Scale & Reliability

While the UI is designed for simplicity, the CellPulse backend is engineered for massive scale, solving the traditional bottlenecks of telecom data processing:

* **Massive Data Handling (Chunking & Downcasting):** Connects directly to Ericsson Sybase IQ databases, pulling millions of rows via memory-optimized streaming. It dynamically compresses data in-flight to prevent Out-Of-Memory (OOM) crashes typical of standard analytics tools.
* **Real-Time Computation Engine:** Custom KPI formulas are pre-compiled into machine-level bytecode, allowing the platform to calculate complex success rates across thousands of cells instantly.
* **Resilient Session Architecture:** Built with a custom "Silent Socket Grafting" technology. If a browser tab goes to sleep or network connectivity drops, the system seamlessly rebuilds the connection in the background without losing the engineer's active dashboard state.
* **Secure Raw SQL Interface:** Provides advanced users with a safe, read-only SQL terminal to extract custom ad-hoc reports directly to CSV without interrupting the main dashboard visualizer.


<div align="center">
  <table>
    <tr valign="top">
      <td width="50%">
        <img src="https://github.com/user-attachments/assets/444e7b67-d803-459f-b8c5-31d7b33ab57d" alt="Dashboard View" width="100%" />
      </td>
      <td width="50%">
        <img src="https://github.com/user-attachments/assets/376cffca-f55f-476d-a51a-c53078b1c068" alt="Ericsson DB Setup" width="100%" />
      </td>
    </tr>
    <tr valign="top">
      <td width="50%">
        <img src="https://github.com/user-attachments/assets/dde36187-a631-4090-ba23-a308f85952f6" alt="Raw SQL Export" width="100%" />
      </td>
      <td width="50%">
        <img src="https://github.com/user-attachments/assets/31f2a889-e9d8-4b81-9cb8-d38797fdd620" alt="Benchmark Engine" width="100%" />
      </td>
    </tr>
  </table>
</div>
---
*CellPulse Analytics: Engineered for precision. Designed for scale. Built for the modern telecom network.*
