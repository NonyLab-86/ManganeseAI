# ManganeseAI
### An Explainable AI-Guided Discovery Platform for Stable, Affordable Manganese-Based Cathodes in Aqueous Zinc-Ion Batteries

<p align="center">
  <strong>Artificial Intelligence × Computational Materials Science × Battery Materials Discovery</strong>
</p>

---

## 1. Overview

**ManganeseAI** is an AI-guided materials discovery platform designed to accelerate the identification, evaluation and optimization of stable, affordable and high-performance manganese-based cathode materials for aqueous zinc-ion batteries (AZIBs).

The platform integrates computational materials science, materials informatics, machine learning (ML), explainable artificial intelligence (XAI), crystal structure analysis and experimental electrochemical data to establish a systematic framework for discovering promising manganese-based cathode materials.

By combining data-driven prediction with scientific interpretability, ManganeseAI aims to move beyond conventional trial-and-error materials development towards a more efficient, reproducible and evidence-based materials discovery process.

The platform is designed to accommodate different manganese-based material families, structural polymorphs, elemental modifications and synthesis approaches, supporting both computational and experimental validation.

## 2. Research Motivation

Aqueous zinc-ion batteries are promising candidates for large-scale energy storage because of their potential advantages in safety, cost, material availability and environmental compatibility.

Manganese-based cathodes, particularly manganese oxides (MnO₂), have attracted considerable research attention due to their diverse crystal structures, accessible redox chemistry and potential electrochemical performance.

However, important challenges remain:

- Structural instability during repeated charge-discharge cycles.
- Manganese dissolution into aqueous electrolytes.
- Irreversible phase transformations.
- Limited electronic conductivity.
- Complex Zn²⁺ and proton insertion mechanisms.
- Capacity fading and poor long-term cycling stability.
- Difficulty identifying optimal dopants and structural modifications.

Conventional experimental optimization can be time-consuming and resource-intensive.

ManganeseAI addresses these challenges by developing an integrated computational and data-driven platform for systematically evaluating material composition, crystal structure, thermodynamic stability and electrochemical performance.

## 3. Main Objectives

The primary objectives of ManganeseAI are to:

1. Establish a structured database of manganese-based cathode materials.
2. Collect and integrate computational and experimental materials data.
3. Investigate the influence of crystal structure, composition and elemental doping on material properties.
4. Develop machine learning models for predicting relevant materials properties.
5. Apply explainable AI to identify the most influential material descriptors.
6. Implement multi-objective optimization for prioritizing promising cathode candidates.
7. Support computational and experimental validation of AI-guided predictions.
8. Develop an accessible and reproducible materials discovery platform.

## 4. Materials Scope

ManganeseAI will investigate a broad range of manganese-based cathode materials.

### 4.1 Manganese Oxide Polymorphs

Initial structural investigations will include:

| Structure | Description |
|---|---|
| α-MnO₂ | Tunnel-type manganese dioxide |
| β-MnO₂ | Pyrolusite-type structure |
| γ-MnO₂ | Intergrowth manganese dioxide |
| δ-MnO₂ | Layered birnessite-type structure |

Other manganese oxide polymorphs and structurally modified manganese oxides will be incorporated as the database expands.

### 4.2 Chemical Systems

Initial chemical systems include:

- Mn–O
- Mn–Zn–O
- Mn–V–O
- Mn–P–O
- Mn–Fe–O

### 4.3 Elemental Modification

Potential dopants and structural modifiers will initially include:

- Magnesium (Mg)
- Zinc (Zn)
- Iron (Fe)
- Aluminium (Al)

Additional elements and modification strategies may be incorporated as the research develops.

## 5. Platform Architecture

ManganeseAI is organized into interconnected computational and analytical modules.

| Module | Main Function |
|---|---|
| Data Collection | Retrieve materials information from external databases |
| Scientific Database | Store material compositions, structures and properties |
| Data Processing | Clean, validate and standardize datasets |
| Structure Analysis | Investigate crystal structures and structural descriptors |
| Materials Descriptors | Generate composition- and structure-based features |
| Machine Learning | Predict relevant materials properties |
| Explainable AI | Interpret model predictions and feature contributions |
| Optimization | Prioritize promising materials using multiple objectives |
| Visualization | Present scientific results and interactive comparisons |

The architecture is modular to support future integration of additional materials databases, computational methods and experimental datasets.

## 6. Data Sources

ManganeseAI will integrate information from established computational and crystallographic databases.

| Database | Intended Application |
|---|---|
| Materials Project | Limited Mn-containing summary records, structures and computational properties; see the [integration guide](docs/materials_project_integration.md) |
| JARVIS | Computational materials properties and structural information |
| OQMD | Formation energies and thermodynamic materials data |
| Crystallography Open Database (COD) | Experimentally reported crystal structures |
| Scientific Literature | Experimental electrochemical properties, synthesis conditions and characterization results |

Experimental information will be collected from relevant scientific publications and supplementary datasets where accessible.

Every collected record should retain its original source, database identifier, retrieval information and measurement conditions where available.

Computationally predicted properties and experimentally measured properties will be maintained as distinct data categories.

## 7. Computational and Machine Learning Framework

The platform will integrate established scientific Python libraries.

### Materials Science

- pymatgen
- matminer
- ASE

### Data Processing and Scientific Computing

- NumPy
- Pandas
- SciPy

### Machine Learning

- Scikit-learn
- XGBoost

### Explainable Artificial Intelligence

- SHAP

### Data Visualization

- Matplotlib
- Plotly

### Database and Application Development

- SQLite
- SQLAlchemy
- Streamlit

### Development Environment

- Python
- Jupyter Notebook
- Git
- GitHub Codespaces

The initial machine learning framework will investigate algorithms including Random Forest, Gradient Boosting, XGBoost, Support Vector Regression and Ridge Regression.

Model selection and performance evaluation will depend on the availability, quality and quantity of relevant observations.

## 8. Target Properties and Optimization Objectives

ManganeseAI will investigate properties relevant to the structural stability and electrochemical performance of aqueous zinc-ion battery cathodes.

### Computational Properties

- Formation energy.
- Energy above hull.
- Electronic band gap.
- Crystal structure.
- Lattice parameters.
- Unit cell volume.
- Density.
- Composition-based descriptors.

### Experimental Electrochemical Properties

- Specific discharge capacity.
- Average operating voltage.
- Capacity retention.
- Coulombic efficiency.
- Cycle life.
- Rate capability.
- Impedance characteristics.
- Manganese dissolution.

### Multi-objective Optimization

The optimization framework will consider:

- High specific capacity.
- Suitable operating voltage.
- Improved structural stability.
- Enhanced cycling performance.
- Reduced manganese dissolution.
- Affordable constituent elements.

The platform will support configurable constraints and ranking methods to identify promising material candidates.

## 9. Computational and Experimental Validation

ManganeseAI adopts a dual-validation strategy.

**Computational validation** will involve appropriate computational materials analysis, comparison with established materials databases, and evaluation of machine learning prediction accuracy.

**Experimental validation** will involve comparison with published electrochemical measurements and, where possible, laboratory synthesis, structural characterization and electrochemical testing.

Potential experimental characterization techniques include:

- X-ray diffraction (XRD).
- Scanning electron microscopy (SEM).
- Transmission electron microscopy (TEM).
- Electrochemical impedance spectroscopy (EIS).
- Cyclic voltammetry (CV).
- Galvanostatic charge-discharge (GCD).
- Galvanostatic intermittent titration technique (GITT).

The purpose is to establish a feedback loop between computational predictions and experimental observations.

## 10. Repository Structure

The repository follows a modular Python project structure.

```text
ManganeseAI/
│
├── .devcontainer/
├── .github/
│   └── workflows/
│
├── configs/
│   ├── chemical_systems.yaml
│   ├── data_sources.yaml
│   ├── database.yaml
│   └── model_config.yaml
│
├── data/
│   ├── raw/
│   ├── processed/
│   ├── structures/
│   └── external/
│
├── database/
│   ├── schema.sql
│   └── migrations/
│
├── docs/
│
├── notebooks/
│
├── scripts/
│
├── src/
│   └── manganeseai/
│       ├── data_collection/
│       ├── database/
│       ├── preprocessing/
│       ├── structures/
│       ├── descriptors/
│       ├── machine_learning/
│       ├── explainability/
│       ├── optimization/
│       └── visualization/
│
├── tests/
│
├── app/
│
├── pyproject.toml
├── README.md
├── LICENSE
└── CONTRIBUTING.md
```

## 11. Installation and Development

ManganeseAI is designed for development using GitHub Codespaces, with support for local Python environments and cloud-based scientific computing.

## Materials Project collection

The project includes a bounded Materials Project summary-data connector. Set
`MP_API_KEY` as an environment variable or Codespaces secret, initialize the
database, and start with a small dry run:

```bash
python scripts/initialize_database.py
python scripts/collect_materials_project.py \
  --dry-run --limit 5 --elements Mn \
  --include-structures --include-properties
```

See [the integration guide](docs/materials_project_integration.md) for
credential setup, fields, provenance, limits and a limited import command.
Never commit API keys or generated source snapshots.

### Phase 2 Materials Project discovery

A Priority A/B exact-chemical-system discovery dry-run is documented in the
[Phase 2 dry-run report](docs/reports/phase2_materials_project_dry_run.md).
The proposed 70-record batch is awaiting review; no Phase 2 records have been
ingested, and the production database has not been modified. See the
[candidate manifest](docs/reports/phase2_collection_manifest.md) and
[discovery strategy](docs/reports/phase2_materials_discovery_strategy.md).

### GitHub Codespaces

1. Open the ManganeseAI repository.
2. Select **Code → Codespaces**.
3. Create or open a Codespace.
4. Allow the development container to initialize.
5. Open the integrated terminal.

### Install the Project

The project is standardized on Python 3.11. The Codespaces development
container selects this version and installs the exact dependency set from
`uv.lock`.

```bash
uv sync --locked --extra dev
```

Pymatgen is a required dependency because formula normalization and elemental
composition validation use its chemical composition parser.

### Initialize and Inspect the Database

```bash
uv run --locked python scripts/initialize_database.py
uv run --locked python scripts/inspect_database.py
```

The database defaults to `database/manganeseai.db`; set
`MANGANESEAI_DATABASE_URL` to override its SQLAlchemy URL. Initialization is
repeatable and does not remove existing records. See
[docs/database_schema.md](docs/database_schema.md) for the schema, provenance
rules and command details.

### Run the Tests

```bash
uv run --locked pytest
```

### Launch the Dashboard

```bash
streamlit run app/streamlit_app.py
```

The dashboard and other platform modules are developed separately from the
scientific database.

## 12. Development Roadmap

ManganeseAI will be developed incrementally.

| Phase | Development Objective |
|---|---|
| Phase 1 | GitHub repository and computational environment |
| Phase 2 | Scientific database architecture |
| Phase 3 | External materials database integration |
| Phase 4 | Automated data collection and validation |
| Phase 5 | Materials processing and descriptor generation |
| Phase 6 | Initial machine learning models |
| Phase 7 | Explainable AI implementation |
| Phase 8 | Multi-objective materials optimization |
| Phase 9 | Interactive materials discovery dashboard |
| Phase 10 | Computational and experimental validation |

## 13. Reproducibility and Data Integrity

Scientific reproducibility is a fundamental principle of ManganeseAI.

The platform will implement:

- Traceable data provenance.
- Documented data-processing procedures.
- Reproducible computational workflows.
- Version-controlled source code.
- Consistent property units.
- Separation of experimental and computational datasets.
- Automated data validation.
- Model evaluation and uncertainty reporting.

No material property should be treated as experimentally verified unless supported by an appropriate experimental source.

Missing values must not be replaced with fabricated measurements.

## 14. Project Status

**Development stage:** Initial infrastructure and platform development.

ManganeseAI is currently under active development. Its database, automated data-collection pipeline, computational modules and machine learning framework are being established.

Predictions and candidate rankings will require appropriate validation before being interpreted as reliable materials discoveries.

## 15. Long-Term Vision

The long-term vision of ManganeseAI is to establish an accessible, scientifically interpretable and reproducible AI-guided materials discovery platform.

By integrating materials databases, computational science, machine learning, explainable AI and experimental validation, the platform aims to accelerate the discovery of next-generation manganese-based cathodes for safer, affordable and sustainable aqueous zinc-ion energy storage technologies.

Ultimately, ManganeseAI seeks to transform how manganese-based battery materials are explored, evaluated and optimized.

---

## 16. Acknowledgement and Contributions

ManganeseAI is a developing scientific research and software initiative.

Contributions involving materials science, computational chemistry, crystallography, electrochemistry, machine learning and scientific software development are welcome.

Please use GitHub Issues and Pull Requests to propose improvements, report bugs and contribute to the platform.

## 17. Citation

A formal software citation and research publication reference will be added when the project reaches its first documented scientific release.

---

**ManganeseAI — Explainable Intelligence for Sustainable Battery Materials Discovery.**
