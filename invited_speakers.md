# Keynote Speakers

We are thrilled to have Omar Khattab as our
keynote speaker at the event. Below you will find the title
and abstract of Omar's talk as well as a short bio.

-------

## From BM25 to (Col)BERT to LLMs: Navigating a Maturing Efficiency-Effectiveness Tradeoff Space in Neural IR

**[Slides](assets/pdfs/ReNeuIR-keynote-v4-shared.pptx)**

**Abstract:** The past five years have dramatically transformed the landscape of IR. What began as a focus on optimizing classical models like BM25 in multi-stage architectures has evolved quickly into working with neural models many orders of magnitude larger. This pivot ultimately continues IR's decades-long tradition of balancing efficiency with effectiveness, a focus that IR has long pioneered compared to adjacent fields.

I'll start by quickly surveying the historical arc of the efficiency-effectiveness trade-offs in IR: from classical ranking models and inverted indexing, through the 1990s with top-k retrieval strategies like MaxScore, to the multi-stage ranking architectures and Block-Max methods of the early 2010s, and through the efficient neural encoders of the mid-2010s. Following this, I'll discuss the introduction of BERT encoders into IR in 2019 and 2020, which brought forward now-maturing paradigms like cross-encoders, bi-encoders, sparse representations, and late interaction.

Following this, I'll spotlight the evolution of the late interaction paradigm, starting with ColBERT, which is fundamentally a paradigm about balancing efficiency and quality. We'll connect late interaction's focus on pruning with classical top-k retrieval strategies and see its reciprocal influences on sparse models such as DeepImpact and SPLADE. We will then discuss the efficiency considerations that led to ColBERTv2, PLAID ColBERTv2, and other methods like XTR, and beyond.

I will conclude by highlighting how the costs and benefits of Large Language Models (LLMs) offer us a chance to apply our methods to optimize much more powerful pipelines and make them tractable. LLMs also present new opportunities for the efficient IR community to shape the future of NLP through scalable retrieval-based NLP pipelines and through more holistic benchmarking methodology.

**Speaker:** **Omar Khattab** is a PhD candidate at Stanford. He builds retrieval models and retrieval-based NLP systems, which can leverage large text corpora to craft knowledgeable responses efficiently and transparently. Omar is the author of the ColBERT retrieval model and several of its derivate NLP systems like ColBERT-QA and Baleen. His most recent work includes the Demonstrate–Search–Predict (DSP) programming model for unifying retrieval and in-context learning with large language models (LLMs). Omar's Ph.D. is supported by the Apple Scholars in AI/ML PhD fellowship.
