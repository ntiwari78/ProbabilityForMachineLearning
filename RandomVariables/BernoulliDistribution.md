# BenoulliDistribution
The **Bernoulli distribution**, a fundamental probability distribution for modeling binary outcomes. A Bernoulli random variable, denoted as \( X \sim \text{Ber}(p) \), can take values of 1 (with probability \( p \)) or 0 (with probability \( 1 - p \)). Examples include a coin flip or success/failure in a trial. Key properties are outlined:

- **PMF**: \( P(X=x) = p^x (1-p)^{1-x} \)
- **Expectation**: \( E[X] = p \)
- **Variance**: \( \text{Var}(X) = p(1 - p) \)

Additionally, **indicator variables** are introduced as Bernoulli variables that represent whether an event has occurred, simplifying certain calculations in probability models.

## Explanation
The **Bernoulli Distribution** is a discrete probability distribution that describes events with only two possible outcomes, often called "success" (usually denoted by \(1\)) and "failure" (usually denoted by \(0\)). It’s one of the simplest yet foundational distributions in probability and statistics, underpinning more complex models and distributions, such as the Binomial Distribution.

### Definition of Bernoulli Distribution

If we have a random variable \( X \) that represents the outcome of a single experiment or trial:
- \( X = 1 \) if the outcome is a success,
- \( X = 0 \) if the outcome is a failure.

The **Bernoulli Distribution** of \( X \) is parameterized by \( p \), the probability of success:
\[
P(X = 1) = p \quad \text{and} \quad P(X = 0) = 1 - p
\]
where \( 0 \leq p \leq 1 \).

In mathematical terms, the probability mass function (PMF) of a Bernoulli random variable \( X \) is:
\[
P(X = x) = p^x (1 - p)^{1 - x} \quad \text{for } x \in \{0, 1\}
\]

### When to Use Bernoulli Distribution

The Bernoulli Distribution is used when:
- We are modeling an experiment or process that has exactly two outcomes, typically “success” and “failure.”
- Each outcome occurs with a fixed probability.
  
Examples include:
- A coin toss, where "heads" (or tails) can be considered a success.
- A yes/no survey response.
- Any situation where there is a binary (0/1) outcome in a single trial.

### Properties of Bernoulli Distribution

1. **Expected Value (Mean)**:
   The mean of a Bernoulli random variable \( X \) is given by:
   \[
   E(X) = p
   \]

2. **Variance**:
   The variance of \( X \) is:
   \[
   \text{Var}(X) = p(1 - p)
   \]

3. **Moment Generating Function (MGF)**:
   The moment generating function \( M_X(t) \) of \( X \) is:
   \[
   M_X(t) = E(e^{tX}) = (1 - p) + p e^t
   \]

### Derivation of the Expected Value and Variance

#### 1. Derivation of the Mean \( E(X) \):

The expected value of \( X \) is given by:
\[
E(X) = \sum_{x=0}^1 x \cdot P(X = x)
\]
Since \( X \) takes the value \( 1 \) with probability \( p \) and \( 0 \) with probability \( 1 - p \), we have:
\[
E(X) = 0 \cdot (1 - p) + 1 \cdot p = p
\]

#### 2. Derivation of the Variance \( \text{Var}(X) \):

Variance is given by \( \text{Var}(X) = E(X^2) - (E(X))^2 \).

Since \( X^2 = X \) for a Bernoulli random variable (because \( X \) can only be 0 or 1), we get:
\[
E(X^2) = E(X) = p
\]

Therefore:
\[
\text{Var}(X) = E(X) - (E(X))^2 = p - p^2 = p(1 - p)
\]

### Summary

The Bernoulli Distribution models binary outcomes with a probability \( p \) of success and \( 1 - p \) of failure. Key characteristics include:
- PMF: \( P(X = x) = p^x (1 - p)^{1 - x} \)
- Mean: \( E(X) = p \)
- Variance: \( \text{Var}(X) = p(1 - p) \)

The Bernoulli Distribution is foundational for understanding binary events and serves as the building block for more complex distributions, such as the Binomial and Geometric distributions.
