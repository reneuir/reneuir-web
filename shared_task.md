# Shared Task

ReNeuIR 2024 will have an shared task that aims to collect and measure neural IR systems to foster the development of new IR measures that incorporate efficiency and effectiveness. The methodology of the shared task was developed in the first two iterations of ReNeuIR, using (1) an unified hardware/execution environment, (2) handling effectiveness evaluation via existing evaluation tools and relevance judgments, and (3) ensuring that submitted systems follow a standardized workflow.

## Synopsis

The shared task invites retrieval pipelines (or parts thereof) that follow an expected pipeline to (1) index, (2) retrieve, (3) and re-rank different workloads sampled from [ir_datasets](https://ir-datasets.com/) while we monitor their execution in [TIREx](https://www.tira.io/tirex) with [Scaphandre](https://github.com/hubblo-org/scaphandre). Participants can submit their retrieval pipelines as source code repositories or as Docker images. We especially encourage code submissions where participants organize their code in (private) GitHub repositories and use prepared Github Actions to upload a submission to TIRA. The GitHub Actions dockerize a repository's code with other required resources and test if the created Docker image works on a small "unit test dataset". If that is the case, it is uploaded along with all metadata to TIRA.

Within TIRA, we run the uploaded templates on different datasets derived from the MS~MARCO passage dataset. In doing so, we vary the number of queries and passages to be indexed to cover different workloads while monitoring their execution with Scaphandre. The execution happens within the TIRA sandbox, which ensures reproducibility (e.g., all dependencies must be installed in the Docker image), and keeps the test data (i.e., test queries and documents) secret, allowing different document and query distributions to be measured. The reuse of MS~MARCO lowers the barrier to entry, as a wide range of retrieval systems already exist for this test collection, allowing participants to focus on efficiency. With this in mind, for the first iteration of the shared task in 2024, we focus on submitting pre-trained systems that batch-process the entire dataset. After the shared task, we will make all collected run files together with Scaphandre traces of their executions available to foster the development of new



## Important Dates

Oral Presentation deadline: **June 26, 2024**

Workshop: **July 18, 2024**

Final Proceedings Deadline: **July 31, 2024**

All deadlines are 11.59 pm UTC -12h (“Anywhere on Earth”).

## Baselines

We encourage submissions that follow an (1) index, (2) retrieve, (3) and re-rank pipeline where participants can also submit only parts of a complete pipeline (e.g., indexing and retrieval vs. re-ranking). We make [baselines available](https://github.com/mam10eks/reneuir-code/tree/main/sigir24/baselines), specifically for [(1) indexing](https://github.com/mam10eks/reneuir-code/tree/main/sigir24/baselines/indexing), [(2) retrieval](https://github.com/mam10eks/reneuir-code/tree/main/sigir24/baselines/retrieval), and [(3) re-ranking](https://github.com/mam10eks/reneuir-code/tree/main/sigir24/baselines/re-ranking).

## Submission Instructions

We will use TIREx for submissions, submissions are open at [https://www.tira.io/task-overview/reneuir-2024](https://www.tira.io/task-overview/reneuir-2024). We provide a [step-by-step tutorial on how to submit](https://github.com/mam10eks/reneuir-code/blob/main/sigir24/tutorials) and a [set of baselines](https://github.com/mam10eks/reneuir-code/tree/main/sigir24/baselines). Please do not hesitate to contact us in case of questions and/or problems.

## Contact

For any questions please do not hesitate to contact us via [the forum](https://www.tira.io/c/reneuir)
or via mail at reneuir2024 [at] easychair [dot] org.
