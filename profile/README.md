# NKZ Open Standard (Nekazari) 🚜🛰️

<p align="left">
  <a href="https://nkz-os.org">
    <img src="https://img.shields.io/badge/Documentation-nkz--os.org-blue?style=for-the-badge&logo=readthedocs" alt="Documentation" />
  </a>
  <img src="https://img.shields.io/badge/License-AGPL--3.0-green?style=for-the-badge" alt="License: AGPL-3.0" />
  <img src="https://img.shields.io/badge/Standard-FIWARE_NGSI--LD-orange?style=for-the-badge" alt="FIWARE NGSI-LD" />
  <img src="https://img.shields.io/badge/Deploy-Kubernetes-326ce5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes" />
</p>

**The Open Source reference architecture for 3D Digital Twins in AgTech, Industry, and Environment.**

Nekazari OS (NKZ) is a highly modular, GitOps-driven platform designed to bridge the gap between physical assets (Edge) and their digital representations (Cloud). Built strictly on **FIWARE NGSI-LD** and **Smart Data Models**, it provides unparalleled interoperability for massive satellite imagery processing, IoT telemetry, and autonomous agricultural robotics.

---

## 🏗️ The Ecosystem (Polyrepo Architecture)

NKZ OS follows a decoupled architecture to prevent vendor lock-in and allow independent scaling of components.

* 🧠 **[nkz](https://github.com/nkz-os/nkz)**: The Core backend. Contains the Context Broker integrations, FastAPI Gateway, TimescaleDB persistence, Keycloak Auth, and the CEP visual rules engine.
* 🌐 **[web](https://github.com/nkz-os/web)**: The SSG portal for our Docs-as-Code automated documentation.
* 📦 **[nkz-module-template](https://github.com/nkz-os/nkz-module-template)**: The canonical starter kit for third-party developers to create platform extensions with pre-configured CI/CD and Docker scaffolding.

## 🧩 Dynamic Modularity (IIFE Runtime)

NKZ OS relies on an **IIFE (Immediately Invoked Function Expression) Runtime Script Injection** architecture. This allows third-party developers, academic researchers, and hardware manufacturers to build independent, domain-specific modules (e.g., LiDAR point clouds, isoBUS telemetry, Crop Health via Sentinel-2) that dynamically plug into the core **CesiumJS 3D engine** without tight coupling or redeploying the core platform.

## 🔌 Open Hardware & Edge Integration

We don't just process data; we standardize how it's generated. NKZ provides **Hardware Reference Designs** for field edge devices.
Whether you are building custom MQTT dataloggers or designing autonomous agricultural rovers (ROS2/Zenoh), our reference architectures ensure your hardware is natively compliant with the NKZ Digital Twin standard right out of the box.

👉 *Check the [Edge Integration Docs](https://nkz-os.org) for BOMs, isoBUS wiring, and payload schemas.*

---

## 🎓 Academic Research & Community 

NKZ is built to be the foundational infrastructure for AgTech research. We actively welcome contributions from university talent (Computer Science, Telecommunications, Agronomy). 
* Don't waste time building backends for your TFG/TFM. Fork the `nkz-module-template`, focus on your algorithm (AI, Vision, Robotics), and inject it into our 3D environment.
* Look for issues tagged with `good first issue` or `tfg-candidate` across our repositories.

## 🏢 Enterprise & Institutional Adoption

For public institutions handling Copernicus data or managing large-scale agronomic knowledge transfer, the NKZ architecture handles terabytes of TIFs via MinIO and rio-tiler without cluster degradation. The **NKZ Enterprise** deployment model offers SLA-backed operations, dedicated GitOps pipelines (ArgoCD), and custom legacy ERP integrations (Odoo).

---

### 📖 Start Building

All technical documentation, K8s deployment guides, and API specifications are automatically compiled from our source code:

**👉 [Read the Official Documentation at nkz-os.org](https://nkz-os.org)**

📫 **Contact the maintainers:** [nkz@nkz-os.org](mailto:nkz@nkz-os.org)
