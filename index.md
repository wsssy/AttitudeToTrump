---
layout: page
title: Population's Attitudes Towards Trump
cover-img	: assets/img/trump_in_g7.jpeg
---


# Population's Attitudes Towards Trump

## Abstract 📖

In recent years, Donald Trump is no doubt one of the most controversial public figures around the world. From winning the 2016 presidential election as a dark horse to losing the election by a narrow margin in late 2020, Trump has made a non-negligible impact on the United States and the world in the four years of his presidency. People’s attitude towards him greatly divides over different groups of people and varies as time moves forward. We want to see what people's attitudes toward Trump are in these four years, whether these attitudes have changed, and further what factors might be related to these changes. In other words, we will study people’s attitudes before and after some major events to find out how the attitudes change.

## Who talked most about Trump?

### Who talked most about Trump in 2015 before election?
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width="100%" height="500" allowfullscreen="true" src="assets/img/quotes-2015_before_election_top10_count.html"></iframe>

Trump has announced his willingness for the presidential election in June 2015. Before his presidency,  as we know, he was a businessman, a TV show host, a writer of *The art of deal*, a WWE wrestler,with such a rich professional experience but surprisingly no political career.  It would be interesting to see who talks most about Trump at different times. Since this may reveal how his social circle changes. Thanks to quotebank, we collect all those people who talked most about Trump before he announced his candidacy.  As shown in the above picture, Trump himself without doubt has most quotations about himself. Other people seem to be less famous. Their occupations are shown in the table below. 


| People              | Occupation                 |
| :-------------------| ---------------------------|
| Sarah Palin         | a local politician         |
|  Herman Saatkamp    | fourth president of Stockton University  |
| Jerry Seinfeld      | a famous actor             |
| Steve Deace         | a comedy show host         |
| Alec Baldwinn       | an actor                   |
| Ian Ziering         | an actor                   |
| John Gibbons        | a baseball player          |
| Hope Hicks          | a  former employee of The Trump Organization |
| Leeza Gibbons       | a talk show host           |
| Joe Scarborough     | a Television host          |

As we can see from the table, most people are non politicians and most of them are from show business. If we take a close look at the quotation numbers, we found that they are all less than one hundred. Not too many people were interested in Trump except himself before his presidency.  However everything has changed after he became president of america. Now let us fly to 2020 to see who talks about him most. As shown in the picture below, first and not surprisingly, Trump was still the person who talked himself most. However, other people who talked most about Trump have hugely changed. One obvious observation is that all of them are now politicians. This strongly suggests that Trump’s circle has changed, from a businessman to the centre of the political vortex. On the other hand, if we take a close look at the quotation numbers, we may find that it has grown hugely from below a hundred to thousands of quotes. This also suggests that Trump becomes the centre of the whirling vortex of politics. 

### Who talked most about Trump in 2020?
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width="100%" height="500" allowfullscreen="true" src="assets/img/quotes-2020_top10_count.html"></iframe>

In this part we have discovered the transition of Trump’s circle from the difference of people who talked about him most. It would be nice to take a closer look at what people actually say. So we analyze the word frequency as discussed in the next section.







## **word frequency** 
<div class="withSidenote" markdown="1">


<figure class="sidenote">
    <img src="assets/img/Trump_wings.jpeg">
    <figcaption><em>Figure 1.</em> Trump and his wings</figcaption>
</figure>
</div>

## The Semantics of the Quotes in 2015 are Different

<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width="100%" height="500" allowfullscreen="true" src="assets/img/PCA_Result_of_Aggrageted_by_Month.html"></iframe>

The graph above is the 2-dimension representation of the word
embeddings aggregated by months. We aggregate the word embeddings by
averaging the embedding vectors grouped by months. In the graph,
numbers called 'Date Sequence' map to months between January 2015 and
April 2020.

As we can see from the graph, quotes in 2015, which are represented by
points with the darkest colours, have vastly different semantics from
those in the other years. The points spread around the plot and quite
a few of them are far away from the cluster of points near the middle.

2015 is the year preceding Trump's presidency and as we can see from
our previous analysis people who talked about Trump has changed after
his presidency, which should be the main reason why quotes in 2015
mentioning Trump have different semantics.

If the conjecture were true, we can see that different people talk in
different styles and talk about different things.

## **Research Questions** ❓

- **Question 1**. To explore the attitude towards Trump of each people cluster and check whether there is (a) specific cluster(s) that has/have an explicit attitude towards him and find out whether these clusters have some defining or distinguishing characteristic.

- **Question 2**. To explore the changes of attitude towards Trump in each cluster as time went by. we could pick up some specific time such as,	
  - before and after Trump won his presidency (December 2016 ) 
  - the covid outbreak (March 2020)

- **Question 3**. To explore whether there is any correlation between people’s attitudes toward Trump and America.



##  **Methods** 🔨

### 1. **Quotebank Data Cleaning**

According to our topic, first we need to extract quotations related to Donald Trump and America and build databases respectively. To build the database, we filter out quotations whose speaker is “None”, keep the quotation containing the keywords related to Donald Trump or America, and only keep the quotation whose phase is ‘E’. After that, we get speakers’ identical information from wikidata through **‘qid’**.

### 2. **Sentiment Analysis**

By applying **text2emotion**  package, we could get the emotion of each quote with probability, the result for each is like: {'Happy': 0.0, 'Angry': 0.0, 'Surprise': 0.5, 'Sad': 0.0, 'Fear': 0.5}. 

### 3. **Wikidata Cleaning and processing**

We aggregate all the categorical fields of a speaker into one array with the label of the fields prepended, which we then convert to an indicator vector whose columns represent one category. The categorical fields we consider are as follows:

 - nationality
 - gender 
 - ethnic group
 - occupation
 - party
 - academic degree
 - candidacy
 - religion

We also calculate the ages of the speakers from their dates of birth. After that, we plot the distribution of the ages of the speakers and filter out people aged over 120, which we consider irrelevant to our analysis.

### 4. **Clustering or Simple Grouping**

By applying some clustering algorithms, our target speakers will be clustered with features in wiki data. In this part, we can also manually group people by some single feature such as their age, occupation, or their educational background.

### 5. **Analysis of attitude distributions in each cluster**

We will find the attitude distribution in each cluster to see whether people who share similar characteristics have similar attitudes towards Trump. We say people sharing similar characteristics means a group of people either generated by clustering algorithm or we manually group them by some simple feature. Then we try to find out if there are some groups that have some explicit attitude towards Trump. In other words, we will get the attitude distribution in each group, if there is an attitude dominant, then we try to find out what is the defining or distinguishing characteristic of this group. 

### 6. **Analysis of how time and events influence people’s attitudes**  

Now we focus on some clusters and try to find how their attitudes changed over time or around some major events. We plot the distribution of people's attitudes towards Trump in this cluster over time to get a general picture of how people’s attitudes changed overtime. This can be done with a slider plot where the slider controls time. Then we pick two specific time points (‘2016 election’ and ‘outbreak of Covid’) and get the distributions of people’s attitudes before and after these time points. We can use t-test or other methods to see whether the distributions are significantly different from each other which can help us find out if people’s attitudes correspond to specific events.

### 7. **Correlation between people’s attitudes towards USA and Trump**

To show whether there is a correlation between people’s attitudes towards Trump and America, the most initiative way could be to plot how people’s attitudes change towards Trump and America as time went by in one single picture. In order to find the relation between people’s attitudes toward Trump and America, we first need to compute the average probability for each emotion of a cluster towards Trump and America, then we could get Pearson correlation coefficients between emotion probabilities of Trump and the USA. We can also perform null hypothesis tests to explore more about their correlation. 

## **Proposed timeline** 🗓

| Date                         | Tasks                                                        |
| :--------------------------- | ------------------------------------------------------------ |
| By week 6                    | Brainstorm and decide final project ideas                    |
| By week 8  (milestone 2 due) | Data clean and data extraction, finish initial analysis and finish sentiment analysis |
| By week 10 (HW2 due)         | Clustering speakers by Wikidata features                     |
| By week 11                   | Research question 1                                          |
| By week 12                   | Research question 2 and 3                                    |
| By week 13 (milestone 3 due) | Draw the final conclusions and write the data stories        |



## **Organization within the team** 👨‍👩‍👧‍👦

### Milestone 2

**Jinyi Xian**: initial data analysis, data wrangling, sentiment analysis

**Sijia Du**: initial data analysis, data wrangling, sentiment analysis

**Huan Yang**: initial data analysis, write readme file, come up with research questions and possible methods 

**Siyi Wang**:  initial data analysis, write readme file, come up with and improve proposal

### Milestone 3

**Jinyi Xian**: Cluster analysis, visualization, research question1, research question 3, write data story.

**Sijia Du**: Visualization, research question1, research question2, write data story.

**Huan Yang**: Cluster analysis, visualization, research question2, research question 3, write data story.

**Siyi Wang**: Visualization, research question1, research question 3, correlation analysis, write data story.

## **Ideas that we have dropped** 🗑

- **Idea 1**: Build a regression model to predict people’s attitude towards Trump

  **weakness**: The categorical feature of speakers may lead us to have too many independent variables in our regression model that we can not handle. 

- **Idea 2**:  Research question 1 is about finding out people with similar characteristics also have similar attitudes toward Trump. Can we do it the other way around, that is we find out those people who have similar attitudes, can we find some common features among them. 

  **weakness**:  We think this is not very feasible because people’s characteristics in each group could still be greatly diverse. The pattern behind is likely to be obscure. 

## **Questions for TAs** 👀

1. How to deal with one speaker having more than 1 qid?
2. For research question 3 the original one is “To explore whether
   there is any correlation between people’s attitudes toward Trump
   and America and discover whether there is any causal relationship
   between them.” But it seems difficult to find if it is actually a
   causal relation. How can we know if changes in people's attitudes
   towards Trump actually cause their opinion change towards America?
   Some major events can be those compounders where it both changes
   people’s attitude towards Trump and Us. How can we select people
   with a “coin”? Or how can we find some useful matching?
