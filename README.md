# Smarter Power for Smarter AI 🚀
### Power Optimization in AI Data Centers using NVIDIA GB300 & Machine Learning

This project explores how **unsupervised machine learning** techniques can be used to optimize energy efficiency in **AI-driven data centers**, using telemetry data inspired by **NVIDIA’s GB300 NVL72 architecture**.

We simulate and analyze the behavior of **7,200 GPUs** across **100 racks** over a one-hour window, focusing on:
- Power draw (Watts)
- GPU utilization (%)
- Energy storage (Joules)
- Grid voltage (Volts)
- Workload synchronization and transitions

## 🧠 Techniques Used
- **KMeans Clustering** – Identify GPU workload patterns
- **Isolation Forest** – Detect anomalies in voltage, temperature, or power
- **PCA** – Visualize high-dimensional power behavior
- **Exploratory Data Analysis (EDA)** – Understand load profiles and transitions

## 📊 Key Findings
- Synchronized GPU workloads cause power spikes >1300W
- Capacitor-based energy smoothing can reduce grid load by ~30%
- Power draw directly correlates (0.90+) with GPU utilization
- Training workloads dominate, with clear separation from inference and idle states
- Burn mode stabilizes power transitions and avoids grid stress

## 🔍 Dataset
- **Synthetic, time-series dataset**
- 10,000 records with 5-second intervals
- Features: `Power_Draw_Watts`, `GPU_Utilization_Percent`, `Energy_Stored_Joules`, `Grid_Voltage_Volts`, `Temperature_Celsius`, `Workload_Type`, `Power_State`, `Sync_Flag`, `Power_Cap_Watts`, etc.

