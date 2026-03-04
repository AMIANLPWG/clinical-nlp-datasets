# clinical-nlp-datasets
A standardized, community-maintained catalog of clinical and biomedical NLP datasets curated by the AMIA NLP Working Group, following a 30+ variable FAIR-aligned metadata framework.

# Clinical & Biomedical NLP Dataset Registry

> A FAIR-aligned, community-maintained catalog of clinical and biomedical NLP datasets,
> curated by the **AMIA NLP Working Group**.

---

## Quick Access


|                          |                                                                                                                                 |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------- |
| 📊**Browse Datasets**    | [View Full Metadata Table (Google Sheets)](https://docs.google.com/spreadsheets/d/1_quhlfDgXRP2lY-JS3J0PYMrO5t1Bb8yY0koeR6gDwo) |
| 🔍**Interactive Search** | [Search & Filter Datasets](https://github.com/AMIANLPWG/clinical-nlp-datasets/blob/main/index.html)                                                 |
| ➕**Suggest a Dataset**  | [Open an Issue](../../issues/new?template=dataset_submission.md)                                                                |
| 📄**Cite This Work**     | [Citation](#citation)                                                                                                           |

---

## About This Project

Clinical NLP research depends on annotated datasets, yet these resources are scattered across repositories, described inconsistently, and difficult to compare. This project addresses that gap by establishing a **standardized metadata framework** and curating a **searchable, community-maintained catalog** of clinical and biomedical NLP datasets.

This initiative was launched by the AMIA Natural Language Processing Working Group and is being promoted through collaboration across multiple institutions. The directory currently includes over 60 publicly available clinical and biomedical NLP datasets, comprising various text sources such as ICU clinical notes, radiology reports, biomedical literature, and other EHR-related documents.

**Two parallel deliverables are in development:**

- **White Paper** — Describing the metadata framework, FAIR alignment, and best practices for clinical NLP data documentation
- **Benchmark Paper** — A multi-site annotated dataset establishing community standards for clinical NLP evaluation

---

## Catalog at a Glance


| Metric                         | Count                                                                                               |
| ------------------------------ | --------------------------------------------------------------------------------------------------- |
| Datasets cataloged             | **60**                                                                                              |
| NLP tasks covered              | NER, Relation Extraction, QA, Summarization, ICD Coding, De-identification, Clinical Trial Matching |
| Metadata variables per dataset | **30+**                                                                                             |
| Languages covered              | English                                                                                             |
| Last updated                   | Mar 2026                                                                                            |

**Dataset landscape highlights:**

- Domain concentration: Radiology (8) and ICU (7) are the most represented specialized settings.
- Access fragmentation: Open (11), DUA-based (10), Mixed/Unclear (42).
- Task gap: NER and information extraction dominate; summarization, temporal reasoning, and clinical trial matching remain underrepresented.

---

## Metadata Framework

Each dataset is documented using **30+ FAIR-aligned metadata variables**, organized into six categories:


| Category                       | Key Variables                                                  |
| ------------------------------ | -------------------------------------------------------------- |
| **Basic Information**          | Dataset Name, Institution, DOI/URL, Citation, Related Datasets |
| **Clinical & Content Context** | Domain, Clinical Setting, Document Type, Language, Time Period |
| **Annotation & Labeling**      | Annotation Types, Schema/Ontologies, Inter-annotator Agreement |
| **Data Processing**            | Preprocessing/De-identification, Train/Test Split, Limitations |
| **Technical Specifications**   | Format, Encoding, Version, Repository URLs, Tools/Code         |
| **Access, Ethics & Legal**     | Access Conditions, Access Mechanism, License, IRB/Privacy      |

The framework is aligned with [FAIR data principles](https://www.go-fair.org/fair-principles/) (Findable, Accessible, Interoperable, Reusable) to support reproducible clinical NLP research.

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
│       └── dataset_submission.yml  # Structured template for dataset submissions
│
├── data/
│   ├── datasets.csv              # Full metadata table (machine-readable)
│   └── datasets_summary.csv      # Key fields only (quick reference)
│
├── docs/
│   ├── metadata_schema.md        # Metadata field definitions and controlled vocabularies
│   └── screening_criteria.md     # Dataset inclusion and exclusion criteria
│
├── dataset_visualization.html    # Interactive FAIR metadata visualization
├── index.html                    # GitHub Pages entry point for browsing datasets
```

---

## Data Collection Methodology

Datasets were identified through a **concept-based landscape-mapping strategy** using six predefined search categories:

- *clinical NLP dataset*
- *biomedical text annotation*
- *clinical named entity recognition dataset*
- *clinical relation extraction corpus*
- *medical natural language processing shared task*
- *electronic health record (EHR) NLP*

Because major clinical NLP repositories have limited support for structured Boolean queries, identification relied on platform-specific keyword searches, category-based filtering, manual review of shared task collections, and iterative expert input from AMIA NLP Working Group members.

**Inclusion criteria:** publicly accessible (open or controlled access), focused on clinical or biomedical text, relevant to NLP tasks (NER, classification, QA, summarization, information extraction).

**Exclusion criteria:** proprietary or inaccessible datasets, non-clinical corpora, resources lacking sufficient documentation to support reuse.

→ Full methodology: [`docs/process_documentation.md`](docs/process_documentation.md)

---

## Quality Assurance

To ensure metadata accuracy, about 10% of datasets undergo independent double review. Discrepancies are resolved through structured discussions, with predefined thresholds guiding whether to proceed, refine definitions, or perform a broader re-review.

---

## How to Contribute

We welcome contributions from the AMIA NLP community and beyond.

**To suggest a new dataset:**

1. Check that the dataset meets our [inclusion criteria](docs/screening_criteria.md)
2. Open an [issue](../../issues/new?template=dataset_submission.md) using our dataset submission template
3. Or submit a pull request with a completed row in `data/datasets.csv`

Contributions are reviewed by the working group admin team. See [`CONTRIBUTING.md`](CONTRIBUTING.md) for detailed instructions.

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

This project was developed collaboratively by contributors from **N institutions** through the [AMIA NLP Working Group](https://www.amia.org/communities/natural-language-processing).

---

## License

The metadata catalog is released © 1999 by <a href="https://example.com">Jane Doe</a> is licensed under <a href="https://creativecommons.org/licenses/by/4.0/">CC BY 4.0</a><img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;">. Individual datasets retain their own licenses — please consult each dataset's access conditions before use.

---

*This repository is maintained by the AMIA NLP Working Group. For questions, open an issue or contact the working group.*
