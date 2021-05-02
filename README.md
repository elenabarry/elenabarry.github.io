# Emoji Abuse Scores 

https://elenabarry.github.io

![Screenshot 2021-05-02 at 10 50 49](https://user-images.githubusercontent.com/53048127/116809151-9ae0b980-ab34-11eb-8c1e-c2ab236c377c.png)


I used the corresponding dataset from the paper ‘Large Scale Crowdsourcing and Characterization of Twitter Abusive Behavior’ [1]. Each tweet is labelled as abusive/hateful/spam/normal by 5 CrowdFlower workers. Founta et al. [1] 

My focus was cyberbullying; therefore, I only included abusive, hateful, and normal tweets were included in the dataset, and tweets labelled as ‘spam’ were removed.

To find out the underlying emotions of abusive tweets that used emojis, I calculated the probabilities of each emoji in the dataset to be in either an abusive, hateful, or normal context. 

Produced a sentiment lexicon of the 751 most frequent emojis. I have followed their process and calculated 334 new abuse scores of emojis from -1 and 1 on whether the emoji is present in a normal, hateful, or abusive context.

Emojis with at least 5 occurrences are included, resulting in a lexicon of 334 emojis. The sentiment scores for the emojis with fewer than 5 occurrences are not very reliable.

Abuse labels can take one of three values: abusive ≺ hateful ≺ normal. Which correspond to a discrete, 3-valued variable c ∈ {−1, 0, +1}.

For each emoji, I was able to use these three labels to form a discrete probability distribution. The distribution components, p−, p0, and p+ denote the abusiveness, hatefulness, and normality of the emoji, respectively.

The number of occurrences N, of each emoji to appear in each label, c, allows a probability, pc, to be estimated. Multiple emojis in a tweet are counted.

The mean of the distribution gives an emoji it’s abuse score

## A Worked Example

   

## Dataset 
[1]A.  Founta et al., "Large Scale Crowdsourcing and Characterization of Twitter Abusive Behavior", 12th International Conference on Web and Social Media, ICWSM 2018, 2018. [Accessed 10 October 2020].

## Method 
[2]P.  Kralj Novak, J.  Smailović, B.  Sluban and I.  Mozetič, "Sentiment of Emojis", PLOS ONE, vol. 10, no. 12, p. e0144296, 2015. Available: 10.1371/journal.pone.0144296.

## Website Template
[3]"tutsplus/tablesorter", GitHub, 2021. [Online]. Available: https://github.com/tutsplus/tablesorter. [Accessed: 30- Apr- 2021].
