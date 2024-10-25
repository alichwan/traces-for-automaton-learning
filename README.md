# Automata Learning Dataset

This dataset is intended to be used for the creation and evaluation of algorithms that learn automata from fixed examples.

The dataset was created using the same mechanism as in the StaMina competition [1], utilizing the Statechum code [2] with the help of Kirill Bogdanov.

## Dataset Structure

Each of the files represents a "problem". Each problem consists of positive and negative (disjoint) traces, and the name of the problem is determined by its configuration:

- **`L`**: Number of letters or symbols that exist in the problem.
- **`T`**: Number of traces for each sign in the problem.
- **`X`**: Index of extra length of the trace. The higher the value of `X`, the longer the traces will be, on average.
- **`C`**: Seed of randomness chosen. `C=0` could be used as a debugger and the other values are used for the real experiments.
- **`S`**: Number of states of the automaton that originated the traces. In this dataset, `S` is equal to 50 for all examples.

## References

- [1] Walkinshaw, N., Lambeau, B., Damas, C., Bogdanov, K., & Dupont, P. (2013). **STAMINA: A Competition to Encourage the Development and Assessment of Software Model Inference Techniques**. _Empirical Software Engineering, 18_, 791-824. [DOI: 10.1007/s10664-012-9210-3](https://doi.org/10.1007/s10664-012-9210-3)
- [2] Statechum Repository: [https://github.com/kirilluk/statechum](https://github.com/kirilluk/statechum)
