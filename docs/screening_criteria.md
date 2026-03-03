# AMIA NLP Working Group — Clinical & Biomedical NLP Dataset Registry
## Screening Criteria: Inclusion and Exclusion Criteria

> **Version:** 1.0  
> **Date:** January 2026  
> **Maintainer:** AMIA NLP Working Group — Dataset Standardization Subgroup

---

## Overview

Each candidate dataset identified through the systematic search and community contribution process was screened against the criteria below before proceeding to metadata abstraction. Screening was applied consistently across all sources, including PhysioNet, Hugging Face, n2c2, and community-contributed entries.

---

## Inclusion Criteria

A dataset must meet **all** of the following criteria to be retained:

**I1. Accessibility**  
The dataset is accessible to the public, either through open access (freely downloadable) or controlled access with a clear, documented request process (e.g., credentialed access, Data Use Agreement).

**I2. Clinical or Biomedical Text Focus**  
The dataset is primarily composed of clinical or biomedical text data (e.g., clinical notes, discharge summaries, radiology reports, pathology reports, biomedical literature).

**I3. NLP Task Relevance**  
The dataset is designed for or has been used in at least one NLP task, including but not limited to: named entity recognition (NER), relation extraction, text classification, question answering (QA), summarization, de-identification, ICD coding, or temporal extraction.

---

## Exclusion Criteria

A dataset is excluded if it meets **any** of the following criteria:

**E1. Proprietary or Inaccessible**  
The dataset is proprietary, has no documented access pathway, or cannot be obtained by researchers outside the originating institution.

**E2. Non-Clinical Domain**  
The dataset belongs to the general-domain NLP corpus (e.g., newswire, social media, Wikipedia) without a clinical or biomedical focus.

**E3. Insufficient Documentation**  
The dataset lacks sufficient documentation (e.g., no publication, no README, no metadata) to support reuse or reliable metadata abstraction.

---

## Application of Criteria

Screening was applied during the initial candidate review phase. After screening, approximately **60+ datasets** were retained for metadata abstraction.

Where a dataset presented borderline eligibility (e.g., partial text content, indirect NLP relevance), final inclusion decisions were made through working group discussion and recorded in the reviewer notes field.

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | January 2026 | Initial criteria based on Process Documentation v1.0 |
