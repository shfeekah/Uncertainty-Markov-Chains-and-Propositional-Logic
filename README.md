Topic 1: Probability & Bayes' Rule
Task 1: Toy Weather Graph
Objective: Explore discrete probability states (Sunny, Cloudy, Rainy) and compute joint, marginal, and conditional probabilities.
Key Steps:
Calculated the joint distribution  P(today,tomorrow)=P(today)×P(tomorrow∣today) .
Extracted the marginal probabilities of the weather for tomorrow and today.
Computed conditional probabilities (e.g., probability of tomorrow's weather given today's, and vice versa).
Applied Bayes' Rule to find  P(today=Rainy∣tomorrow=Rainy) .
Verified independence between weather states.
Task 2: Real Data (Breast Cancer Diagnostic Dataset)
Objective: Apply probability principles to real-world medical data.
Key Steps:
Explored features (mean radius, mean texture) to create boolean indicators for tumor size (large) and texture roughess (rough).
Computed a joint distribution (cross-tabulation) of tumor size versus malignancy.
Calculated conditional probabilities ( P(large∣malignant)  and  P(large∣benign) ).
Validated Bayes' Rule against direct count-based statistics to confirm empirical mathematical consistency.
Topic 2: Markov Chains and Language Models
Part A: Weather Chain
Objective: Model state transitions over time using a Markov Chain matrix.
Key Steps:
Simulated a 10-day weather sequence starting from a "Sunny" state using randomized path generation.
Computed the probability distribution of states after 2 days and 30 days using matrix powers ( Pt ).
Observed stationary convergence by running the chain for 100 steps from two completely different initial conditions.
Part B: Word Graph / Bigram Language Model
Objective: Build a simple character/word-level language model from a small toy text corpus.
Key Steps:
Tokenized a text corpus using special sentence delimiters (<s> and </s>).
Computed word frequencies and sequential bigram counts.
Estimated transition probabilities:  P(next\_word∣current\_word) .
Developed a function to compute the exact probability of any new sentence occurring under this model.
Implemented a text-generation algorithm to automatically generate new sentences using random sampling weighted by bigram probabilities.
