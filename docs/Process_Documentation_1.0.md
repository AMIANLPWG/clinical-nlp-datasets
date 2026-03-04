**Process Documentation**

*AMIA NLP Working Group*

**Version**: 1.0

**Date**: January 2026

**Project Goal**: Establish a FAIR, reproducible framework for clinical
and biomedical NLP datasets and curate a transparent metadata repository

# **1. Project Overview**

## **1.1 Background**

This project addresses a critical need for standardized documentation of clinical NLP data. The framework supports dataset discovery and reuse for the AMIA NLP community and establishes a foundation for reproducible clinical NLP research.

## **1.2 Scope Definition**

The project scope has been refined from broad NLP resources to focused
clinical and biomedical NLP data sources, ensuring relevance and
manageability.

## **1.3 Dual Deliverable Strategy**

1.  **White Paper:** Metadata-driven publication providing theory and
    guidance on clinical NLP data standards and best practices

2.  **Benchmark Paper:** Multi-site annotated dataset establishing
    community standards for clinical NLP evaluation

**2. Data Collection Methodology**

**2.1 Systematic Search**

Our approach, based on our prior reviews of NLP methodologies, applies a
concept-based dataset landscape-mapping strategy to identify and
organize clinical NLP datasets.

Unlike bibliographic databases such as PubMed or Scopus, major clinical NLP data repositories offer limited support for structured Boolean queries. Consequently, dataset identification relied on platform-specific strategies, including free-text keyword searches, category-based filtering using platform taxonomies, manual review of shared task collections, and iterative expansion guided by expert advice within the AMIA NLP Working Group.

Six predefined concept-level categories guided the search process:

*clinical NLP dataset*

*biomedical text annotation*

*clinical named entity recognition dataset*

*clinical relation extraction corpus*

*medical natural language processing shared task*

*electronic health record (EHR) NLP*

## **2.2 Community contribution and feedback**

To enhance recall beyond the initial search:

-   The candidate list was shared with members of the AMIA NLP Working
    Group.

-   Community members contributed additional datasets based on their
    domain expertise and prior experience.

-   Duplicate entries were merged.

This combined approach (systematic search + expert augmentation) was
used to balance coverage and feasibility.

# **3. Screening and Eligibility Criteria**

Each candidate dataset was screened using the following criteria:

**Inclusion Criteria**

-   Accessible to the public (open or controlled access with a clear
    request process)

-   Focused on clinical or biomedical text data

-   Relevant to NLP tasks (e.g., NER, classification, QA, summarization,
    information extraction)

**Exclusion Criteria**

-   Proprietary or inaccessible datasets

-   Non-clinical datasets (e.g., general-domain NLP corpora)

-   Resources lacking sufficient documentation to support reuse

After screening, approximately 45--50 datasets were retained for
metadata abstraction.

# **4. Metadata Framework Development**

## **4.1 FAIR Principles Alignment**

The metadata framework was designed to align with FAIR (Findable,
Accessible, Interoperable, Reusable) data principles:

-   **Findable:** Persistent identifiers, comprehensive metadata,
    searchable repository

-   **Accessible:** Clear access protocols, license information, and
    contact details

-   **Interoperable:** Standardized vocabularies, format specifications,
    data schemas

-   **Reusable:** Clear provenance, usage licenses, version control,
    ethical documentation

## **4.2 Comprehensive Metadata Variables**

**Current Status:** 30+ FAIR-aligned metadata variables established

Key metadata categories include:

  ---------------- ---------------------------------------------------------
  **Category**     **Examples**

  Basic            Dataset Name, Institution, DOI/URL, Citation, Related
  Information      Datasets

  Clinical &       Domain, Clinical Setting, Document Type, Language, Time
  Content Context  Period

  Annotation &     Annotation Types, Annotation Schema/Ontologies,
  Labeling         Annotation Quality

  Data Processing  Preprocessing/DEID, Train/Test Split, Limitations

  Technical        Format, Encoding, Version, Last Update, Repository URLs,
  Specifications   Tools/Code

  Access, Ethics & Access Conditions, Access Mechanism, License,
  Legal            Ethics/IRB/Privacy
  ---------------- ---------------------------------------------------------

**5. Metadata Abstraction Process**

## **5.1 Primary Abstraction**

-   Each included dataset was assigned to a contributor.

-   Contributors extracted metadata directly from primary
    sources (dataset documentation, original publications, and
    repository pages).

-   Metadata entries were recorded in a shared master table using
    standardized definitions.

## **5.2 Consolidation and Cleaning**

-   Inconsistent entries and missing values were reviewed.

-   Multimodal or non-text datasets were re-evaluated and, where
    appropriate, removed to maintain scope of consistency.

-   Naming conventions and categorical values were harmonized.

## **5.3 Data Cleaning Phase**

Post-abstraction cleaning included:

-   Review of multimodal and non-textbook datasets for scope alignment

-   Identification and resolution of missing metadata

-   Standardization of terminology and formatting

-   Consolidation of duplicate or variant datasets

# **6. Quality Assurance Process**

## **6.1 Double Review Strategy**

To assess abstraction reliability, a random sample of approximately
**10%** of datasets will undergo an independent double review. Reviewers
will independently re-abstract metadata using the same template, blinded
to the original entries.

## **6.2 Agreement Analysis**

Inter-reviewer agreement will be assessed using:

-   Percentage agreement for categorical and binary variables

-   Cohen's kappa for selected categorical variables to adjust for
    chance agreement

-   Element-level analysis to identify metadata fields with higher or
    lower consistency

## **6.3 Adjudication Plan**

Discrepancies identified during double review will be resolved through
structured discussion. Depending on agreement levels:

-   **High agreement (\>90%):** proceed with minor clarifications

-   **Moderate agreement (70--90%):** refine definitions and expand
    quality checks

-   **Low agreement (\<70%):** conduct broader re-review and revise
    abstraction guidelines

# **7. Community Repository and Maintenance**

## **7.1 GitHub Repository Structure**

The repository will include:

-   **Metadata Table:** Comprehensive spreadsheet with all dataset
    metadata

-   **Documentation:** README, contributing guidelines, code of conduct

-   **Process Documents:** This document and the metadata framework
    specification

-   **Visualization Scripts:** Code for generating summary statistics
    and visualizations

-   **Issue Templates:** Standardized forms for dataset submissions and
    corrections

## **7.2 Community Contribution Model**

The repository is designed as a living resource:

-   Community members can submit new datasets via pull requests

-   Assigned admins review and approve contributions

-   Regular maintenance and updates by the working group

-   Version control tracks all changes over time

## **7.3 Governance and Maintenance**

-   Create an NLP Working Group Gmail account for repository
    administration

-   Credentials transferable to future leadership for continuity

-   Establish an admin team with update privileges

-   Quarterly reviews to ensure currency and accuracy

# **8. Appendices**

Appendix A: Quality Check Instructions for Reviewers

*Instructions will be provided separately to quality check volunteers,
including:*

-   Detailed metadata element definitions

-   Abstraction template and data entry instructions

-   Examples of completed abstractions

Appendix B: Version History

  ------------- ------------- ---------------------------------------------
  **Version**   **Date**      **Changes**

  1.0           January 2026  Initial comprehensive process documentation
                              based on project progress and meeting notes
  ------------- ------------- ---------------------------------------------
