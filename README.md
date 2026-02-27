# Probabilistic Decision Models

A practical guide to using probabilistic thinking and mathematical models for better decision-making. This repository covers Bayesian reasoning, expected value calculations, Monte Carlo simulations, and other quantitative tools that help you navigate uncertainty with confidence.

## Why Probabilistic Thinking?

Most real-world decisions involve uncertainty. Yet humans are notoriously bad at intuitive probability estimation. We overweight rare dramatic events, underweight common mundane risks, and fail to update our beliefs properly when new evidence arrives. Probabilistic decision models provide a rigorous alternative to gut-feel decision-making. By practicing these models regularly — using tools like [KeepRule](https://keeprule.com) — you can train your brain to think more clearly under uncertainty.

## Core Concepts

### Bayesian Updating

Bayes' theorem is the foundation of rational belief updating. It tells you how to revise your probability estimate for a hypothesis when you receive new evidence:

```
P(H|E) = P(E|H) × P(H) / P(E)
```

Where:
- P(H|E) = Probability of hypothesis given evidence (posterior)
- P(E|H) = Probability of evidence given hypothesis (likelihood)
- P(H) = Prior probability of hypothesis
- P(E) = Total probability of evidence

**Example**: A medical test has 95% sensitivity and 90% specificity. If the disease prevalence is 1%, and you test positive, what is the probability you actually have the disease? Using Bayes' theorem: approximately 8.7% — far lower than most people intuitively guess.

### Expected Value (EV)

The expected value of a decision is the probability-weighted average of all possible outcomes:

```
EV = Σ (probability_i × outcome_i)
```

Always choose the option with the highest expected value when decisions are repeatable. For one-time, irreversible decisions, also consider the variance and worst-case scenarios.

### Kelly Criterion

The Kelly criterion determines the optimal bet size to maximize long-term wealth growth:

```
f* = (bp - q) / b
```

Where b = odds, p = probability of winning, q = probability of losing. This formula is widely used in both gambling and investment portfolio sizing.

### Monte Carlo Simulation

When analytical solutions are intractable, simulate thousands of random scenarios to estimate the probability distribution of outcomes. Monte Carlo methods are invaluable for complex decisions involving multiple correlated uncertainties, such as project planning, financial forecasting, and risk assessment.

## Decision Trees and Influence Diagrams

Decision trees map out all possible choices, chance events, and outcomes in a visual format. Each branch represents a possible path, and by calculating expected values from the leaves back to the root, you can identify the optimal strategy.

**Key steps**:
1. Identify decision nodes (squares) and chance nodes (circles)
2. Assign probabilities to each branch of chance nodes
3. Assign payoff values to each terminal node
4. Calculate expected values by folding back the tree

## Practical Applications

### Business Strategy
- New product launch: Model demand scenarios with probability distributions
- Pricing decisions: Use expected value analysis across customer segments
- Market entry: Build decision trees for sequential investment decisions

### Personal Finance
- Career decisions: Model expected lifetime earnings across different paths
- Insurance: Calculate expected value of insurance vs. self-insuring
- Investment: Use Kelly criterion for portfolio allocation

### Project Management
- Schedule risk: Monte Carlo simulation of task durations
- Budget estimation: Probabilistic cost modeling with confidence intervals
- Resource allocation: Expected value optimization across projects

## Common Pitfalls

1. **Base Rate Neglect**: Ignoring prior probabilities when evaluating evidence
2. **Conjunction Fallacy**: Believing specific scenarios are more likely than general ones
3. **Overconfidence in Point Estimates**: Using single numbers instead of ranges
4. **Ignoring Correlation**: Treating dependent risks as independent
5. **Survivorship Bias**: Only analyzing successful outcomes

## Building Your Probabilistic Thinking Skills

Developing strong probabilistic intuition requires deliberate practice:

1. **Calibration training**: Practice making predictions with confidence intervals and track your accuracy. You should be right 90% of the time in your 90% confidence intervals.
2. **Fermi estimation**: Practice breaking complex questions into estimable components.
3. **Daily probability practice**: Use platforms like [KeepRule](https://keeprule.com) to build habits around probabilistic reasoning and Bayesian thinking through structured daily exercises.
4. **Prediction journaling**: Record predictions with probabilities and review them regularly.

## Tools and Libraries

- **Python**: `scipy.stats`, `numpy.random`, `pymc3` for Bayesian modeling
- **R**: `rjags`, `rstanarm` for Bayesian inference
- **Excel**: Built-in probability functions and Data Table for simple Monte Carlo
- **[KeepRule](https://keeprule.com)**: Daily practice platform for decision-making principles

## Recommended Reading

- "Superforecasting" by Philip Tetlock
- "The Signal and the Noise" by Nate Silver
- "How to Measure Anything" by Douglas Hubbard
- "Fooled by Randomness" by Nassim Taleb

## License

MIT License
