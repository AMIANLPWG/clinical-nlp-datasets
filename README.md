# Clinical & Biomedical NLP Dataset Registry

> A FAIR-aligned, community-maintained catalog of clinical and biomedical NLP datasets,
> curated by the **AMIA NLP Working Group** using a 33-variable metadata schema.

---

## Quick Access

|                             |                                                                                                                                 |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| 📊 **Browse Datasets**       | [View Full Metadata Table (Google Sheets)](https://docs.google.com/spreadsheets/d/1_quhlfDgXRP2lY-JS3J0PYMrO5t1Bb8yY0koeR6gDwo) |
| 🔍 **Interactive Search**    | [Search & Filter Datasets](https://amianlpwg.github.io/clinical-nlp-datasets/index.html)                                        |
| 📈 **Dataset Visualization** | [Display Visual Charts](https://amianlpwg.github.io/clinical-nlp-datasets/dataset_visualization.html)                           |
| ➕ **Suggest a Dataset**     | [Open an Issue](https://github.com/AMIANLPWG/clinical-nlp-datasets/issues/new?template=dataset_submission.yml)                  |
| 📄 **Cite This Work**        | [Citation](#citation)                                                                                                           |

---

## About This Project

Clinical NLP research depends on annotated datasets, yet these resources are scattered across repositories, described inconsistently, and difficult to compare. This project addresses that gap by establishing a **standardized metadata framework** and curating a **searchable, community-maintained catalog** of clinical and biomedical NLP datasets.

The initiative was launched by the AMIA Natural Language Processing Working Group and is developed collaboratively across multiple institutions. The catalog currently includes **60 publicly accessible datasets** (including credentialed-access resources) drawn from EHR and clinical notes, radiology reports, biomedical literature, and other clinical sources, together with a small number of multimodal resources (speech, imaging, sensor, and physiological signals).

**Related work:**

- **AMIA 2026 Annual Symposium** — podium presentation of the catalog
- **Manuscript** — describing the metadata framework, FAIR-aligned assessment, and catalog findings (in preparation)
- **Benchmark Paper** — a multi-site annotated dataset establishing community standards for clinical NLP evaluation (in development)

---

## Catalog at a Glance

| Metric                         | Value                                                                                             |
| ------------------------------ | ------------------------------------------------------------------------------------------------- |
| Datasets cataloged             | **60** (release or publication years 2010–2026)                                                    |
| Metadata variables per dataset | **33**                                                                                            |
| Most common task categories    | Multiple tasks (30), named entity recognition (10), question answering (6)                         |
| Most common data sources       | EHR/clinical text (23), biomedical literature (17), radiology/imaging (11)                         |
| Access and use conditions      | Restricted (34), open/permissive (18), license unclear (8)                                         |
| Languages                      | Mostly English (53 of 60); also Spanish, Catalan, Portuguese, German, Italian, and Chinese                             |
| Last updated                   | November 2026                                                                                     |

**Dataset landscape highlights:**

- **Care settings:** Among datasets derived from clinical care, ICU-associated resources are the largest group (13 of 34), largely MIMIC-derived, whereas emergency department data are scarce (4 of 34).
- **Access:** More than half of the datasets require credentialed access, a data use agreement, or non-commercial use; 8 have no clearly specified license.
- **Task coverage:** Summarization (2) and cohort selection (1) remain underrepresented relative to multi-task and NER resources.

---

## Metadata Framework

Each dataset is documented using **33 FAIR-aligned metadata variables**, organized into six categories:

| Category                       | Key Variables                                                  |
| ------------------------------ | -------------------------------------------------------------- |
| **Basic Information**          | Dataset Name, Institution, DOI/URL, Citation, Related Datasets |
| **Clinical & Content Context** | Domain, Clinical Setting, Document Type, Language, Time Period |
| **Annotation & Labeling**      | Annotation Types, Schema/Ontologies, Inter-annotator Agreement |
| **Data Processing**            | Preprocessing/De-identification, Train/Test Split, Limitations |
| **Technical Specifications**   | Format, Encoding, Version, Repository URLs, Tools/Code         |
| **Access, Ethics & Legal**     | Access Conditions, Access Mechanism, License, IRB/Privacy      |

The framework is aligned with the [FAIR data principles](https://www.go-fair.org/fair-principles/) (Findable, Accessible, Interoperable, Reusable) to support reproducible clinical NLP research. Sixteen documentation-related variables (four per FAIR dimension) are additionally scored for metadata completeness on a five-level scale using a predefined scoring rubric; the overall score is the mean of the 16 field scores (see the FAIR heatmap in the [visualization page](https://amianlpwg.github.io/clinical-nlp-datasets/dataset_visualization.html)).

→ See [`docs/metadata_schema.md`](docs/metadata_schema.md) for full variable definitions and controlled vocabularies.

---

## Repository Structure

```
/
├── README.md                     # Project overview and usage instructions
├── CONTRIBUTING.md               # Guidelines for contributing new datasets
│
├── .github/
│   └── ISSUE_TEMPLATE/
│       └── dataset_submission.yml   # Structured template for dataset submissions
│
├── data/
│   ├── datasets.csv              # Full metadata table (machine-readable)
│   └── datasets_summary.csv      # Key fields only (quick reference)
│
├── docs/
│   ├── metadata_schema.md                      # Metadata field definitions and controlled vocabularies
│   ├── Process_Documentation_1.0.md            # Data collection and QA methodology
│   ├── screening_criteria.md                   # Dataset inclusion and exclusion criteria
│   └── primary_task_classification_criteria.md # Rules for assigning task categories
│
├── dataset_visualization.html    # Interactive FAIR metadata visualization
└── index.html                    # GitHub Pages entry point for browsing datasets
```

---

## Data Collection Methodology

Datasets were identified through a **concept-based search strategy** on major data repositories and institutional websites (PhysioNet, Hugging Face, and n2c2), combining data-related terms (e.g., *dataset*, *corpus*, *benchmark*), clinical and biomedical terms (e.g., *clinical*, *electronic health record*), and NLP task terms (e.g., *named entity recognition*, *question answering*). Search terms were adapted to each platform's search capabilities, and additional datasets were identified through a taxonomy-based approach and recommendations from AMIA NLP Working Group members.

**Inclusion criteria:** publicly accessible (open or credentialed access), clinically or biomedically focused, and related to at least one NLP task. A small number of multimodal resources (speech, imaging, sensor, or physiological signals) are also included; for these, task type and annotation granularity reflect their prediction targets and units.

**Exclusion criteria:** proprietary or not publicly accessible datasets, and resources outside the clinical or biomedical domain. Publicly accessible datasets with limited documentation are retained so that documentation gaps can be characterized.

→ Full methodology: [`docs/Process_Documentation_1.0.md`](docs/Process_Documentation_1.0.md) and [`docs/screening_criteria.md`](docs/screening_criteria.md)

---

## Quality Assurance

All metadata are abstracted following a unified variable definition manual, with each dataset assigned to one trained Working Group member. A random 10% sample of datasets undergoes independent review by a second contributor, and disagreements are adjudicated by a third contributor using predefined criteria.

---

## How to Contribute

We welcome contributions from the AMIA NLP community and beyond.

**To suggest a new dataset:**

1. Check that the dataset meets our [inclusion criteria](docs/screening_criteria.md)
2. Open an [issue](https://github.com/AMIANLPWG/clinical-nlp-datasets/issues/new?template=dataset_submission.yml) using our dataset submission template
3. Or submit a pull request with a completed row in `data/datasets.csv`

Contributions are reviewed by the Working Group admin team before being added to the catalog. See [`CONTRIBUTING.md`](CONTRIBUTING.md) for detailed instructions.

---

## Citation

If you use this catalog or the metadata framework in your research, please cite:

```bibtex
@article{[last_name][year],
  title   = {[Paper Title]},
  author  = {[Author List]},
  journal = {[Journal]},
  year    = {[Year]},
  doi     = {[DOI]}
}
```

*Citation will be updated upon publication.*

---

## Team & Acknowledgments

This project was developed collaboratively by contributors from eight institutions through the [AMIA NLP Working Group](https://amia.org/community/working-groups/natural-language-processing).

---

## License

© 2026 AMIA NLP Working Group. The catalog metadata (`data/` and `docs/`) is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Individual datasets retain their own licenses and access conditions — please consult each dataset's terms before use.

---

*This repository is maintained by the AMIA NLP Working Group. For questions, open an issue or contact the Working Group.*
