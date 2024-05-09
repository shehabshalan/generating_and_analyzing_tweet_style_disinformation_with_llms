### Generating And Analyzing Tweet-Style Disinformation with LLMs - Master Thesis

This repo contains the latest results from the experiments conducted to generate tweet-style disinformation using state-of-the-art prompting techniques including both closed and open source models.

#### Notebook content

The code can be found in `disinformation_generation.ipynb`. The notebook contains three sections:

- **Data preparation**: where the disinformation claims collected from fact-checking websites are added.
- **Disinformation generation**: code responsible for generating disinformation using various jailbreaking techniques across three different models namely GPT-3.5 Turbo, Vicuna, and WizardLM.
- **Analysis**: code responsible for analyzing the generated disinformation.

#### How to run

- Create a new virtual environment and install the required packages.
  `pip install -r requirements.txt`.
- Create a `.env` file and add API keys from [OpenAI](https://platform.openai.com/) and [TogtherAI](https://together.ai/). See `example.env` for reference.

#### Generated Datasets:

- `responses.csv`: contains the generated responses from the models.
- `responses_annotated.csv`: contains the generated responses from the models with the corresponding labels manually annotated.

[![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
