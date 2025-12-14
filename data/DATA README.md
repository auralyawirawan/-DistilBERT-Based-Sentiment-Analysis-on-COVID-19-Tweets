## Dataset Description

This study uses the public COVID-19 NLP Text Classification dataset from Kaggle,
containing English-language tweets annotated into five sentiment categories:
Extremely Negative, Negative, Neutral, Positive, and Extremely Positive.

### Raw Data
The original dataset is provided as two separate files:
- train.csv
- test.csv

These splits were supplied by the original dataset source.

### Processed Data
For preprocessing, the training and testing splits were combined to ensure
consistent text cleaning, tokenization, and label encoding.
After preprocessing, the dataset was re-split into training and testing sets
using an 80/20 stratified split, as described in the paper.

### Preprocessing Steps
- removal of URLs and non-textual artifacts
- tokenization using transformer tokenizers
- label encoding for multi-class classification
- stratified train–test split

### Data Source
https://www.kaggle.com/datasets/datatattle/covid-19-nlp-text-classification
