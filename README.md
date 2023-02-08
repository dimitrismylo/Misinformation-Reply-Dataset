
# Dataset of Public Response to COVID-19 Misinformation on Twitter

This repository corresponds to the dataset used in the Master's thesis [A study of Emotion Detection on COVID-19 related Misinformation on Twitter](https://www.github.com/octokatherine).

It contains a collection of around 40,000 English tweet responses from users towards Twitter posts that have been mentioned by fact-checking websites and are classified as false or partially false.


The original dataset of misinformation tweets is that of Shahi et al. from their paper [An exploratory study of covid-19 misinformation on twitter](https://www.sciencedirect.com/science/article/pii/S2468696420300458?via%3Dihub) and can be found [here](https://github.com/Gautamshahi/Misinformation_COVID-19).

## Usage

In accordance with Twitter terms and conditions the
dataset contains only Tweet ID and Tweet Response ID pairs.

To access the full text of the tweets, Twitter's [status/lookup API](https://developer.twitter.com/en/docs/api-reference-index) must be used to rehydrate the dataset. Alternatively, a Python library such as [Twarc](https://scholarslab.github.io/learn-twarc/) can be used to rehydrate a .txt file of tweet ID's like so 


```bash
  twarc hydrate tweet_ids.txt > tweets_hydrated.jsonl
```

## How to cite this dataset

Since the associated paper has not yet been published, the GitHub repo can be cited instead.

```
@misc{dimitrismylo2023,
  author = {Dimitrios Mylonas},
  title = {A study of Emotion Detection on COVID-19 related Misinformation on Twitter},
  year = {2023},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/dimitrismylo/project-title}}
}
```