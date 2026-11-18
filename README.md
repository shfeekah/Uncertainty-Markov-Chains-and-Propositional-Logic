# Probability, Bayes' Rule, Markov Chains & Language Models

A Python-based project exploring fundamental probability concepts, Bayesian inference, Markov Chains, and Bigram Language Models through practical simulations and real-world datasets.

The project is divided into two major topics, covering both theoretical probability experiments and practical applications using real-world data.

## 📌 Project Overview

### Topic 1: Probability & Bayes' Rule

#### Task 1: Toy Weather Graph

**Objective:** Explore discrete probability states (Sunny, Cloudy, Rainy) and calculate joint, marginal, and conditional probabilities.

**Key Implementations:**
- Defined three discrete weather states: Sunny, Cloudy, and Rainy.
- Calculated the joint probability distribution:

  `P(Today, Tomorrow) = P(Today) × P(Tomorrow | Today)`

- Extracted marginal probability distributions for today's and tomorrow's weather.
- Computed conditional probabilities in both directions.
- Applied Bayes' Rule to calculate:

  `P(Today = Rainy | Tomorrow = Rainy)`

- Verified the statistical independence of weather states.

#### Task 2: Real-World Data – Breast Cancer Diagnostic Dataset

**Objective:** Apply probability concepts and Bayesian inference to real-world medical data.

**Dataset:** Breast Cancer Diagnostic Dataset.

**Key Implementations:**
- Explored diagnostic features, including mean radius and mean texture.
- Created boolean indicators to classify tumors as:
  - Large or Small (based on mean radius).
  - Rough or Smooth (based on mean texture).
- Generated a joint distribution using cross-tabulation of tumor size and malignancy.
- Calculated conditional probabilities:
  - `P(Large | Malignant)`
  - `P(Large | Benign)`
- Applied Bayes' Rule to estimate probabilities from the observed data.
- Validated Bayesian calculations against direct count-based statistics to confirm mathematical consistency.

---

### Topic 2: Markov Chains & Language Models

#### Part A: Weather Markov Chain

**Objective:** Model weather transitions over time using a Markov Chain transition matrix.

**Key Implementations:**
- Defined weather states: Sunny, Cloudy, and Rainy.
- Constructed a transition probability matrix.
- Simulated a randomized 10-day weather sequence starting from Sunny.
- Calculated state probability distributions after:
  - 2 days
  - 30 days
- Used matrix powers (`P^t`) to predict future weather distributions.
- Investigated stationary distribution convergence over 100 steps.
- Compared convergence from two completely different initial weather conditions.

#### Part B: Word Graph / Bigram Language Model

**Objective:** Build a simple probabilistic language model using word-level transitions from a toy text corpus.

**Key Implementations:**
- Tokenized a text corpus using special sentence boundary markers (`<START>` and `<END>`).
- Calculated individual word frequencies.
- Generated sequential bigram counts.
- Estimated conditional transition probabilities:

  `P(Next Word | Current Word)`

- Implemented a function to calculate the probability of a given sentence using the learned bigram model.
- Developed a probabilistic text-generation algorithm.
- Generated new sentences using random sampling weighted by learned bigram transition probabilities.

---

## 🛠️ Technologies & Libraries

- **Python** – Core programming language
- **NumPy** – Probability calculations and matrix operations
- **Pandas** – Data manipulation and cross-tabulation
- **Matplotlib / Seaborn** – Data visualization (if used in the implementation)
- **Jupyter Notebook / Google Colab** – Development and experimentation

## 📚 Concepts Covered

| Topic | Concepts |
|---|---|
| Probability | Joint, Marginal & Conditional Probability |
| Bayesian Inference | Bayes' Rule |
| Independence | Statistical Independence |
| Real-World Applications | Medical Dataset Analysis |
| Markov Chains | State Transitions & Transition Matrices |
| Matrix Operations | Matrix Powers & Long-Term Predictions |
| Stationary Distribution | Convergence of Markov Chains |
| Language Models | Tokenization & Word Frequencies |
| Bigram Models | Conditional Word Probabilities |
| Text Generation | Weighted Random Sampling |

## 🎯 Learning Outcomes

Through this project, we explored how probability theory can be applied to both simulated and real-world problems.

- Understood the relationship between joint, marginal, and conditional probabilities.
- Applied Bayes' Rule to simulated weather conditions and medical diagnostic data.
- Learned how Markov Chains model sequential events and predict future states.
- Observed long-term convergence toward stationary distributions.
- Built a basic Bigram Language Model from a text corpus.
- Implemented probabilistic sentence evaluation and automatic text generation.

## 👥 Contributors

Developed as an academic project to demonstrate practical applications of probability theory, Bayesian inference, Markov Chains, and probabilistic language modeling.

---

*This project is intended for educational purposes and demonstrates foundational probabilistic techniques rather than a clinical diagnostic system or production-ready language model.*
