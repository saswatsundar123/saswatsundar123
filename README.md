# 🌌 Hi! I am Saswat 

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&duration=3000&pause=1000&color=2ecc71&center=true&vCenter=true&width=700&lines=Hi%2C+I%27m+the+Architect+behind+CropForge;Building+Scientific+Tools+for+Plant+Biology;Bridging+the+Gap+with+Computational+Physics" alt="Typing SVG" />
</p>

<p align="center">
  <a href="https://github.com/saswatsundar123"><img src="https://img.shields.io/github/followers/saswatsundar123?label=Followers&style=for-the-badge&color=2ecc71&logo=github" alt="GitHub Followers" /></a>
  <a href="mailto:saswatsundar123@gmail.com"><img src="https://img.shields.io/badge/Email-Contact%20Me-blue?style=for-the-badge&logo=gmail&logoColor=white&color=3498db" alt="Email" /></a>
  <a href="https://linkedin.com/in/saswat-sundar-laha-7b4478227"><img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin&logoColor=white&color=0077b5" alt="LinkedIn" /></a>
</p>

---

### 🚀 The Mission

> **I am a developer and researcher building high-performance, open-source scientific computing tools.**  
> My work focuses on bridging the gap between functional-structural plant biology and computational physics, providing researchers with the infrastructure they need to simulate, visualize, and scale agricultural digital twins.

---

## 🔬 Featured Research: CropForge

> **CropForge is a local-first, code-driven virtual farm environment designed for agricultural scientists.**  
> It moves beyond the "black box" of legacy point-models by providing a spatially explicit, 3D interactive digital twin ecosystem.

### 🏛️ The Decoupled Playback Architecture
The core innovation of this ecosystem is the complete separation of mathematical computation from visual rendering:

```mermaid
graph LR
    subgraph Compute Engine ["🧠 The Headless Engine (Python)"]
        A[Physics Solver] -->|NumPy Arrays| B[Simulation Loop]
        B -->|High-throughput writing| C[(Apache Parquet Logs)]
    end
    
    subgraph Visualization Canvas ["🎨 The Playback Canvas (Three.js/WebGL)"]
        C -->|Buffered Streaming| D[Float32Array Buffers]
        D -->|GPU Instancing| E[10,000+ Custom Crops at 60 FPS]
    end

    style Compute Engine fill:#111,stroke:#2ecc71,stroke-width:2px,color:#fff
    style Visualization Canvas fill:#111,stroke:#3498db,stroke-width:2px,color:#fff
    style C fill:#222,stroke:#f1c40f,stroke-width:2px,color:#fff
```

* **The Headless Engine:** The Python-based time-stepping engine processes complex biological and environmental physics, logging the entire spatial field state into highly optimized, columnar Apache Parquet files.
* **The Playback Canvas:** The frontend acts as an interactive mirror, reading the Parquet logs and streaming them as binary `Float32Array` buffers directly to the GPU. This allows researchers to render and scrub through timelines of 10,000+ custom crops without choking the browser thread.

---

## 💻 Core Technical Stack

| Domain | Technologies Used |
| :--- | :--- |
| **Compute & Logic** | ![Python](https://img.shields.io/badge/python-3670A0?style=flat-square&logo=python&logoColor=ffdd54) **Python 3.10+**, ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=flat-square&logo=numpy&logoColor=white) **NumPy** |
| **Data Streaming** | ![Apache Parquet](https://img.shields.io/badge/Apache_Parquet-000000?style=flat-square&logo=apache&logoColor=white) **Apache Parquet**, ![PyArrow](https://img.shields.io/badge/PyArrow-FC6D26?style=flat-square&logo=apache&logoColor=white) **PyArrow** |
| **Backend API** | ![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=flat-square&logo=fastapi) **FastAPI**, ![Uvicorn](https://img.shields.io/badge/Uvicorn-222222?style=flat-square) **Uvicorn** |
| **Visualization** | ![Three.js](https://img.shields.io/badge/three.js-000000?style=flat-square&logo=three.js&logoColor=white) **Three.js** (WebGL Instancing), ![Plotly Dash](https://img.shields.io/badge/Plotly_Dash-3F4F75?style=flat-square&logo=plotly&logoColor=white) **Plotly Dash** |

---

## 🌱 Secondary Sandbox

While my primary engineering focus is on computational agriculture, I also apply my development skills to a few other domains:

* **Vadraa:** Exploring robust software solutions and digital platforms.
* **CampusKatha:** Building community-driven architecture and tools.

---

## 📬 Let's Connect

I am always open to discussing digital agriculture, systems architecture, or open-source scientific computing.

* **GitHub:** [saswatsundar123](https://github.com/saswatsundar123)
* **LinkedIn:** [Saswat Sundar Laha](https://linkedin.com/in/saswat-sundar-rath)
* **Email:** [saswatsundar123@gmail.com](mailto:saswatsundar123@gmail.com)

> *"We aren't just replacing field trials; we are providing the spatial environment that legacy models completely lack."*
