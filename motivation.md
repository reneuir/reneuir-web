# Motivation

Perhaps the applied nature of information retrieval (IR) research
goes some way to explain the community’s rich history of evaluating
machine learning models holistically, understanding that efficacy
matters but so does the computational cost incurred to achieve it.
This is evidenced by, among other efforts, more than a decade of
research on efficient training and inference of large decision
forest models in learning-to-rank. The community systematically
investigated questions of efficiency and explored the trade-offs
between efficiency and effectiveness in ranking models, leading
to several innovations such as multi-stage architectures, cost-aware
training and pruning algorithms, early-exit strategies, and fast
decision forest inference algorithms.

As IR adopts even more complex, neural network-based models
in a wide range of applications—marking the beginning of a
new era known as Neural Information Retrieval (NIR)—questions
on efficiency have once again become relevant. Whatever the
reason behind their success may be, NIR models achieve a
greater effectiveness than the previous wave of machine
learning models like decision forests on many IR tasks,
but with orders of magnitude more learnable parameters
and much greater amounts of data. Achieving high accuracy
by way of ever-increasing complexity once again presents
a new, but nonetheless familiar challenge that necessitates
the exploration of the Pareto frontier of the two competing
objectives: efficiency and effectiveness—echoes of the past
decade of research albeit in a different context.

While researchers in various communities concurrently
investigate efficiency-related questions posed by neural
network-based methods, we believe that the IR community
would benefit from an organized effort that is focused on NIR.
We therefore hope that this workshop on Reaching Efficiency in
Neural Information Retrieval (ReNeuIR) will serve as a forum
for a critical discussion of efficiency in the era of NIR.
Our goal is to encourage debate on the current state and
future directions of research in this space, and to promote
more sustainable research by identifying best practices in
the development and evaluation of neural models for IR.