# Shared Task

ReNeuIR 2024 will have an shared task to collect and measure neural IR systems to foster the development of new IR measures that incorporate efficiency and effectiveness. 

~~The methodology of the shared task was developed in the first two iterations of ReNeuIR, using (1) a unified hardware/execution environment, (2) delegating effectiveness evaluation to existing evaluation tools and relevance judgments, and (3) ensuring that submitted systems follow a standardized workflow.~~

## Synopsis

The shared task invites retrieval pipelines (or parts thereof) that follow an expected pipeline to (1) index, (2) retrieve, (3) and re-rank different workloads sampled from [ir_datasets](https://ir-datasets.com/) while we monitor their execution on [TIRA](https://www.tira.io) / [TIREx](https://www.tira.io/tirex) with [Scaphandre](https://github.com/hubblo-org/scaphandre). Participants can submit their retrieval pipelines as source code repositories or as Docker images. We encourage code submissions where participants organize their code in (private) GitHub repositories~~and use prepared Github Actions to dockerize, test, and upload submissions. To improve reproducibility, all resources must be included in the Docker image, therefore, submissions are executed in a sandbox without internet connection (the GitHub Action tests that the Docker image works without internet connection on a small unit test dataset).~~

We run the uploaded templates on different datasets derived from the MS MARCO passage dataset. We vary the number of queries and passages to be indexed to cover different workloads. We reuse the MS MARCO passage dataset to lower the barrier to entry, as many retrieval systems already exist for this test collection, allowing participants to focus on efficiency. With this in mind, for the first iteration of the shared task in 2024, we focus on submitting pre-trained systems that batch-process the entire dataset. After the shared task, we will make all collected run files together with Scaphandre traces of their execution available to foster the development of new measures that incorporate efficiency and effectiveness.

## Important Dates

Submissions to the shared task are centered around the workshop. We will have an oral presentation deadline before the workshop, so that approaches submitted by that deadline can present their submissions at the workshop, and a final proceedings deadline that welcomes existing and potentially new submissions after the workshop that will be included into the workshop proceedings.

Oral Presentation deadline: **June 26, 2024**

Workshop: **July 18, 2024**

Final Proceedings Deadline: **July 31, 2024**

All deadlines are 11.59 pm UTC -12h (“Anywhere on Earth”).

## Baselines

We encourage submissions that follow an (1) index, (2) retrieve, (3) and re-rank pipeline where participants can also submit only parts of a complete pipeline (e.g., indexing and retrieval vs. re-ranking). We make [baselines available](https://github.com/reneuir/reneuir-code/tree/main/sigir24/baselines), specifically for [(1) indexing](https://github.com/reneuir/reneuir-code/tree/main/sigir24/baselines/indexing), [(2) retrieval](https://github.com/reneuir/reneuir-code/tree/main/sigir24/baselines/retrieval), and [(3) re-ranking](https://github.com/reneuir/reneuir-code/tree/main/sigir24/baselines/re-ranking).

## Submission Instructions

We will use TIREx for submissions, submissions are open at [https://www.tira.io/task-overview/reneuir-2024](https://www.tira.io/task-overview/reneuir-2024). We provide a [step-by-step tutorial on how to submit](https://github.com/reneuir/reneuir-code/blob/main/sigir24/tutorials) and a [set of baselines](https://github.com/reneuir/reneuir-code/tree/main/sigir24/baselines). Please do not hesitate to contact us in case of questions and/or problems.

## Contact

For any questions please do not hesitate to contact us via [the forum](https://www.tira.io/c/reneuir)
or via mail at reneuir2024 [at] easychair [dot] org.
