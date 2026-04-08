# Shared Task

ReNeuIR 2026 hosts a shared task to foster the development of efficient neural IR systems.

## Synopsis

Using the [lsr-benchmark](https://github.com/reneuir/lsr-benchmark) that was developed in the previous iterations of ReNeuIR, we aim to run a large set of efficient neural retrieval systems on diverse hardware to enable IR evaluations that account for efficiency and effectiveness. All executions are tracked with the [TIREx tracker](https://github.com/tira-io/tirex-tracker) that persists efficiency metrics into the [ir_metadata format](https://www.ir-metadata.org/) so that the result of the shared task is a big collection of run files (for effectiveness evaluations) with their ir_metadata (for efficiency evaluations). We have three subtasks (1) efficiency measurements on diverse hardware, (2) neural embedding models, and (3) efficient retrieval systems.

## Task 1: Efficiency Measurements on Diverse Hardware

Do you have a computer that is idle for ca. 15 hours with Docker/Podman installed? Then please consider to participate in task 1 by running the lsr-benchmark suite. All embeddings are pre-computed and the retrieval engines are dockerized. We plan to support x86_64 and ARM64 processors (ARM64 is in progress). You can verify if your machine is supported via (**attention, this is not yet published to pypi**):

```
pip3 install lsr-benchmark
lsr-benchmark verify-installation
```

The output should look like this:

<img width="900" alt="Screenshot_20260408_185039" src="https://github.com/user-attachments/assets/20f014ab-70d8-47f8-80a2-2e1330acab1d" />

For participants of task 1, our idea is that each participant runs the same benchmarks on his/her hardware and sends back the run files (that contain the efficiency measures in the ir_metadata format). The full benchmark suite is estimated to take ca. 15 hours and requires ca. 50 GB of disk space (embeddings + docker images), you can interrupt the process in between and continue the benchmark later if you wish. You can run the full benchmark via (**attention, this is not yet published to pypi**):

```
lsr-benchmark run-retrieval-experiment reneuir-2026/full --output my-reneuir-2026-results
```

To run the efficiency/effectiveness oriented evaluation on your results, please run (assuming you have stored your results in `my-reneuir-2026-results` as in the execution above):

```
lsr-benchmark evaluate my-reneuir-2026-results
```

### Task 1 Submission Instructions

**TBD**: We will ask to upload the run files.

## Task 2: Neural Embedding Models

We aim to collect diverse embedding models into the [lsr-benchmark](https://github.com/reneuir/lsr-benchmark). So far, we mostly have lexical and learned sparse embedding models, but we also want to incorporate more embedding models. If you have an interesting embedding model (all retrieval paradigms are encouraged!), please consider to submit this model. We maintain the lsr-benchmark as a mono-repo, so that participants of task 2 can contribute their embedding model via a pull request to the [lsr-benchmark](https://github.com/reneuir/lsr-benchmark) repository. The structure of new embedding models is flexible, please have a look at existing embedding models such as [lightning-ir](https://github.com/reneuir/lsr-benchmark/tree/main/step-02-embedding-approaches/lightning-ir), [bge-m3](https://github.com/reneuir/lsr-benchmark/tree/main/step-02-embedding-approaches/bge-m3), or [lexical](https://github.com/reneuir/lsr-benchmark/tree/main/step-02-embedding-approaches/lexical) as starting point. If you want, we can include your embedding model into the `reneuir-2026/full` suite that is executed in Task 1.


### Task 2 Submission Instructions

Please create a pull request to the [lsr-benchmark](https://github.com/reneuir/lsr-benchmark). You can create an early "Draft Pull Request" to indicate on what you want to work and to get early feedback.

## Task 3: Efficient Retrieval Systems

Is your favorite retrieval system not included in the [lsr-benchmark](https://github.com/reneuir/lsr-benchmark)? We aim to collect diverse retrieval systems, so far, we mostly have systems that we have experience with but it would be very interesting to expand the number of included retrieval systems, so if your favorite retrieval system is not yet included, please consider to submit this retrieval system. We maintain the lsr-benchmark as a mono-repo, so that participants of task 3 can contribute their retrieval system via a pull request to the [lsr-benchmark](https://github.com/reneuir/lsr-benchmark) repository. The structure of new retrieval systems is flexible, please have a look at existing systems such as [seismic](https://github.com/reneuir/lsr-benchmark/tree/main/step-03-retrieval-approaches/seismic), [duckdb](https://github.com/reneuir/lsr-benchmark/tree/main/step-03-retrieval-approaches/duckdb), or [pyterrier-splade-pisa](https://github.com/reneuir/lsr-benchmark/tree/main/step-03-retrieval-approaches/pyterrier-splade-pisa) as starting point. If you want, we can include your retrieval system into the `reneuir-2026/full` suite that is executed in Task 1.


### Task 3 Submission Instructions

Please create a pull request to the [lsr-benchmark](https://github.com/reneuir/lsr-benchmark). You can create an early "Draft Pull Request" to indicate on what you want to work and to get early feedback.

## Important Dates

Submissions to the shared task form part of the workshop. We will have an oral presentation deadline before the workshop so that approaches submitted by that deadline can present their submissions at the workshop, and a final proceedings deadline that welcomes existing and potentially new submissions after the workshop, which will be included in the workshop proceedings.

Oral Presentation deadline: **TBD**

Workshop: **TBD**

Final Proceedings Deadline: **TBD**

All deadlines are 11.59 pm UTC -12h (“Anywhere on Earth”).



## Contact

For any questions, please do not hesitate to contact us via [the forum](https://www.tira.io/c/reneuir)
or via mail at reneuir2026 [at] easychair [dot] org.
