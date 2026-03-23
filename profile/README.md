# Nekazari OS (NKZ)

<p align="center">
  <a href="https://nkz-os.org">
    <img src="https://img.shields.io/badge/Documentation-nkz--os.org-blue?style=for-the-badge&logo=readthedocs" alt="Documentation" />
  </a>
  <img src="https://img.shields.io/badge/License-AGPL--3.0-green?style=for-the-badge" alt="License: AGPL-3.0" />
  <img src="https://img.shields.io/badge/Standard-FIWARE_NGSI--LD-orange?style=for-the-badge" alt="FIWARE NGSI-LD" />
</p>

**The Open Source standard for Digital Twins in Agriculture, Industry, and Environment.**

Nekazari OS is a highly modular, GitOps-driven platform designed to bridge the gap between physical assets (Edge) and their digital twin representations (Cloud). Built on top of strict industry standards like **FIWARE NGSI-LD** and **Smart Data Models**, it provides unparalleled interoperability for IoT telemetry, satellite imagery, and autonomous robotics.

## 🚀 Ecosystem

- **[nkz](https://github.com/nkz-os/nkz)**: The Core platform repository (Context Broker, API Gateway, TimescaleDB, Keycloak Auth).
- **[web](https://github.com/nkz-os/web)**: The Docs-as-Code automated documentation portal.
- **[nkz-module-template](https://github.com/nkz-os/nkz-module-template)**: The canonical starter kit for third-party developers to create platform extensions.

## 🧩 Modularity

NKZ OS relies on an IIFE (Immediately Invoked Function Expression) Runtime Script Injection architecture. This allows third-party developers, hardware manufacturers, and universities to build independent domain-specific modules (e.g., LiDAR, isoBUS, Crop Health) that dynamically plug into the core CesiumJS 3D engine without coupling.

## 📖 Documentation

All technical documentation, deployment guides, and hardware integration specifications are automatically compiled and available at our official portal:

**👉 [Read the Docs at nkz-os.org](https://nkz-os.org)**
