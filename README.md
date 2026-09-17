# Brightcon 2026 Presentation Files 
**Title:** Co-Simulating Brightway Life Cycle Assessments with the Functional Mockup Interface

**Authors:** Kathryn Hinkelman, Anastasija Mensikova

**Email:** kathryn{dot}hinkelman{at}uvm{dot}edu

**Presentation Date:** 24 September 2026


# Quick Start
1. Create the conda environment:
	```bash
	conda env create -n fmlca -f environment-fmlca.yml
	```
2. Activate it:
	```bash
	conda activate fmlca
	```
3. Run the demo notebook:
	```bash
	jupyter notebook Demonstration.ipynb
	```

# Presentation Details
## Abstract
Modern sustainability assessments increasingly require dynamic integration of life cycle assessment (LCA) results with engineering simulations for systems optimization, real-time decision support, and multi-physics modeling. While Brightway-based LCA makes this integration more feasible than end-to-end software stacks (e.g., SimaPro, OpenLCA), coupling with external simulation environments remains challenging due to incompatible interfaces and computational overhead. The Functional Mockup Interface (FMI) standard offers a solution by enabling seamless co-simulation between heterogeneous modeling tools.

This presentation demonstrates a complete workflow for converting Brightway2 LCA models into standardized FMI 2.0-compliant Functional Mockup Units (FMUs). Using Python, Brightway2, and the pythonfmu library, we showcase automated extraction of emission factors from ecoinvent 3.12 databases for both climate change impacts (IPCC 2021 GWP100) and endpoint damages (ReCiPe 2016). The workflow transforms JSON inventories into production-ready FMUs with standardized input/output interfaces (energy consumption as input and single-score environmental impacts as output). These FMUs are ready for co-simulation with dynamic multi-domain system simulation tools, such as Modelica. A live demonstration includes FMU generation for a grid-tied PV system, followed by validation. All code, data, and FMUs are provided as reproducible examples with complete automation scripts.

With a focus on advancing the sustainable design and operation of energy systems, this presentation advocates for fully open-source, reproducible tools that democratize access to advanced LCA-simulation coupling. By standardizing LCA interfaces through FMI compliance, we foster cross-platform collaboration between LCA practitioners and model-based systems engineers, advancing transparent and interoperable sustainability assessment workflows.

## Presenter Bio
Dr. Kathryn Hinkelman is an Assistant Professor in Civil and Environmental Engineering at the University of Vermont. She develops open-source tools for community energy systems, combining expertise in Modelica, life cycle assessment, and biomimetic systems engineering to advance sustainable, resilient, and equitable infrastructure. This presentation will explore how Brightway models can bridge LCA and engineering simulation through open standards, enabling integrated environmental analysis of complex energy systems.



