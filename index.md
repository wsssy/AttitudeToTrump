---
layout: page
title: "Trump: 2015 to 2020"
cover-img: assets/img/trump_in_g7.jpeg
---


## Backgrounds 

In recent years, Donald Trump is no doubt one of the most
controversial public figures around the world. From winning the 2016
presidential election as a dark horse to losing the election by a
narrow margin in late 2020, Trump has made a significant impact on
the United States and the world during the four years of his presidency.

In our story we are going to discover what has changed for quotes on Trump and the reason behind these changes. At the beginning, we will first discover the change of Trump's social circle by analysing who talked most about him at different times. Then we are going to investigate the changes over people's words when they talked about Trump. After that, we go one step further to analyse the semantics of quotes rather than analysing on the level of words. Finally, we will try to identify the potential factors that would have caused these changes.


## Who talked most about Trump?

### Who talked most about Trump in 2015 before election?
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width="100%" height="500" allowfullscreen="true" src="assets/img/quotes-2015_top10_count.html"></iframe>

Trump has announced his willingness for the presidential election in June 2015. Before his presidency,  as we know, he was a businessman, a TV show host, a writer of *The art of the deal*, a WWE wrestler,with such a rich professional experience but surprisingly no political career.  It would be interesting to see who talks most about Trump at different times. Since this may reveal how his social circle changes. Thanks to quotebank, we collect all those people who talked most about Trump before he announced his candidacy.  As shown in the above picture, Trump himself without doubt has most quotations about himself. Other people seem to be less famous. Their occupations are shown in the table below. 

<div class="withSidenote" markdown="1">


<figure class="sidenote">
    <img src="assets/img/Trump_wings.jpeg">
    <figcaption><em>Figure 1.</em> Trump and his wings</figcaption>
</figure>
</div>


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





## **Word frequency** 

<figure style="text-align: center">
    <img src="assets/img/2015_wordcloud_befor6.png" style="width:65%">
</figure>

Now let us look at the keywords of all quotes in 2015 before he announced his candidacy. As shown in the above picture, we can see some interesting keywords such as “business”, “businessman”, “golf” etc. This matches his role at that time pretty well. Now let us fly to 2020, as shown in the second picture here we can easily see that the semantics of  keywords have hugely changed. Most keywords appearing now are tightly related to topics of politics, such as “campaign”, “administration”, “election“ etc. Again, this gives us strong evidence of the transition of Trump’s position, namely from  a businessman to the president. Also not surprisingly, we found the keywords “coronavirus”  in the below  picture which also made us more convinced that  this “word cloud” in some way can represent the trends of that time.


<figure style="text-align: center">
    <img src="assets/img/2020_wordcloud.png" style="width:65%">
</figure>

In this section  we have checked word frequency to analyse how Trump’s role changed and how main topics have changed when people speak about Trump. However, in this section we did not analyse the semantics on the level of the sentence.  It would be nice to discover the semantics of each quote. So in the next section we will use BERT to do further  analysis.





## The Semantics of the Quotes in 2015 are Different

<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width="100%" height="500" allowfullscreen="true" src="assets/img/PCA_Result_of_Aggrageted_by_Month.html"></iframe>

The graph above is the 2-dimension representation of the word
embeddings aggregated by months. We aggregate the word embeddings by
averaging the embedding vectors grouped by months. In the graph,
numbers called 'Date Sequence' map to months between January 2015 and
April 2020.

As we can see from the graph, quotes in 2015, which are represented by
points with the darkest colours, have vastly different semantics from
those in the other years. These points are mostly around (0.6, 0) and
in the graph they are to the right of where most other points
lie. Also, some spread around the graph.

2015 is the year preceding Trump's presidency and as we can see from
our previous analysis people who talked about Trump has changed after
his presidency, which should be the main reason why quotes in 2015
mentioning Trump have different semantics.

If the conjecture were true, we can see that different people talk in
different styles and talk about different things and one of the most
significant change takes place around 2015, which is about the time
when Trump turned from a businessman without political experience into
the president of the United States. Below, we will dig deeper to find
out the factors that may influence people's words towards Trump.

## Do people's attitudes towards Trump relate to their regions?

Since people’s attitudes may be changed over time, It's hard to see people's attitudes over a long time range. Thus, we chose to study people's attitudes in 2019 because the data from 2019 is complete and closer to the current situation than data from another year.

### Distribution of speakers' regions

First, let’s look at the number of speakers from different regions.

<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width="100%" height="500" allowfullscreen="true" src="assets/img/distribution_of_speakers_Regions_2019.html"></iframe>

Most speakers come from Europe, then followed by the United States, and then Asia. This is probably because Europe and the United States are English-speaking regions, and most of the quotes included in Quotebank are from newspapers published in these two regions.

### People’s attitude towards Trump in 2019 grouped by regions

We performed sentiment analysis on each quote and got positive and negative scores. if positive is greater than negative, we considered this quote as positive and vice versa, if the scores are equal this quote was neutral. Let's see how people from different Regions are thinking about Trump.


<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width="100%" height="500" allowfullscreen="true" src="assets/img/2019_country_attitude.html"></iframe>

In general, there is no huge difference between the proportion of positive and negative in most countries, with slightly more positive than negative. However, the proportion of positive attitudes in “others” is large, because the number of people from other places is small and there is a bias in the statistics, so we do not consider "others" for the time being. Let's look at the rest of the regions, there are still some differences between their attitudes. People in **North America** and **Africa** have more negative attitudes toward Trump, while people in **Oceania**have more positive attitudes toward Trump.

###  What people in different regions were talking about when they mentioned Trump?

From the distribution chart we can see that there are indeed differences between the attitudes of people from different regions, so why is there such a difference? Let's take a look at what people in different regions were talking about when they mentioned Trump.

<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width="100%" height="500" allowfullscreen="true" src="assets/img/2019_other_words_frequency_grid.html"></iframe>

**“American”**, **“campaign”**, **“democrats”**, **“country”** occur in most regions with high frequencies, they may relate to the same topic. But we can also see that some new words appear in different regions, and the attitude difference may relate to these new high-frequency words.



#### **North America**

<figure style="text-align: center">
    <img src="assets/img/2019_wordcloud_NorthAmerica.png" style="width:65%">
</figure>

The new word **"law"** appears in the North American buzzwords, perhaps this content is related to the more negative attitude of North America, let's see what content is related to **"law"**.

> Quotes containing **“law”**
>
> (1) been in the middle of Trump's barbs with her husband, George, a conservative **lawyer** who frequently makes headlines for his criticism of the president. 
>
> (2)First, the courts had it right to review the decision made by the Trump administration to end the DACA program, and second, the actions by the Trump administration were **unlawful** and unwise and consequential for many Americans.

Most of the contents that contain  "law" are criticizing Trump which tend to express the negative attitude.



#### **Africa**

<figure style="text-align: center">
    <img src="assets/img/2019_wordcloud_Africa.png" style="width:65%">
</figure>

**“Ukraine”** and **"Giuliani"** are new words appearing in the quotes mentioned by speakers from Africa.  both of them are related to **The Trump–Ukraine scandal**. The Trump–Ukraine scandal is president Donald Trump coerces Ukraine and other foreign countries into providing damaging narratives about 2020 Democratic Party presidential candidate Joe Biden as well as misinformation relating to Russian interference in the 2016  United States elections. This event has brought a lot of negative comments to Trump.

> Quotes containing **“Ukraine”** and **"Giuliani"** 
>
> (1) Absolutely. I am afraid it will be on my gravestone. Rudy **Giuliani**: He lied for Trump, 
>
> (2) Using the American embassy in **Ukraine** as their focal point to get dirt on Trump.
>
> (3) Will Trump's CIA director contact foreign nationals to aid in spying on Biden's aides? Will National Security Advisor John Bolton request that the names of surveilled Biden campaign officials become unmasked as a way of having them leaked to the media? Will Trump hire a British ex-spy to gather together rumors and gossip about Biden's previous overseas trips and foreign contacts, especially in the **Ukraine**, and then see them seeded among the Trump CIA, FBI, Justice Department, and State Department? Is that the sort of country we have now?  



#### **Oceania**


<figure style="text-align: center">
    <img src="assets/img/2019_wordcloud_Oceania.png" style="width:65%">
</figure>


People from Oceania have more positive attitudes compared to people from other regions. In Oceania, we see **“support”** among the hot frequency words, Let's see what content it comes with.

> Quotes containing **“support”**
>
> (1) The most visible manifestation of this is the **support** for Donald Trump
>
> (2) As former chair of RPOF chair... I am proud to **support** Donald Trump
>
> (3) Not even Ronald Reagan had as much **support** within the party as President Trump!

We can see that the attitude of the quotes that appear together with support is relatively positive.



## People's attitude towards Trump over year grouped by regions

So far, we've looked at people's attitudes in 2019. Let's look at the other years.

<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width="100%" height="500" allowfullscreen="true" src="assets/img/country_attitude_overyear.html"></iframe>

We see that the attitudes of different regions are changing over time. At the same time, the difference in attitudes between regions becomes larger as time goes on. The difference in attitudes is more pronounced in 2020. 

**Conclusion**

In general, differences in attitudes between regions exist and are becoming more obvious. This difference may be influenced by the quickly changing international situation. We think people's attitudes toward Trump are related to their regions.

In this part we have discovered how the factor region affects people’s attitude towards Trump. It would be nice if we could go beyond only grouping people by a single factor, so we perform a clustering procedure for people talking about Trump to see if there is any difference among clusters as shown in the next section.



## Cluster Analysis

Having viewed the results grouped by the nationalities and age groups,
we observed that there are people from different regions have
different attitudes towards Trump; however, different age groups does
not give the same result. In this case, we want to have a higher and
more abstract view of how different kinds of people have different
views or speak differently about Trump. We decided to do the
clustering based on speakers’ age, nationalities, genders, religions,
parties, and their education degrees. Data from Wikidata have too many
low level details and concepts. It is hard to analyse the data in its
raw form because the raw data bring in too many categorical values
that makes clustering analysis infeasible. Therefore, we make use of
the semantic links in the Wikidata database so that we can work on
fewer concepts that have broader semantics.

For clustering, we used K-prototype, which could deal with mixed data
continue variables and categorical variables. After getting the costs
tendency (see below), we decided to cluster speakers into 5
clusters.

<!-- Costs -->
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0"
width="100%" height="500" allowfullscreen="true"
src="assets/img/Costs_Trendency_depending_on_the_Number_of_Clusters.html"></iframe>

<!-- PCA Plots of Clustering -->
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0"
width="100%" height="500" allowfullscreen="true"
src="assets/img/PCA_Result_of_Clustering.html"></iframe>

The figures show the distribution of features for each
cluster as below.

<!-- Age Distribution -->
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0"
width="100%" height="500" allowfullscreen="true"
src="assets/img/Age_Distribution_over_Clusters.html"></iframe>

<!-- Candidate Portion -->
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0"
width="100%" height="500" allowfullscreen="true"
src="assets/img/Candidate_Portion_in_cluster.html"></iframe>

<!-- Education Portion -->
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0"
width="100%" height="500" allowfullscreen="true"
src="assets/img/Education_Portion_in_cluster.html"></iframe>

<!-- Gender Portion -->
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0"
width="100%" height="500" allowfullscreen="true"
src="assets/img/Gender_portion_in_cluster.html"></iframe>

<!-- Party Portion -->
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0"
width="100%" height="500" allowfullscreen="true"
src="assets/img/Party_Portion_in_cluster.html"></iframe>

<!-- Regions Portion -->
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0"
width="100%" height="500" allowfullscreen="true"
src="assets/img/Regions_Portion_in_cluster.html"></iframe>

<!-- Religion Portion -->
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0"
width="100%" height="500" allowfullscreen="true"
src="assets/img/Religion_Portion_in_cluster.html"></iframe>

Then, we want to see if there exists different quotes’ contents over
different cluster. We first calculated mean of each cluster for each
month based on BERT embedding matrix. And then we did 2-dimention PCA
for all of the mean vector.

<!-- All Speakers -->
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0"
width="100%" height="500" allowfullscreen="true"
src="assets/img/Total_Speakers_Time_PCA_Result.html"></iframe>

From the above figure, we could observe that although different
clusters had different quotes’ contents’ in early years (i.e. 2015,
2016), then, as time passed, all the clusters’ quotes’ contents tend
to be the same. This result also implies that people tend to talked
about Trump under a focused context after he became
president. Combined with the word cloud we have above, we could see
that the contexts focused more on the political aspects.

## Ending

In our story we have discovered many things around Trump have changed from who actually talked about him to the contents and attitude of each quote about him. We have also found some factors like region may influence people’s attitude. Furthermore, we used a clustering method to discover if there are higher dimensions of factors that may influence people’s attitude toward Trump. Among all the changes overtime, there is one thing that has never changed, that is, Trump never stops bragging about himself.


