**Strategic Intelligence Engine for Humanitarian Decision-Making**

**The "Why" Behind This Project: A View from the Field**

As a Consortium Coordinator and Head of Base, I was constantly navigating a torrent of fragmented information. Strategic decisions depended on synthesizing data streams that rarely spoke to each other: quantitative reports from different clusters like Security, Food Security, WASH, and Protection, secuirty and qualitative updates from field staff, and our own internal project M&E data.

The core challenge I faced was not a lack of data, but a lack of synthesis. We had the pieces of the puzzle, but no way to assemble them into a single, coherent picture to guide strategy.

This project was born from that challenge. It is the strategic intelligence engine I always wanted, designed to break down these data silos. Its purpose is to ingest, harmonize, and unify disparate information into one holistic view. This unified data layer allows different leaders to ask their specific questions and receive answers that are contextually aware, creating a foundation for truly integrated and evidence-based decision-making.

**A Unified View for Multi-Scale Decisions & Strategic Benchmarking**

By creating a single, harmonized data environment, this engine provides a unique dual capability. It allows leaders to conduct multi-scale analysis—zooming from a national, strategic overview down to a tactical, communal level. Furthermore, it enables strategic benchmarking by comparing internal project data against broader contextual trends, providing a much deeper measure of performance. This ensures that tactical, operational, and strategic decisions are all grounded in the same comprehensive understanding of the context.

Some Exemple include:

1. Strategic Planning & Gap Analysis
Question: Where are the "epicenters" of the crisis? Which communes suffer from a convergence of shocks like high conflict, soaring food prices, and acute humanitarian needs?

Data Used: Conflict Events + Food Prices + Humanitarian Needs (IPC)+ Wealth Index


2. Operations, Logistics & Access

Question: What is the safest and most viable route to reach a target community today, considering recent security incidents along key roads?

Data Used: Road Network + Conflict Events (filtered by date)


3. Risk Management & Early Warning

Question: Which communes are showing early warning signs of a deteriorating food security situation, allowing for anticipatory action?

Data Used: Food Prices + Conflict Events + IPC (historical)

4. Context for Monitoring, Evaluation & Benchmarking
Question (Strategic Benchmarking): Is our beneficiaries' food security improving at a faster rate than the overall trend in their commune of residence?

Data Used: IPC (over time) + (Internal M&E data for beneficiaries)


**Technical Innovation for Humanitarian Action**

Flexible & Automated Data Pipeline: A dynamic ingestion engine automatically discovers and loads various data formats (CSV, Shapefile, GeoDatabase), allowing for the seamless integration of new datasets without code changes.

Intelligent Geospatial Harmonization: A "canonical" geographic reference layer is created from multiple, often inconsistent sources, ensuring the integrity and consistency of all spatial analysis.

AI-Powered Semantic Georeferencing: A state-of-the-art AI model (sentence-transformer) matches locations based on their semantic meaning, robustly cleaning and harmonizing messy, real-world data where place names are often ambiguous or misspelled.

**Modularity and Adaptability**

While this project uses food security in Haiti as its central case study—integrating key contextual factors like security, road access, prices, wealth index, operational presence, and humanitarian needs—its core strength lies in its flexibility.

The underlying code is designed to be thematic and country-agnostic. The entire data processing pipeline can be easily adapted for other countries or different humanitarian sectors (e.g., Health, WASH, Protection). Furthermore, the automated ETL process is built to seamlessly integrate new datasets, allowing any organization to incorporate its own internal data for a customized and even more powerful analysis.

**Technical Stack**

Data Analysis: pandas, numpy

Geospatial Processing: geopandas, fiona

Natural Language Processing (NLP): sentence-transformers

Visualization: matplotlib, seaborn

Environment: Python 3.12, Google Colab

**Project Status**

The project is structured in distinct phases, providing a clear development roadmap.

Phase 1: ETL & Data Harmonization - Completed
The core data engineering pipeline is fully functional. This includes the automated ingestion of diverse data sources, the creation of a canonical geographic table, and the development of the AI-powered semantic matching engine.

Phase 2: Data Cleaning & Preprocessing - Ongoing
This phase involves applying the harmonization functions to the full range of loaded datasets and conducting in-depth cleaning to handle missing values, outliers, and inconsistencies identified during the initial loading.

Phase 3: Exploratory Data Analysis (EDA) & Modeling - To-Do
Future work will focus on performing detailed univariate and multivariate analysis to uncover insights and correlations. This phase will also include the development of predictive models for an an early warning system.

Phase 4: Interface & Dashboard Development - To-Do
The final stage will be to develop an interactive and user-friendly dashboard (e.g., using Tableau, Power BI, or Dash) to make the engine's analytical power accessible to non-technical end-users.
