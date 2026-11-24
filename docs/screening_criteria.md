# AMIA NLP Working Group — Clinical & Biomedical NLP Dataset Registry
## Screening Criteria: Inclusion and Exclusion Criteria

> **Version:** 1.1  
> **Date:** November 2026  
> **Maintainer:** AMIA NLP Working Group

---

## Overview

Each candidate dataset identified through the systematic search and community contribution process was screened against the criteria below before proceeding to metadata abstraction. Screening was applied consistently across all sources, including PhysioNet, Hugging Face, n2c2, and community-contributed entries.

---

## Inclusion Criteria

A dataset must meet **all** of the following criteria to be retained:

**I1. Accessibility**  
The dataset is accessible to the public, either through open access (freely downloadable) or controlled access with a clear, documented request process (e.g., credentialed access, Data Use Agreement).

**I2. Clinical or Biomedical Focus**  
The dataset is clinically or biomedically focused (e.g., clinical notes, discharge summaries, radiology reports, pathology reports, biomedical literature).

**I3. NLP Task Relevance**  
The dataset is designed for, or has been used in, at least one NLP task, including but not limited to named entity recognition (NER), relation extraction, text classification, question answering (QA), summarization, de-identification, ICD coding, or temporal extraction.

**Multimodal resources.** A small number of multimodal resources (speech, imaging, sensor, or physiological signals) are also retained. For these resources, task type and annotation granularity reflect their prediction targets and units (e.g., recording- or patient-level labels) rather than NLP tasks or textual annotations, and they are reported as separate data modalities.

---

## Exclusion Criteria

A dataset is excluded if it meets **any** of the following criteria:

**E1. Proprietary or Inaccessible**  
The dataset is proprietary, has no documented access pathway, or cannot be obtained by researchers outside the originating institution.

**E2. Outside the Clinical or Biomedical Domain**  
The dataset is a general-domain corpus (e.g., newswire, social media, or Wikipedia content) without a clinical or biomedical focus.

---

## Datasets with Limited Documentation

Publicly accessible datasets with limited documentation (e.g., no dataset card, publication, or license) are **retained** rather than excluded, so that documentation gaps can be characterized. Their missing information is recorded as undocumented in the metadata table and is reflected in the FAIR-aligned metadata completeness assessment.

---

## Application of Criteria

Screening was applied during the initial candidate review phase. After screening, **60 datasets** were retained for metadata abstraction.

Where a dataset presented borderline eligibility (e.g., partial text content, indirect NLP relevance), final inclusion decisions were made through Working Group discussion and recorded in the reviewer notes field.

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | Mar 2026 | Initial criteria based on Process Documentation v1.0 |
