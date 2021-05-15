---
layout: post
title: Crypto Sentiment Analysis
subtitle: Natural Language Processing
gh-repo: CacheKatch/crypto_sentiment_nlp
thumbnail-img: /assets/img/thumb.png
comments: true
---

This repository is dedicaded to analyze people sentiments onto 2 of the most common cryptocurrencies (Bitcoin and Ethereum).

The analysis is solely based on news extracted from [newsapi](https://newsapi.org/) and utilizing Natural Language coding to identify the 10 most common words used in reference to these cryptos as well as the sentiment score (positive, negative or neutral) that encompass those cryptocurrencies.

The attched jupiterlab notebook has three segments:

&ensp; **Sentiment Analysis**, performed with [Vader Sentiment Analysis](http://www.nltk.org/howto/sentiment.html) to determine the sentiment (positive, negative or neutral) towards Bitcoin and Ethereum.

&ensp; **Natural Language Processing**, which consists of tokenizing, gathering the 10 most popular bigrams combinations as well as a Word Cloud chart showcasing the word frecuency on both cryptos.

&ensp; **Name Entity Recognition**, in which the two main entities were segregated ("ORG" and "GPE") from all the extracted news texts.

## Results:

&ensp; **Sentiment Analysis**: based on the mean value for the compound score, Ethereum sentiment is more positive than the one for Bitcoin. Additionally, Ethereum positive sentiment scored higher than Bitcoin, while the negative score was higher for Bitcoin than Ethereum.

Due to the above, the sentiment outlook is more favorable toward Ethereum than Bitcoin.


<table>
  <tr>
    <td><font size="3">Bitcoin Sentiment</font></td>
     <td><font size="3">Ethereum Sentiment</font></td>
  </tr>
  <tr>
    <td><img src="Images/bit_sentiment_scores.png" width=270 height=280></td>
    <td><img src="Images/ethe_sentiment_score.png" width=270 height=280></td>
  </tr>
</table>

&ensp; **Natural Language Processing**: Based on the qualititative appearance of the Word Clouds, the word Bitcoin is more frequently mentioned, as the size of the words in the charts increases with the frequency that the word appears. Also, it is worth mentioning that the word Bitcoin was so often cited on Ethereum news that an additional stopword removal (with bitcoin) was needed to differentiate Ethereum word cloud.

![Bitcoin Word Cloud](Images/bitcoin_word_cloud.png)

![Ethereum Word Cloud](Images/ethereum_word_cloud.png)

&ensp; **Name Entity Recognition**: Below the entity recognition diagrams for each crypto currency