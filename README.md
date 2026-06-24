# Words of Power - Veridion Side Challenge (HACKITALL 2025)

This repository is a fork of the original project developed during the HACKITALL hackathon (March 2025) for the challenge sponsored by Veridion.

The primary objective of the application was to build an automated system capable of competing in an extended, highly complex variant of "Rock, Paper, Scissors," leveraging a massive dataset of words and semantic rules.

## My Contribution

While this was a collaborative effort in a two-person team, my primary responsibility was the **architecture and implementation of the core decision logic**. I engineered the system responsible for analyzing the opponent's input word and dynamically calculating the optimal counter-attack.

### Key Implementations:

* **Semantic Analysis (NLP):** Integrated the `nltk` library and `WordNet` to dynamically extract synonyms and map semantic counter-relationships (e.g., *water* vs. *fire*, *light* vs. *darkness*).
* **Selection Heuristics:** Designed an algorithm to identify structural vulnerabilities in the incoming word—analyzing unique vowel count, string length, and special characters—to determine the optimal cost class for the response.
* **Decision Optimization:** Implemented a weight-based selection function (`weighted_choice`) that prioritizes the most cost-effective vocabulary, maximizing the long-term statistical win rate.
