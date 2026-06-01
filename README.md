# Agent-assisted Marine Data Knowledge Base

This repository provides the prototype implementation of an agent-assisted knowledge framework for multidisciplinary marine data discovery, evidence retrieval, dataset comparison, and reuse-oriented decision support.

## Relationship to the paper

This repository supports the review article:

"Multidisciplinary marine data resources for deep-learning applications: a cross-domain data review and comparative assessment."

## Main functions

- Evidence retrieval from the structured marine data catalog
- Dataset comparison based on coverage, resolution, quality control, metadata, accessibility, interoperability, and deep-learning readiness
- User-oriented answer generation
- Quality checking and evidence verification

## Repository structure

- `workflows/`: Dify DSL workflow file
- `prompts/`: prompt templates used by the agent
- `catalog/`: curated marine data catalog and evaluation indicators

## How to use

1. Import `workflowsmarine_data_review.yml` into Dify.
2. Reconnect your own model provider and knowledge base.
3. Use Dify to test the workflow.
4. Do not upload private API keys or third-party copyrighted source data.

## Data statement

This repository does not redistribute third-party marine data products. Users should access original data from official providers listed in the paper and catalog files.

## Citation

Please cite the related paper and the archived Zenodo release.
