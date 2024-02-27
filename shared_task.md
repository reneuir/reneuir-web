# Shared Task

ReNeuIR 2024 hosts a shared task to foster the development efficient neural IR systems.

## Synopsis

The shared task invites the submission of retrieval pipelines (or parts thereof) that implement the follow the basic steps (1) index, (2) retrieve, (3) and re-rank. Participants can submit their retrieval pipelines in the form of source code repositories or as Docker images. We encourage code submissions where participants organize their code in (private) GitHub repositories. Submitted pipelines are then executed automatically with different workloads sampled from [ir_datasets](https://ir-datasets.com/), using [TIRA](https://www.tira.io) / [TIREx](https://www.tira.io/tirex) and [Scaphandre](https://github.com/hubblo-org/scaphandre) to measure both their effectiveness and efficiency.

More specifically, TIRA runs submitted retrieval pipelines on datasets derived from the MS MARCO passage dataset. To simulated different worklods, the number of queries and passages to be indexed are varied. By reusing the MS MARCO passage dataset, we lower the barrier to entry, as many retrieval systems already exist for this test collection, allowing participants to focus on efficiency. With this in mind, for the first iteration of the shared task in 2024, our focus is on submitting pre-trained systems that batch-process the entire dataset.

After the shared task, we will make all collected run files together with Scaphandre traces of their execution available to foster the development of new performance measures that incorporate efficiency and effectiveness.

## Important Dates

Submissions to the shared task form part of the workshop. We will have an oral presentation deadline before the workshop, so that approaches submitted by that deadline can present their submissions at the workshop, and a final proceedings deadline that welcomes existing and potentially new submissions after the workshop that will be included into the workshop proceedings.

Oral Presentation deadline: **June 26, 2024**

Workshop: **July 18, 2024**

Final Proceedings Deadline: **July 31, 2024**

All deadlines are 11.59 pm UTC -12h (“Anywhere on Earth”).

## Baselines

We encourage submissions that implement a pipeline with the steps (1) index, (2) retrieve, (3) and re-rank, where participants can also submit only parts of a complete pipeline (e.g., indexing and retrieval vs. re-ranking). We make [baselines available](https://github.com/reneuir/reneuir-code/tree/main/sigir24/baselines), specifically for [(1) indexing](https://github.com/reneuir/reneuir-code/tree/main/sigir24/baselines/indexing), [(2) retrieval](https://github.com/reneuir/reneuir-code/tree/main/sigir24/baselines/retrieval), and [(3) re-ranking](https://github.com/reneuir/reneuir-code/tree/main/sigir24/baselines/re-ranking).

## Submission Instructions

We will use TIREx for submissions. Submissions are open at [https://www.tira.io/task-overview/reneuir-2024](https://www.tira.io/task-overview/reneuir-2024). We provide a [step-by-step tutorial on how to submit](https://github.com/reneuir/reneuir-code/blob/main/sigir24/tutorials) and a [set of baselines](https://github.com/reneuir/reneuir-code/tree/main/sigir24/baselines). Please do not hesitate to contact us in case of questions and/or problems.

## Contact

For any questions please do not hesitate to contact us via [the forum](https://www.tira.io/c/reneuir)
or via mail at reneuir2024 [at] easychair [dot] org.
