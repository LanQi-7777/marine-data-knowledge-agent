# Agent-assisted Marine Data Knowledge Framework



This repository is the supporting GitHub repository for a manuscript currently under review and provides the prototype implementation of the agent-assisted marine data knowledge framework described in the paper.



The framework is designed to support multidisciplinary marine data discovery, evidence retrieval, dataset comparison, and reuse-oriented decision support. It is intended as a research-support workflow built on top of the reviewed data catalogue and evaluation indicators, rather than as a new marine observational dataset, a new foundation model, or a task-specific predictive model.



## Related paper



This repository accompanies the manuscript:



**Multidisciplinary marine data resources for data-driven research: a cross-domain data review, comparative assessment, and agent-assisted knowledge framework**



**Authors:** Yuqi Shao, Zhensheng Shi, and Haiyong Zheng



The manuscript reviews and compares representative marine data resources across major marine domains, including marine meteorology and climate, marine geology and bathymetry, ocean observation and biogeochemical profiles, marine biodiversity, marine ecological environment and pollution, fisheries and aquaculture, and supporting geospatial and integrated marine data infrastructures.



This repository provides supporting materials for the agent-assisted marine data knowledge framework described in the manuscript, including workflow files, prompt templates, catalogue metadata, and example materials for marine data discovery, evidence retrieval, dataset comparison, and reuse-oriented decision support.



## Repository status



This repository is released as a submission-stage supporting repository for the related manuscript.



At the current stage, the repository provides a prototype workflow and supporting materials to make the agent-assisted framework more transparent and reusable. The repository may be updated after peer review to reflect revisions to the manuscript, workflow design, catalogue structure, prompt templates, and evaluation indicators.



## Framework overview



The agent-assisted framework is designed to help users search, compare, and interpret marine data resources in a task-oriented way.



The current workflow focuses on four main functions:



* evidence retrieval from the structured marine data catalogue and supporting metadata;

* dataset comparison based on common evaluation indicators;

* answer generation for dataset discovery, comparison, and reuse-oriented selection;

* quality checking to reduce unsupported claims and improve evidence consistency.



The framework can be used to support questions such as:



* Which marine data products are suitable for a specific research task?

* How do different datasets compare in coverage, resolution, quality control, uncertainty, accessibility, and metadata completeness?

* Which data products are more suitable for deep-learning applications?

* What limitations should be considered before reusing a dataset?

* Which datasets can provide environmental covariates for cross-domain marine research?



The generated answers should be treated as decision-support outputs. Users should verify important dataset information against official data-provider documentation before using any data product for scientific analysis, model training, operational forecasting, or policy-related applications.



## Repository contents



* `workflows/`: Dify workflow files for the agent-assisted marine data knowledge framework.

* `prompts/`: prompt templates for evidence retrieval, dataset comparison, answer generation, quality checking, and response revision.

* `catalog/`: curated marine data catalogue, evaluation indicators, and supporting metadata.

* `examples/`: example queries and use cases for marine dataset discovery and comparison.



The exact file names and directory structure may be updated as the manuscript and repository are revised. Please check the latest repository tree before importing or adapting the workflow.



## How to use



### 1. Clone the repository



```bash id="v96nve"

git clone https://github.com/LanQi-7777/marine-data-knowledge-agent.git

cd marine-data-knowledge-agent

```



### 2. Import the workflow into Dify



Open Dify in your own environment and import the workflow file:



```text id="eem8a0"

workflows/marine_data_review.yml

```



After importing the workflow, reconnect your own model provider, embedding model, API keys, and knowledge base settings.



### 3. Load the catalogue and prompt files



Use the files in `catalog/` and `prompts/` to construct or update the knowledge base used by the workflow. The catalogue files are intended to support retrieval and comparison of representative marine data resources reviewed in the manuscript.



### 4. Test the workflow



Example questions include:



```text id="6tmosr"

Which sea-surface temperature products are suitable for marine heatwave analysis?

```



```text id="pwx97u"

Compare GEBCO, ETOPO, and SRTM15+ for seabed habitat modelling.

```



```text id="c19zff"

Which marine biodiversity datasets are suitable for deep-learning-based species distribution modelling?

```



```text id="1vthq5"

What should be considered when selecting marine data products for harmful-algal-bloom prediction?

```



```text id="ooqpg1"

Which datasets provide useful environmental covariates for fisheries and aquaculture studies?

```



## Data and copyright statement



This repository does not redistribute third-party marine data products.



Users should access the original data products from the official providers listed in the manuscript and catalogue files. The catalogue and assessment materials provided here are derived review-support resources intended to help readers inspect, compare, and reuse the information summarized in the manuscript.



API keys, proprietary model weights, private credentials, and third-party copyrighted source data are not included.



Third-party marine data products, external source materials, and official data-provider documentation are not covered by this repository license. Users should follow the original licenses, access policies, citation requirements, and usage restrictions of the corresponding data providers.



## Availability



* GitHub repository: https://github.com/LanQi-7777/marine-data-knowledge-agent



The repository may be archived through Zenodo or another long-term repository after a formal release. If an archived DOI becomes available, this section will be updated.



## Citation



If you use this repository, the workflow files, prompt templates, or catalogue materials in your research, please cite the related manuscript and the archived repository release when available.



Before formal publication, please cite the manuscript as:



```bibtex id="84kum5"

@misc{shao2026marine_data_review,

  title        = {Multidisciplinary marine data resources for data-driven research: a cross-domain data review, comparative assessment, and agent-assisted knowledge framework},

  author       = {Shao, Yuqi and Shi, Zhensheng and Zheng, Haiyong},

  year         = {2026},

  note         = {Manuscript under review},

  howpublished = {Supporting GitHub repository},

  url          = {https://github.com/LanQi-7777/marine-data-knowledge-agent}

}

```



After formal publication, this section will be updated with the final journal citation, DOI, and archived repository DOI.



## License



Please refer to the `LICENSE` file for reuse conditions.



Unless otherwise stated, the workflow files, prompt templates, catalogue metadata, and original documentation in this repository are provided for academic research and review purposes. If no formal `LICENSE` file is provided in the current submission-stage release, please contact the repository maintainer before copying, modifying, or redistributing the repository contents.



## Contact



For technical questions about this repository, workflow files, prompt templates, or catalogue structure, please open a GitHub issue.



For repository maintenance or implementation-related questions, please contact:



**Yuqi Shao**

Email: [shaoyuqi@stu.ouc.edu.cn](mailto:shaoyuqi@stu.ouc.edu.cn)



For academic questions about the related manuscript, please contact the corresponding authors:



**Haiyong Zheng**

Email: [zhenghaiyong@ouc.edu.cn](mailto:zhenghaiyong@ouc.edu.cn)



**Zhensheng Shi**

Email: [zhenshengshi@gmail.com](mailto:zhenshengshi@gmail.com)
