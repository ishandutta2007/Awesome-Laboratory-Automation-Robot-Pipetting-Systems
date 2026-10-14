# Awesome-Laboratory-Automation-Robot-Pipetting-Systems

# Top Laboratory Automation & Robot Pipetting Systems Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Liquid Handling, Workcell Orchestration & Closed-Loop Experiment Execution*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Laboratory Automation & Robot Pipetting Systems**. These tools control liquid handling robots, orchestrate multi-instrument workcells, and connect experiment execution to electronic lab notebooks — enabling high-throughput screening, assay development, and autonomous "lab-in-the-loop" workflows.

**Examples** include Benchling, TetraScience, Automata, OpenTrons, Biosero Green Button Go, HighRes Biosolutions, Strateos (Transcriptic), Hamilton VENUS, Tecan FluentControl, and Cellario OS (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, Python-native protocol control, and transparent workcell orchestration — ideal for academic labs, biotech startups, and developers building accessible automation infrastructure.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Benchling Automation](https://www.benchling.com/)**  
  Unified platform connecting instrument data to scientific records, enabling "lab-in-the-loop" systems where AI models propose candidates and automated labs execute experiments. Launched with **open ecosystem** partners including **HighRes, Automata, Ginkgo Bioworks, Celltrio, Opentrons, and Hamilton** [citation:2]. Features **Automation Designer** (drag-and-drop pipeline builder), **Custom Code** (Python-in-Benchling for advanced parsing and analysis), and **Experiment Optimization** (ML and Bayesian methods for next-best experimental conditions) [citation:14]. Pulls data from **200+ instruments** across file-based and API-based systems, automatically linked to samples and experiments [citation:2].

- **[TetraScience Tetra Data Platform](https://www.tetrascience.com/)**  
  Open, vendor-agnostic platform purpose-built for scientific data, built on AWS. Ingests raw data from **1000+ instruments**, replatforms to Tetra OS, and harmonizes into vendor-agnostic format via **Intermediate Data Schema (IDS)** [citation:3]. Event-driven architecture with **GxP support** including audit trails and disaster recovery. Data lands in open-source **Delta Lake** format for SQL queries via Amazon Athena and integration with Databricks, Snowflake, or enterprise data lakes [citation:3]. Features **full data lineage** from capture to archival with human-in-the-loop audit trails [citation:15].

- **[Automata LINQ](https://www.automata.tech/)**  
  Lab automation platform building "operating system for AI-ready labs" with **$45M Series C** (January 2026) led by Dimension with strategic investment from **Danaher Corporation** [citation:4]. **LINQ** offers both a **node-based workflow canvas** (drag-and-drop, no-code) and a **Python SDK** for developers, built on an industry-first intelligent scheduling engine [citation:16]. **Cloud-native architecture** enables centralized collaboration and management across multiple workcells. Open platform with full public developer documentation and REST API. Integrating with Danaher's Molecular Devices and Beckman Coulter Life Sciences instruments [citation:4].

- **[OpenTrons](https://opentrons.com/)**  
  **Open-source liquid handling robots** used by Stanford, MIT, Harvard, Merck, and Pfizer [citation:5]. **Flex series** (third generation) supports 1–1000 µL pipetting with Flex 1/8/96 channels, 12 main plate positions plus 4 temporary storage, plate gripper, and smart screen. **OT-2** is the desktop-level, cost-effective open-source alternative. Both share the same **Python API and open-source protocol library** [citation:5]. **Opentrons is a launch partner for Benchling Automation** [citation:2].

- **[Biosero Green Button Go](https://biosero.com/)**  
  Automation scheduling and orchestration software with **Green Button Go Scheduler** (overnight/weekend experiment execution) and **Green Button Go Orchestrator** (full lab orchestration, job routing, safety protocols) [citation:6]. February 2026: **Assistive AI** integrated into Green Button Go allows users to create, review, and troubleshoot automation workflows using **plain English instead of code** [citation:18]. **Strictly assistive** — AI does not execute workflows or make autonomous decisions; all scientific, operational, and quality decisions remain in human hands [citation:18].

- **[HighRes Biosolutions Cellario OS](https://www.highres.com/)**  
  Web-based orchestration software managing full lab workflows including **manual steps, mobile carts, and shared devices** [citation:11]. **Enhanced Digital SOPs** integrate human-performed steps into automated workflows with step-by-step guidance and data capture. **Instruction Libraries** standardize common procedures. **Parallel Requesting** enables concurrent experiments sharing critical resources with conflict detection. **CellarioOS 1.13** adds cart scheduling, Skip Approval workflows, and integrations with Mosaic by Cenevo and Scigilian [citation:11]. Acquired **Let's Go Robotics** (low-volume dispensing) in March 2025 [citation:7].

- **[Hamilton VENUS](https://www.hamiltoncompany.com/)**  
  Software for Hamilton Microlab STAR and VANTAGE liquid handlers. **VENUS 6.3** provides method editor, deck layout configuration, and 21 CFR Part 11 security settings [citation:9]. **CO-RE II pipette technology** with individual pressure monitoring for error detection. Supports 8–384 channel pipetting with on-deck centrifuge and shaker integration [citation:1].

- **[Tecan FluentControl](https://www.tecan.com/)**  
  Control software for Tecan Fluent liquid handling platforms. **FluentControl 3.8** introduces **Identity Access Management (IAM)** with 12-character minimum passwords, DriverFramework 3.3.14+ (no dots in driver names), and automatic user migration from legacy UMS to IAM [citation:10]. Requires Tecan Field Service Engineer for firmware updates.

- **[Strateos (formerly Transcriptic)](https://www.strateos.com/)**  
  **Cloud Lab Automation-as-a-Service** platform providing remote access laboratories and lab control software. Founded 2012, based in Menlo Park [citation:8].

## Open-Source GitHub Projects

- **[pyhamilton](https://github.com/dgretton/pyhamilton)**  
  **Python for Hamilton liquid handling robots.** 181+ GitHub stars, actively maintained [citation:12]. Provides Pythonic interface to Hamilton Microlab STAR and VANTAGE systems, enabling programmatic protocol development without proprietary VENUS software for routine workflows.

- **[PyLabRobot](https://github.com/PyLabRobot/pylabrobot)**  
  **Interactive and hardware-agnostic SDK for lab automation.** 398+ GitHub stars, updated this week [citation:12]. Cross-platform Python framework for controlling liquid handling robots from multiple vendors with a unified API. The most actively developed open-source lab automation SDK.

- **[Tecan Fluent Python Interface](https://github.com/pylabrobot/pylabrobot)**  
  Python interface to TECAN Fluent liquid handling robot [citation:12]. Enables programmatic control and protocol execution.

- **[robotools](https://github.com/JuBiotech/robotools)**  
  **Pythonic in-silico liquid handling and creation of Tecan FreedomEVO worklists.** 17+ GitHub stars [citation:12]. Generates worklists for Tecan Freedom EVO platforms programmatically.

- **[robotevo](https://github.com/qPCR4vir/robotevo)**  
  **Generates Freedom EVOware scripts for the Freedom EVO universal pipetting robot from TECAN.** 28+ GitHub stars [citation:12]. Provides abstraction layers for Tecan Freedom EVO programming.

- **[Roboliq](https://github.com/ellis/roboliq)**  
  **Software for controlling liquid handling robots.** 11+ GitHub stars (archived 2018 but historically significant) [citation:12]. Early open-source attempt at vendor-agnostic liquid handling control.

- **[orca](https://github.com/Cheshire-Labs/orca)**  
  **Lab Automation Scheduling Software.** 20+ GitHub stars, updated December 2025 [citation:12]. Open-source scheduling and orchestration for lab automation workflows.

- **[Otto_the_Robot](https://github.com/Luger-Lab/Otto_the_Robot)**  
  **Protocols for Pipetting with OpenTrons.** 347 commits, actively maintained [citation:17]. Collection of OpenTrons protocols including custom labware definitions and validated scripts for specific assays.

### Additional Strong Open-Source Options

- **Opentrons Python API** — The foundational open-source Python API for programming OT-2 and Flex workstations. Full protocol library available on GitHub.
- **SiLA 2** — Open standard for lab instrument communication, enabling vendor-agnostic control.
- **Antha** — Declarative language for describing and executing laboratory protocols (historical).
- **Autoprotocol** — JSON-based standard for describing biology experiments, originally from Transcriptic/Strateos.

**Frameworks for building custom systems**: Combine **PyLabRobot** for hardware-agnostic robot control, **pyhamilton** for Hamilton-specific protocol execution, **Opentrons Python API** for accessible benchtop automation, and **orca** for scheduling across multiple instruments to build a complete open-source lab automation stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Laboratory automation systems must comply with applicable regulations (21 CFR Part 11 for electronic records, GxP for regulated workflows) and validated for specific assay requirements. **Liquid handling protocols and automation workflows must be validated before use with biological or chemical samples** — incorrect volumes, cross-contamination, or instrument failures can compromise experiments and safety.
- Self-hosted open-source solutions require proper instrument calibration, protocol validation, and integration testing before production use.

---

**Made for lab automation engineers, research scientists, protocol developers, and developers building accessible laboratory automation platforms.**  
Let's make laboratory automation more open, accessible, and reproducible.
