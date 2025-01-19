### Generating And Analyzing Tweet-Style Disinformation with LLMs

This repo contains the latest results from the experiments conducted to generate tweet-style disinformation using state-of-the-art prompting techniques including both closed and open source models.

#### Notebook content

The code can be found in `llm_generation_pipelines.ipynb`. The notebook contains three sections:

- **Data preparation**: where the disinformation claims collected from fact-checking websites are added.
- **Disinformation generation**: code responsible for generating disinformation using various jailbreaking techniques across three different models namely GPT-3.5 Turbo, Vicuna, and WizardLM.
- **Factual Information generation**: code responsible for generating factual information using various jailbreaking techniques across three different models namely GPT-3.5 Turbo, Vicuna, and WizardLM.
- **Analysis of both pipelines**: code responsible for analyzing the generated disinformation or factual information.

#### How to run

- Create a new virtual environment and install the required packages.
  `pip install -r requirements.txt`.
- Create a `.env` file and add API keys from [OpenAI](https://platform.openai.com/) and [TogtherAI](https://together.ai/). See `example.env` for reference.

#### Datasets:

- `false_claims.csv`: contains false claims collected from various sources.
- `true_claims.csv`: contains true/factual claims collected from various sources.
-

#### Generated Datasets:

- `response_false.csv`: contains all responses generated from the false claims by all LLMs.
- `response_true.csv`: contains all responses generated from the true claims by all LLMs.

#### Labelled Datasets:

- `responses_false_annotated.csv`: contains all false claims responses from LLMs with their labels.
- `responses_true_annotated.csv`: contains all true claims responses from LLMs with their labels.

[![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
