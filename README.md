**Strategic Analysis & Decision-Support Engine for Humanitarian Response in Haiti**

**The "Why" Behind This Project: A View from the Field**

"As a Head of Base in complex emergencies, I always wanted a single tool that could unify the fragmented data I relied on for daily decisions: the latest security report, project progress, road accessibility, the presence of other actors, and local market prices. I needed a holistic view—a single, flexible, and easily accessible tool that could be integrated with new data on the fly."

This project is born from that need. It is my answer, developed with data science skills, to a critical operational challenge I faced firsthand for over a decade. The goal is not to create yet another dashboard, but to provide humanitarian managers with a strategic analysis engine: a tool that transforms raw, disconnected data into actionable intelligence for better, faster decision-making.

*While the initial focus is on Haiti, I have engineered the architecture to be modular and flexible, ready to be rapidly adapted to any other operational context.*

**Project Goals: From Analysis to Action**
This tool is designed to provide concrete answers for leaders and managers within NGOs and International Bodies.

**For an NGO Program Manager or Country Director**:
Create a "Living Map" of the Context:

Not a static map, but a dynamic, multi-layered view that integrates data on food security (IPC), market prices, conflict events, operational presence (3W), infrastructure, and socio-economic vulnerability.

Identify Operational Gaps (Gap Analysis): 

By overlaying our operational presence with needs data, managers can instantly see which areas are most vulnerable and underserved, thereby guiding program strategy and resource allocation.

Integrate Logistics and Security Planning: 

Combine road network data with real-time conflict events to create dynamic access maps, which are critical for staff safety and operational continuity.

**For International Bodies and Donors**:
Allocate Funding Strategically:

Analyze the correlations between different data layers to identify where an intervention can have the greatest impact, ensuring that funding is synergistic and well-targeted.

Build an Early Warning System:

Leverage the harmonized historical database to develop predictive models capable of forecasting a deterioration in food security, enabling a faster and more effective response.

**Technical Innovation for Humanitarian Action**
I have applied advanced data science skills to solve practical, field-level problems.

**Flexible & Automated Data Pipeline:**

I built a dynamic data ingestion engine that automatically discovers and loads various formats (CSV, Shapefile, GeoDatabase). This flexibility allows for the integration of new datasets without any code changes, a crucial feature in contexts where data sources evolve rapidly.

**Intelligent Geospatial Harmonization:**

The system creates a single, "canonical" geographic reference layer from multiple, often inconsistent sources. This guarantees the integrity and consistency of all spatial analysis.

AI-Powered Semantic Georeferencing: The project's most innovative feature. Instead of relying on exact string matching (which often fails due to typos or abbreviations), I used a state-of-the-art AI model (sentence-transformer) to match locations based on their semantic meaning. This allows for a far more robust cleaning and harmonization of messy, real-world data.

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
Future work will focus on performing detailed univariate and multivariate analysis to uncover insights and correlations. This phase will also include the development of predictive models for an early warning system.

Phase 4: Interface & Dashboard Development - To-Do
The final stage will be to develop an interactive and user-friendly dashboard (e.g., using Tableau, Power BI, or Dash) to make the analytical power of this engine accessible to non-technical end-users.
