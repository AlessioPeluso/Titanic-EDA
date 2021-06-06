# Titanic-EDA

Today we'll explore one of the first dataset to analize in order to approach data science: Titanic dataset.

We will follow the following steps:
  1. Feature engineer
  2. Missing values
  3. Prediction

Using R.

Let's begin by loading the datasets and putting them together.

train <- read.csv('../input/titanic/train.csv', stringsAsFactors = F)
test  <- read.csv('../input/titanic/test.csv', stringsAsFactors = F)

full  <- bind_rows(train, test) # bind training & test data

str(full)

