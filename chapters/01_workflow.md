# Automated experiment workflow

The central idea of automated experiment is to connect scientific goals, algorithms, instruments, and data into a closed decision-making loop.

:::{figure} ../figures/workflow.svg
:label: fig-automated-workflow
:width: 95%
:align: center

A simplified automated experiment workflow. The human defines the scientific objective, the algorithm selects actions, the instrument executes them, and the data update the model for the next decision.
:::

The important point is that the algorithm does not operate on the sample alone. It also operates through the instrument. Therefore, knowledge of the instrument — including noise, transfer functions, delays, drift, and constraints — becomes part of the decision-making system.

This is why the concept of an **instrument digital twin** is important. It provides transferable knowledge between experiments. Instead of relearning the measurement process from scratch, the optimizer can separate sample uncertainty from instrument uncertainty.

In later chapters, we will use notebooks to demonstrate this idea computationally.
