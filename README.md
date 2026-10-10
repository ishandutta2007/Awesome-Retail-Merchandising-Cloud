# Awesome-Retail-Merchandising-Cloud

# Top Retail Merchandising Cloud Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Assortment Planning, Inventory Optimization & Self-Hosted Merchandising Platforms*  
**Last updated: October 2026**

This repository tracks notable **commercial retail merchandising platforms** and **open-source projects** that manage product assortment, inventory planning, pricing optimization, and shelf execution across retail channels.

**Examples** include Salesforce Mass Merchant Solutions, Blue Yonder, SPS Commerce, Repsly, Trax Retail, Toolio, Inventory Planner, Flxpoint, Crisp Data, and Retalon (the category leaders).

**Open-source emphasis**: Retail merchandising cloud is an emerging open-source domain with strong foundations for demand forecasting, inventory optimization, and pricing. **demandplan** leads as a production-grade demand planning library with probabilistic forecasting, intermittent demand methods, and hierarchical reconciliation validated on real Walmart M5 data . **OpenEC** provides a modular, provider-agnostic analytics platform for e-commerce and retail with inventory forecasting and pricing modules . **AI Blueprints from Crisp** offers open-source, AI-ready templates for assortment planning, on-shelf availability, and store clustering . **RetailVision** demonstrates AI-powered shelf auditing with planogram mismatch detection . **planogram-tools** brings zero-dependency planogram visualization and editing . **Retail Price Optimization** shows end-to-end ML-based price elasticity and profit maximization . This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Blue Yonder](https://blueyonder.com/)**
  **Enterprise retail planning and execution platform** — Category Management suite with Shopper Insights for behavioral analytics, Planogram Generator Enterprise for algorithmic store-specific planogram generation, and assortment optimization with demand transfer prediction .

- **[SPS Commerce](https://www.spscommerce.com/)**
  **Retail analytics and decision intelligence platform** — unifies omnichannel sales and inventory data across trading partners with pre-built dashboards for sell-through, weeks of supply, and assortment performance. Customers see +68% two-year revenue growth and +12% gross margin improvement .

- **[Repsly](https://www.repsly.com/)**
  **Retail execution platform** — AI Image Recognition turns shelf photos into insights in under 60 seconds with up to 98% SKU accuracy. Merchandising, field sales, promotion execution, and retail services modules. Customers see 22% more visits per rep and 180% more voids closed .

- **[Trax Retail](https://traxretail.com/)**
  **Computer vision and shelf analytics platform** — Signal-Based Merchandising leverages shelf signals and visit data to uncover root causes of out-of-stocks. Next Best Action provides real-time store-specific guidance to field teams. New SKU detection in under two weeks .

- **[Retalon](https://retalon.com/)**
  **Unified retail analytics and merchandise planning** — AI-powered demand forecasting, assortment planning, inventory optimization, and markdown optimization. One customer reduced rebalancing from a month-long cycle to 15 minutes for the entire company .

- **[Crisp](https://gocrisp.com/)**
  **Collaborative commerce platform** — connects and normalizes 40+ retail data sources for real-time insights. AI Blueprints provide open-source, AI-ready templates for store clustering, weather analytics, anomaly detection, and on-shelf availability .

- **[Salesforce Mass Merchant Solutions](https://www.salesforce.com/)**
  **Salesforce's retail merchandising solutions** — integrated with Commerce Cloud for assortment, inventory, and order management.

- **[Toolio](https://www.toolio.com/)**
  **Merchandise planning platform** — modern planning for assortment, inventory, and open-to-buy.

- **[Inventory Planner](https://www.inventory-planner.com/)**
  **Inventory forecasting and replenishment** — demand forecasting, purchase order suggestions, and stockout prevention.

- **[Flxpoint](https://www.flxpoint.com/)**
  **Product data and inventory management** — multi-channel product listings, inventory sync, and dropship automation.

## Open-Source GitHub Projects

### Demand Forecasting & Inventory Planning

- **[demandplan](https://pypi.org/project/demandplan/0.4.0/)**  
  **Production-grade demand planning library with probabilistic forecasting, intermittent demand methods, hierarchical reconciliation, and inventory decisions**, Apache-2.0 licensed . **Measured selection, not rules** — champion-challenger backtests pick a method per SKU; no hardcoded segmentation thresholds. **Quantiles are the contract** — every forecaster returns predictive distributions because inventory decisions consume tails (newsvendor), not points. **Validated adversarially** — golden-reference tests against vetted implementations, ground-truth simulations, real Walmart M5 data. **Results**: +30% FVA vs naive on real M5 data, coherence error 5e-13 across 283 nodes, safety stock hits 95.3% realized service vs 95% target, 25,000-series champion-challenger in ~250s single machine. **Shipped**: naive/seasonal-naive, ETS, ARIMA/SARIMA, Croston/SBA/TSB, global LightGBM, MinT-shrink/WLS/BU-TD-MO reconciliation, rolling-origin backtesting, newsvendor order-up-to. **Best for production demand planning with measured model selection**.

- **[OpenEC](https://pypi.org/project/openec/)**  
  **Open Source AI-Powered Ecommerce & Retail Analytics Platform**, AGPL-3.0 licensed . **Provider pattern** — one API, many data sources (Shopify, Amazon SP-API, WooCommerce, Google Analytics). **Command hierarchy** covering products, orders, customers, inventory, marketing, analytics, and pricing. **Inventory commands**: `/inventory/levels/*`, `/inventory/forecasting/*`, `/inventory/movements/*` for stock management, demand forecasting, and turnover analysis. **OECject response wrapper** with `.to_dataframe()`, `.to_dict()`, `.to_json()`, `.to_chart()`. **Extension system** via pip-installable plugins discovered at runtime. **REST API** on port 6900. **Best for modular, extensible retail analytics with provider abstraction**.

- **[Smart Inventory and Demand Forecasting System](https://github.com/JRAnalyst14/Smart_Inventory_and_Demand_Forecasting_System)**  
  **MySQL-powered system for tracking stock, analyzing sales trends, and predicting demand in retail**, open-source . **Real-time inventory tracking** — keep an eye on stock levels and movement. **Demand forecasting** — predict future sales trends using SQL-based analysis. **Data-driven insights** — make informed decisions based on historical sales data. **User access control** — secure role-based permissions. **Automated reports** — generate key inventory and demand insights dynamically. **SQL techniques**: joins, subqueries, transactions, constraints. **Best for SQL-centric inventory and demand analysis**.

- **[python_inventory_manager](https://github.com/NK-Forge/python_inventory_manager)**  
  **Professional inventory management automation tool**, open-source . **Automated analysis** — low stock detection with urgency levels (Critical/Low), category performance breakdown, inventory valuation, and reorder calculations with cost estimates. **Professional reporting** — visual charts (category analysis, stock distributions, restock priorities), CSV exports, executive summaries, customizable thresholds. **Python 3.8+** with pandas, matplotlib, seaborn. **Best for automated inventory analysis and reporting**.

### Assortment Planning & Pricing Optimization

- **[Retail Price Optimization with ML](https://github.com/bijay-odyssey/Retail-Price-Optimization-with-ML-Regression-Elasticity-Profit-Maximization)**  
  **End-to-end price optimization system using ML regression, competition-adjusted elasticity, and profit-curve simulation**, open-source . **Gradient Boosting/Random Forest regression** for demand prediction. **Competition-adjusted price elasticity** estimated via 1% price change simulation. **Price simulations (+/−10%)** to test sensitivity. **Profit curve construction** for individual products. **Optimal price selection** that maximizes predicted profit. **Key findings**: average elasticity –0.45 (inelastic), some products up to –7, optimal prices often higher than current. **Example output**: optimal price $350 vs current $45.95, profit swing +$384.44. **Best for ML-based retail pricing research**.

- **[RLASORTI (SKU Optimization with RL)](https://github.com/dmitriyrayder/RLASORTI)**  
  **Professional SKU assortment optimization system based on Reinforcement Learning (Deep Q-Network)**, open-source . **Automatically analyzes sales and suggests optimal decisions**: which SKUs to keep, which to remove for profit maximization, how to adjust stock depth. **Features**: Excel/CSV data loading, feature engineering (15+ features), DQN with experience replay, business metrics (GMV, Profit, ROI, Out-of-Stock cost, Turnover), interactive Plotly dashboards, CSV export. **Streamlit web interface** with configurable RL parameters. **Best for RL-based assortment optimization research**.

- **[Retail Markdown Optimization (RelationalAI)](https://github.com/relationalai/templates/blob/main/v1/retail_markdown/retail_markdown.py)**  
  **Retail markdown mixed-integer linear optimization (MILP) template**, open-source . **Models products, discounts, and weeks as concepts** with typed properties. **Chooses exactly one discount level per product per week** (binary selection). **Enforces price ladder** so discounts can only increase over time. **Bounds weekly sales by demand** (base demand × discount lift × weekly multiplier). **Tracks cumulative sales and ensures inventory is not exceeded**. **Maximizes total revenue** from discounted sales plus salvage value of leftover inventory. **Best for prescriptive markdown optimization**.

### Shelf Auditing & Planogram Tools

- **[RetailVision](https://github.com/deoxilix/retailVision)**  
  **AI-powered retail shelf auditor**, open-source . **Upload a shelf photo, get a manager-ready audit report** with detected issues, planogram mismatches, a deterministic score, and prioritized restock actions. **Full-stack pipeline**: FastAPI backend (upload → Magnific enhance → GPT-4o vision → planogram match → score → report) with Next.js frontend. **Deterministic scoring with weighted penalty formula**. **Sample data**: 3 planograms (snacks, cereal, beverages). **Best for AI-powered shelf auditing and planogram compliance**.

- **[planogram-tools](https://www.npmjs.com/package/planogram-tools)**  
  **Zero-dependency planogram visualization and editing tool**, open-source . **Visual editing/generation of chest cabinet planograms** via `npx`. **Forward**: define cabinet dimensions → divide columns → divide baskets → fill skuId → export JSON. **Reverse**: import existing planogram JSON, render on canvas, drag/edit, re-export. **Data model invariants**: column widths sum to cabinet width, basket heights sum to cabinet height, integer allocation via largest remainder method. **Best for planogram design and JSON schema compliance**.

- **[merch-connector (MCP Server)](https://www.npmjs.com/package/merch-connector)**  
  **MCP server giving merchandising agents eyes on any storefront**, open-source . **11 tools** for scrape, audit, compare, roundtable analysis, and eval tracking. **Five expert personas**: Floor Walker (first-time shopper), Auditor (compliance analyst), Scout (competitor VP), B2B Auditor (procurement buyer), Conversion Architect (CRO specialist). **Puppeteer with stealth plugin** bypasses bot detection. **Network intelligence** fingerprints 35+ commerce platforms via XHR interception. **Persistent site memory** with change detection across visits. **Best for AI-agent-driven merchandising audits**.

### Additional Strong Open-Source Options

- **merchGent** — Open-source tool for retail merchandising site analysis, related to merch-connector .
- **Claude-ecom** — Turns ecommerce orders CSV into executive-grade business review with KPI decomposition, prioritized findings, and concrete next actions. One command .
- **Classytic Planning** — Pure, deterministic MRP net-requirements calculation kernel with zero runtime dependencies. Forecast consumption, time-phasing, network allocation, and lot sizing .
- **hypar-io/Function-SpacePlanning** — The Space Planning function for laying out, sketching, and defining program uses for spaces .
- **Sweet Home 3D** — Open-source interior design tool for floor plans and 3D home models, useful for retail space planning .
- **Alea Carta Est** — Research code for shopping basket choice modeling with embeddings for product interactions, useful for assortment optimization .

**Frameworks for building custom retail merchandising solutions**: Combine **demandplan** for production-grade demand forecasting with probabilistic quantiles and hierarchical reconciliation . Use **OpenEC** for modular retail analytics with provider abstraction across Shopify, Amazon, and WooCommerce . Deploy **RetailVision** for AI-powered shelf auditing and planogram compliance . Integrate **planogram-tools** for zero-dependency planogram design and JSON schema generation . Use **Retail Price Optimization** for ML-based price elasticity and profit maximization . Note that true enterprise merchandising cloud with unified assortment planning, inventory optimization, and vendor-supported SLAs (Blue Yonder, SPS Commerce, Retalon) remains primarily commercial territory; open-source stacks provide strong demand forecasting, assortment optimization, and shelf analytics foundations that require integration for complete retail merchandising operations.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Retail merchandising platforms handle sensitive sales, inventory, and pricing data. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations.
- **Demand forecasting accuracy depends on data quality** — historical sales, seasonality, promotions, and external factors all influence forecasts. demandplan's champion-challenger approach validates method selection per SKU .
- **Planogram compliance requires accurate shelf data** — AI-powered auditing like RetailVision depends on image quality and planogram accuracy .
- **License considerations**: demandplan uses Apache-2.0 , OpenEC uses AGPL-3.0 , and planogram-tools is open-source . Verify licensing against your use case before committing.
- The open-source ecosystem provides strong demand forecasting, assortment optimization, and shelf analytics foundations, but **unified assortment planning, inventory optimization, and vendor-supported SLAs** remain primarily commercial offerings.
