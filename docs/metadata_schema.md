## Metadata Schema: Variable Definitions and Controlled Vocabularies

> **Version:** 1.0  
> **Maintainer:** AMIA NLP Working Group

---

## Overview

This schema defines the 33 standardized metadata variables used in the AMIA NLP Working Group Clinical & Biomedical NLP Dataset Registry. Each entry includes the variable definition, accepted values or controlled vocabulary, and an illustrative example.

Missing values should be recorded as `N/A` rather than left blank.

---

### 1. Dataset Name
- **Definition:** The name used for indexing and citation within the registry. Typically the short or canonical name by which the dataset is commonly known.
- **Example:** `MIMIC-III Clinical Notes` · `n2c2 2018 ADE`

---

### 2. Title / Official Name
- **Definition:** Full formal name of the corpus or dataset as used in the primary publication or repository landing page.
- **Example:** `Medical Information Mart for Intensive Care III`

---

### 3. Persistent Identifier (PID)
- **Definition:** A stable, globally unique identifier that permanently resolves to the dataset, such as a DOI or PhysioNet accession number.
- **Accepted values:** DOI string, accession number, URL-based persistent identifier; `N/A` if none exists.
- **Example:** `10.13026/C2XW26` · `N/A`

---

### 4. Domain
- **Definition:** Primary biomedical or clinical domain of the dataset.
- **Examples:** `Intensive Care` · `Radiology` · `Oncology` · `General Medicine` · `Pathology` · `Psychiatry`

---

### 5. Document / Source Type
- **Definition:** Type(s) of clinical or biomedical documents included in the dataset.
- **Examples:** `Discharge summaries` · `Progress notes` · `Radiology reports` · `Pathology reports` · `SOAP notes` · `Biomedical literature abstracts`

---

### 6. Clinical Setting
- **Definition:** Healthcare setting in which the source data were collected.
- **Controlled vocabulary:**

| Value | Description |
|-------|-------------|
| `ICU` | Intensive care unit |
| `Inpatient` | General inpatient / hospital ward |
| `Outpatient` | Ambulatory / clinic setting |
| `Emergency Department` | ED / urgent care |
| `Radiology` | Imaging and radiology services |
| `Pathology` | Pathology and lab reports |
| `Multi-setting` | Spans multiple care settings |
| `N/A` | Setting not applicable or not reported |

---

### 7. Short Name / Acronym
- **Definition:** Abbreviated label commonly used to reference the dataset in the literature.
- **Example:** `MIMIC-III` · `n2c2 2018` · `i2b2/VA`

---

### 8. Number of Documents / Notes
- **Definition:** Total count of documents, notes, or records in the dataset.
- **Example:** `53,423 notes` · `~2,000 discharge summaries` · `Not reported`

---

### 9. Authors / Curators / Contributors
- **Definition:** Individuals or teams who created, annotated, or maintain the dataset.
- **Example:** `Johnson et al.; MIT Lab for Computational Physiology`

---

### 10. Institution / Hosting Organization
- **Definition:** Organization responsible for hosting or stewardship of the dataset.
- **Example:** `MIT / PhysioNet` · `Harvard Medical School` · `Hugging Face`

---

### 11. Note Section / Subtype
- **Definition:** Specific sections or subtypes within clinical documents, if the dataset targets particular note parts.
- **Examples:** `HPI, Assessment, Plan, Medications` · `Findings` · `Impression` · `N/A`

---

### 12. Language(s)
- **Definition:** Primary language(s) of the documents in the dataset.
- **Controlled vocabulary:**

| Value | Notes |
|-------|-------|
| `English` | |
| `Chinese` | Specify Simplified or Traditional if known |
| `Spanish` | |
| `Portuguese` | Specify regional variant if known |
| `French` | |
| `German` | |
| `Multilingual` | Two or more languages; list all |
| `Other` | Specify language name |

---

### 13. Time Period / Collection Date Span
- **Definition:** Temporal range during which the source data were collected.
- **Example:** `2001–2012` · `2010–2020` · `Not reported`

---

### 14. Annotation Types / Levels / Tasks
- **Definition:** The NLP task(s) or annotation layers supported by the dataset.
- **Controlled vocabulary (select all that apply):**

| Value | Description |
|-------|-------------|
| `NER` | Named entity recognition |
| `Relation Extraction` | Binary or n-ary relations between entities |
| `Coreference Resolution` | Entity coreference chains |
| `Text Classification` | Document- or sentence-level labels |
| `De-identification` | PHI / PII removal annotation |
| `ICD Coding` | Diagnostic or procedure code assignment |
| `Temporal Extraction` | Event and time expression extraction |
| `Section Segmentation` | Identifying note sections |
| `Assertion / Negation` | Negation, uncertainty, experiencer annotation |
| `Summarization` | Abstractive or extractive summarization |
| `QA` | Question answering |
| `Multi-task` | Multiple of the above |

- **Example:** `NER, Relation Extraction, Assertion / Negation`

---

### 15. Annotation Schema / Ontologies / Vocabularies
- **Definition:** Annotation standards, schemas, or terminologies used to define entity types, relation categories, or label sets.
- **Examples:** `UMLS` · `SNOMED CT` · `ICD-10` · `i2b2 schema` · `BRAT standoff format`

---

### 16. Annotation Quality / Inter-annotator Agreement / Kappa / F1
- **Definition:** Reported reliability metrics for the annotation process, if available.
- **Examples:** `Inter-annotator Kappa = 0.85` · `micro-F1 = 0.78` · `Not reported`

---

### 17. Training / Test Split / Partitioning
- **Definition:** Whether the corpus is partitioned into train/dev/test subsets, and the sizes of each partition.
- **Example:** `80% train / 10% dev / 10% test; 40k / 5k / 5k notes` · `No official split provided`

---

### 18. Processing / Pre-processing / DEID
- **Definition:** Transformations applied to the raw data prior to release, including de-identification methods, text normalization, tokenization, or sectioning.
- **Examples:** `HIPAA Safe Harbor de-identification` · `Philter rule-based PHI scrubbing` · `Tokenized and lowercased` · `None reported`

---

### 19. Version
- **Definition:** Version number or release tag of the dataset. If versioning is not formally tracked, record the release date.
- **Example:** `v1.0` · `v2025-05-01` · `N/A`

---

### 20. Last Update
- **Definition:** Date or year when the dataset or its current version was most recently made public or updated.
- **Example:** `2024` · `2018-06-15` · `Not reported`

---

### 21. Access / Use Conditions
- **Definition:** Overall access classification and any restrictions on use.
- **Controlled vocabulary:**

| Value | Description |
|-------|-------------|
| `Open` | Freely downloadable without credentialing |
| `Restricted` | Requires credentialing, DUA, or IRB approval |

- **Examples:** `Open access (CC BY 4.0)` · `Requires DUA & IRB approval`

---

### 22. Access Mechanism
- **Definition:** Specific pathway to obtain the dataset.
- **Example:** `PhysioNet credentialed access portal` · `Request form via n2c2 portal` · `Direct download from GitHub`

---

### 23. Citation / Reference
- **Definition:** Primary publication(s) describing the dataset, formatted as a bibliographic reference.
- **Example:** `Johnson et al. (2016). MIMIC-III, a freely accessible critical care database. Scientific Data, 3, 160035.`

---

### 24. Related Datasets / Dependencies
- **Definition:** Other datasets that this corpus builds upon, overlaps with, or depends on.
- **Example:** `Derived from MIMIC-III Clinical Notes` · `Overlaps with i2b2 2010 corpus` · `N/A`

---

### 25. Use Cases / Known Applications
- **Definition:** NLP tasks or research applications for which the dataset has been used or is designed.
- **Examples:** `Medication extraction` · `Clinical phenotyping` · `De-identification model training` · `Outcome prediction`

---

### 26. Limitations / Caveats
- **Definition:** Known biases, coverage gaps, constraints, or risks associated with the dataset.
- **Example:** `Adult ICU patients only; limited generalizability to outpatient settings; lacks rare disease representation`

---

### 27. License / Terms of Use
- **Definition:** Explicit licensing terms governing reuse and redistribution.
- **Examples:** `CC BY 4.0` · `CC BY-NC-ND 4.0` · `PhysioNet Credentialed Health Data License 1.5.0` · `Non-commercial use only`

---

### 28. Ethics / IRB / Privacy Protections
- **Definition:** Description of ethical approvals and privacy safeguards applied to the dataset.
- **Examples:** `HIPAA Safe Harbor de-identification; IRB waiver granted` · `PHI scrubbed via rule-based tool` · `Not reported`

---

### 29. Format / File Types / Schema
- **Definition:** Data storage formats, file structures, and schema specifications.
- **Examples:** `Plain text + XML (BRAT standoff)` · `JSON` · `CoNLL` · `BIO-tagged TSV` · `CSV`

---

### 30. Encoding / Character Set
- **Definition:** Character encoding used for textual data files.
- **Example:** `UTF-8` · `ASCII` · `N/A`

---

### 31. Reuse / Interoperability Tools / Code
- **Definition:** Accompanying tools, APIs, loading scripts, or conversion utilities provided with or for the dataset.
- **Example:** `Python loader script` · `BRAT-to-JSON converter` · `Hugging Face datasets loader` · `N/A`

---

### 32. Repository / Hosting / Mirror URLs
- **Definition:** Official URL(s) where the dataset is hosted, including mirrors or archival copies.
- **Example:** `https://physionet.org/content/mimiciii/` · `https://huggingface.co/datasets/...`

---

### 33. Indicating Whether Data Is Used by LLM Training / Data Leakage
- **Definition:** Indication of whether the dataset is known or suspected to have been included in LLM pre-training corpora, and associated data contamination or leakage risks.
- **Controlled vocabulary:**

| Value | Description |
|-------|-------------|
| `Yes` | Confirmed or highly likely used in LLM training |
| `Possibly` | Suspected but unconfirmed |
| `No` | Confirmed not used; restricted access prevents inclusion |
| `Unknown` | Insufficient information to assess |

---

## FAIR Alignment Summary

| FAIR Principle | Supported By |
|----------------|-------------|
| **Findability** | Persistent Identifier (PID), Dataset Name, Title / Official Name, Domain |
| **Accessibility** | Access / Use Conditions, Access Mechanism, Repository / Hosting URLs |
| **Interoperability** | Annotation Schema / Ontologies, Format / File Types, Encoding / Character Set |
| **Reusability** | License / Terms of Use, Ethics / IRB, Limitations / Caveats, Citation / Reference |

---

## Schema Governance Notes

- Fields with a **controlled vocabulary** table must use only the listed values.
- Missing values must be recorded as `N/A`; blank cells are not permitted.
- All public metadata entries are released under **CC BY 4.0**.
