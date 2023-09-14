# statistics

# Probability of the Union of Multiple Events

The probability of the union of multiple events can differ based on the nature of the events. Here are the two main scenarios:

## 1. Mutually Exclusive Events

If the events $A$ and $B$ are mutually exclusive (they cannot happen at the same time), then the probability of their union is:

$$
P(A \cup B) = P(A) + P(B)
$$

For \(n\) mutually exclusive events $A_1, A_2, \ldots, A_n$, the probability of the union is:

$$
P\left( \bigcup_{i=1}^{n} A_i \right) = \sum_{i=1}^{n} P(A_i)
$$

## 2. Non-Mutually Exclusive Events

If $A$ and $B$ are not mutually exclusive (they can occur simultaneously), then their union's probability is:

$$
P(A \cup B) = P(A) + P(B) - P(A \cap B)
$$

Here, $P(A \cap B)$ is the probability that both $A$ and $B$ happen.

### Inclusion-Exclusion Principle for $n$ Events

For $n$ non-mutually exclusive events, the probability of the union can be calculated using the principle of Inclusion-Exclusion:

$$
P\left( \bigcup_{i=1}^{n} A_i \right) = \sum_{i=1}^{n} P(A_i) - \sum_{i < j} P(A_i \cap A_j) + \sum_{i < j < k} P(A_i \cap A_j \cap A_k) - \ldots + (-1)^{n+1} P(A_1 \cap A_2 \cap \ldots \cap A_n)
$$


## Probability of the Union of Multiple Events $A$, $B$, and $C$

To find the probability of the union of three events $A$, $B$, and $C$, you can use the principle of Inclusion-Exclusion. The formula is as follows:

$$
P(A \cup B \cup C) = P(A) + P(B) + P(C) - P(A \cap B) - P(A \cap C) - P(B \cap C) + P(A \cap B \cap C)
$$

### Explanation:

1. **Add Individual Probabilities**: First, you sum up the individual probabilities of each event occurring:

    $$
    P(A) + P(B) + P(C)
    $$

2. **Subtract Overlaps**: Then, subtract out the probabilities of any two events happening at the same time, as these get counted twice in the first step:

    $$
    P(A \cap B) + P(A \cap C) + P(B \cap C)
    $$

3. **Add Back Triple Overlap**: Finally, add back the probability of all three events happening simultaneously, since it has been subtracted multiple times in the above steps:

    $$
    P(A \cap B \cap C)
    $$

This formula accounts for the overlaps and ensures that each possible outcome is counted exactly once.
