# Primary Task Classification Criteria

Each dataset was assigned a single primary task label following a hierarchical decision process:

## Step 1: Check the original publication or dataset documentation
If the authors explicitly designate a single primary task, assign that label.

*Examples: OpenMed NER → NER; BioASQ → QA*

## Step 2: Identify a dominant task
If no explicit label exists, assign a single-task label when one task accounts for the majority of annotations, is the sole evaluation target in the original benchmark, or is reflected in the dataset name.

*Examples: MIMIC-CXR: the NLP-relevant component is radiology report generation → Summarization; MedSTS: sole task is sentence-pair similarity scoring → Classification*

## Step 3: Assign Multiple Tasks
Only when no single task is dominant — i.e., the dataset was explicitly designed for or has been equally used across two or more distinct NLP tasks — assign Multiple Tasks. If ambiguity remains after applying Steps 1 and 2, default to Multiple Tasks.

*Examples: MIMIC-III, BC5CDR*

## Notes

> **General:** "Multiple Tasks" is reserved for datasets where multi-task use is intrinsic to the dataset design, not merely possible. Incidental secondary uses do not qualify a dataset for this category.

> **Information Extraction tasks:** Datasets designed primarily for entity and relation extraction as a unified information extraction benchmark (e.g., RadGraph, RadGraph-XL) are classified as Multiple Tasks, as the two subtasks are intrinsically coupled and neither is singularly dominant.
