# Abstractive Text Summarization using Transformers-BART Model

To perform abstractive text summarization on a given text data using the BART model.

## Overview
Summarization has been and continues to be a hot research topic in the data science arena. Summarization is a technique that reduces the size of a document while preserving its meaning. It is one of the most researched areas among the Natural Language Processing (NLP) community.

Summarization techniques are categorized into two classes based on whether the exact sentences are considered as they appear in the original text. New sentences are generated using NLP techniques, which are extractive and abstractive summarization.

Extractive summarization: In extractive summarization, the most meaningful sentences in an article are selected and arranged comprehensively. In short, the summarized sentences are extracted from the article without any modifications.

## Data
The data used is from the curation base repository, which has a collection of 40,000 professionally written summaries of news articles, with links to the articles themselves. The data is cloned from GitHub. Then data is downloaded in the form of a CSV file and has the following features:

- Article titles – title for the texts
- Summaries – summary for each text
- URLs – the URL links
- Dates
- Article content – content under each article

_Data is not included in this repository._

## Approach
1. Import the dataset from the dataset library and load a subset of the dataset. (To get an overview of the summarised data)
2. Clone the repository.
3. Download the article titles, summaries, URLs, and dates (a CSV file)
4. Create a new environment, install the requirements and scrape the data.
5. Change the runtime to GPU.
6. Import the required packages and libraries.
7. Create a class function for the dataset.
8. Create a class function for the BART data loader.
9. Create an abstractive summarization model class function.
10. Create a BART tokenizer
11. Define the data loader
12. Read and prepare the data.
13. Perform train test split.
14. Create the main class that runs the ‘BARTForConditionalGeneration’ model and tokenizer as an input.
15. Define the trainer class and then fit the model.
16. Perform the BART summarization using the pre-trained model.
17. Understand the concept behind the BART evaluation metric – Rouge.
18. For running the web application:
- Create a new environment
- Install the requirements.txt file
- Go to the output folder.
- Run the app.py
- Go to localhost 5000 port.
- Give a particular article link for scrapping.
- Summary for the provided article gets generated.

## Tech stack
- Language - Python
- Libraries - pandas, sklearn, pytorch, transformers
- Environment – Google Colab

## How to run
```bash
pip install -r modular_code/requirements.txt
python modular_code/output/app.py
```
Notebooks: [`AbstractiveSummarization.ipynb`](modular_code/notebooks/AbstractiveSummarization.ipynb)

## Project structure
```
.gitignore
modular_code/
  README.md
  notebooks/
    AbstractiveSummarization.ipynb
  output/
    app.py
    templates/
  requirements.txt
```

## Credits
Based on a ProjectPro guided project.
