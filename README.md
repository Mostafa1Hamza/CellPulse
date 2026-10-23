# CellPulse
### Advanced RAN Analytics Engine

<p align="center">
  <strong>Transforming Network Data into Engineering Intelligence</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Domain-RAN%20Analytics-CC0000?style=for-the-badge" alt="RAN Analytics">
  <img src="https://img.shields.io/badge/Focus-KPI%20Intelligence-0A7EA4?style=for-the-badge" alt="KPI Intelligence">
  <img src="https://img.shields.io/badge/Automation-Engineering%20Workflows-3776AB?style=for-the-badge" alt="Engineering Automation">
  <img src="https://img.shields.io/badge/Technologies-Ericsson%20%7C%20Huawei-333333?style=for-the-badge" alt="Multi-vendor RAN">
</p>

---

## Overview

**CellPulse** is an advanced RAN analytics project designed to simplify telecom KPI exploration, accelerate network performance investigations, and automate repetitive engineering workflows.

Built around practical Radio Access Network (RAN) optimization requirements, CellPulse aims to bring data retrieval, temporal analysis, multi-level aggregation, visualization, and automated assessment into a unified analytical environment.

The goal is straightforward: **reduce the time between identifying a network performance issue and producing an evidence-based engineering decision.**

## The Engineering Challenge

Telecom optimization engineers frequently work across multiple data sources, SQL queries, spreadsheets, KPI dashboards, and reporting tools. This fragmented workflow can make investigations slower, repetitive, and difficult to standardize.

CellPulse is designed to address these challenges through:

- Unified KPI exploration across different network entities.
- Flexible temporal filtering and resolution control.
- Consistent data processing and aggregation.
- Interactive visualization for comparing KPIs and network elements.
- Streamlined data export and engineering workflows.
- A foundation for explainable, rule-based performance assessment.

## Core Capabilities

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>📡 Multi-Level Network Analytics</h3>
      Analyze performance at different network levels:
      <ul>
        <li>Cell and sector</li>
        <li>Site and cluster</li>
        <li>Selected network groups</li>
        <li>Aggregated performance views</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>⏱️ Temporal Intelligence</h3>
      Investigate network behavior over time:
      <ul>
        <li>Hourly and daily resolution</li>
        <li>Flexible time-window selection</li>
        <li>Trend comparison</li>
        <li>Historical performance analysis</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>📊 Flexible KPI Visualization</h3>
      Explore network metrics through:
      <ul>
        <li>Single KPI and single-cell analysis</li>
        <li>Multiple KPI comparisons</li>
        <li>Multi-cell trend analysis</li>
        <li>Interactive time-series charts</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>⚙️ Engineering Automation</h3>
      Streamline analytical workflows through:
      <ul>
        <li>Structured data processing</li>
        <li>Excel-driven analytical workflows</li>
        <li>Reusable assessment logic</li>
        <li>Exportable results</li>
      </ul>
    </td>
  </tr>
</table>

> The capabilities above describe the project scope. Refer to the implementation status and roadmap below for the distinction between the current demonstration and planned functionality.

## KPI Analytics

CellPulse is intended to support performance analysis across multiple RAN domains.

| Domain | Example analytical focus |
|---|---|
| Accessibility | Connection establishment and access success |
| Retainability | Connection stability and abnormal release analysis |
| Mobility | Handover performance and mobility behavior |
| Capacity | PRB utilization, CCE utilization, and resource pressure |
| Throughput | User and cell throughput trends |
| Coverage | RF conditions and coverage-related performance |
| User activity | Connected-user trends and network demand |

KPI formulas, aggregation policies, counter semantics, and valid data ranges must be defined explicitly before production use. Not every KPI can be aggregated using a simple arithmetic mean.

## Architecture

CellPulse is designed around a modular architecture that separates data access from analytics and presentation.

```text
               DATA SOURCES
          ┌─────────┴─────────┐
          │                   │
     CSV / Excel        Authorized DB
          │             Integration
          └─────────┬─────────┘
                    │
                    ▼
          DATA ACCESS LAYER
                    │
                    ▼
        VALIDATION & NORMALIZATION
                    │
                    ▼
          KPI ANALYTICS ENGINE
          ├── KPI Definitions
          ├── Aggregation Rules
          ├── Temporal Processing
          └── Assessment Logic
                    │
                    ▼
          FILTERING & ANALYSIS
                    │
                    ▼
          DASHBOARD & EXPORTS
```

### Architectural principles

- **Separation of concerns:** keep database access, KPI calculations, and user interface logic independent.
- **Data integrity:** validate schemas, timestamps, missing values, and KPI domains.
- **Scalability:** select data-processing strategies appropriate for the size and structure of telecom datasets.
- **Reproducibility:** preserve the time window, filters, KPI definition, and aggregation context of analytical outputs.
- **Security:** restrict database access and avoid exposing credentials or confidential network data.

## Technology Stack

The exact stack depends on the implementation of each module.

| Layer | Technologies |
|---|---|
| Programming | Python |
| Data processing | Pandas, NumPy |
| Database analytics | SQL; authorized ENIQ integration where implemented |
| Visualization | Streamlit and charting libraries |
| Data exchange | CSV, Excel |
| Potential analytical storage | DuckDB or another suitable analytical backend |

Only list technologies as implemented dependencies when they are actually used in the repository.


## Development Roadmap

| Phase | Objective |
|---|---|
| Phase 1 | Establish the dashboard, synthetic data, filtering, and basic visualization |
| Phase 2 | Implement KPI definitions, formula validation, and aggregation policies |
| Phase 3 | Add cell, sector, site, and cluster hierarchy processing |
| Phase 4 | Improve large-dataset performance and import/export workflows |
| Phase 5 | Implement approved database adapters with appropriate security controls |
| Phase 6 | Develop explainable assessments, historical baselines, and automated findings |

### Planned enhancements

- Dynamic KPI selection and comparison.
- Configurable aggregation policies for different KPI types.
- Robust hourly and daily time-series handling.
- Automated detection of abnormal KPI trends.
- Excel-driven KPI analysis.
- Controlled SQL query and data-export workflows.
- Reproducible assessments with documented assumptions.
- Automated tests and data-quality reporting.

## Quality and Validation

Reliable RAN analytics requires more than displaying charts. The implementation should validate:

- Missing or malformed input columns.
- Invalid timestamps and inconsistent time zones.
- Empty datasets and filters returning no records.
- Duplicate observations and out-of-range KPI values.
- Zero denominators and undefined KPI calculations.
- Different aggregation requirements for counters, ratios, and measurements.
- Performance limits when processing large datasets.

Assessment outputs should distinguish measured facts from hypotheses and recommendations.

## Security and Data Governance

CellPulse is intended for telecom engineering workflows, where data confidentiality and access control are essential.

- Never commit database credentials, tokens, or connection strings.
- Do not publish confidential operator configurations or restricted vendor documentation.
- Do not expose customer information or identifiable production site/cell data.
- Use synthetic, anonymized, or explicitly authorized data in public demonstrations.
- Use least-privilege database accounts and safe query limits for any authorized integration.

## About the Author

**Mostafa Hamza**  
RAN Optimization Engineer | Telecom Analytics | Python Automation

Telecommunications engineer with approximately six years of experience progressing from RF drive testing and post-processing to RAN optimization, network performance analysis, and engineering automation.

My work focuses on Ericsson and Huawei RAN environments, SQL-based KPI analytics, Python engineering tools, and practical approaches to improving network performance and operational efficiency.

CellPulse reflects my interest in combining telecom domain knowledge with software engineering to build useful, maintainable, and data-driven analytical tools.

- GitHub: https://github.com/Mostafa1Hamza
- LinkedIn: https://www.linkedin.com/in/mostafa-hamza-4lte3umts2gsm/

---

<p align="center">
  <strong>CellPulse — Turning Network Data into Actionable Engineering Insights</strong>
</p>
