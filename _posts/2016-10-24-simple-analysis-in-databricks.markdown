---
layout: post
title: "How to analyze California campaign cash in the cloud with Apache Spark and Databricks"
deckhead: "Use the Coalition's API to run SQL queries across millions of records from the comfort of your browser"
byline: "By [Bill Chambers](http://billchambers.me/about.html)"
image: http://www.californiacivicdata.org/img/databricks-promo.png
published: true
---

*Editor's note: This post was written (and submitted [via pull request](https://github.com/california-civic-data-coalition/california-civic-data-coalition.github.io/pull/15)) by a contributor to our open-source project who is also a Databricks employee.*

<figure style="margin: 8px 0 0 18px; float:right;" >
   <a href="http://billchambers.me/about.html">
    <img src="/img/bill-chambers.jpg" height="200" alt="Bill Chambers" style="float:right; clear:both;" title="Bill Chambers">
   </a>
   <figcaption style="float:left; clear:both;">Bill Chambers</figcaption>
</figure>

As a [past contributor](http://www.californiacivicdata.org/2014/11/24/postgres-support/) to the California Civic Data Coalition I've been really pleased with how much the project has progressed. It's amazing to see the state's [campaign finance and lobbying activity data](http://calaccess.californiacivicdata.org/downloads/latest/) in a simple, clean format that users can immediately work with.

However, with [some](http://calaccess.californiacivicdata.org/documentation/calaccess-files/smry-cd/) [tables](http://calaccess.californiacivicdata.org/documentation/calaccess-files/expn-cd/) stacking up millions of rows, the data are often too big for standard tools like Microsoft Excel spreadsheets.

The result is that most beginners will need to install a series of complicated computer programming tools before they can begin any analysis.

In my experience teaching at [UC Berkeley](https://www.ischool.berkeley.edu/courses/info/018) and on [Udemy](https://www.udemy.com/data-analysis-in-python-with-pandas/), I've observed students often get caught up installing that kind software on their machines, which hinders their introduction to our field.

### The Databricks fix

Now I'm working for new site called [Databricks](https://databricks.com/), which is aiming to solve this problem by making starting and sharing data science easier.

We doing it by harnessing the power of [Apache Spark](http://spark.apache.org/), a free and open-source tool for high-speed data processing that, for the most the part, is only used by super nerds.

Over the last 8 months, the Databricks team has been hard at work integrating Spark into a free [community edition](https://community.cloud.databricks.com/) where,  thanks to the power of cloud computing, even beginners can quickly import, transform and analyze gigantic data files using only their web browser.

### Take a test drive today with California's campaign cash database

When the California Civic Data Coalition [announced last month](http://www.californiacivicdata.org/2016/09/15/website-launch/) it was launching an API for accessing the latest data from the state's campaign finance database, I realized that our new [Databricks notebook](https://docs.cloud.databricks.com/docs/latest/databricks_guide/01%20Databricks%20Overview/03%20Notebooks.html) could make it easy for users to get started querying the data without having to install any software.

The Databricks notebook is an interactive workspace &mdash; similar to the [Jupyter Notebook](http://www.californiacivicdata.org/2016/10/08/first-python-notebook/) &mdash; where you can use your browser to code and collaborate in an easy-to-use environment that leverages our powerful Spark backend. You can see [numerous examples](https://databricks.com/resources/type/example-notebooks) on our site, or watch [the following introductory video](https://vimeo.com/137874931).

<iframe src="https://player.vimeo.com/video/137874931" width="100%"" frameborder="0" style="margin:10px 0;" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

What's amazing about Spark is that it can turn any structured files into an immediately queryable database. And CAL-ACCESS database that is cleaned and served by the California Civic Data Coalition is no different.

To see it in action, all you have to do is make an account and clone my [the Databricks notebook](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/346304/3910054895802185/484361/latest.html). Instructions on how to do that are [here](https://docs.databricks.com/user-guide/notebooks/index.html#importing-notebooks).

<figure style="margin: 8px 0;">
    <a href="https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/346304/3910054895802185/484361/latest.html">
        <img width="100%" src="/img/databricks-notebook.png">
    </a>
    <figcaption>Bill's CAL-ACCESS notebook in action</figcaption>
</figure>

Then push the "run" button and the notebook will automatically download and import the state's sprawling database. In mere minutes it will be available for exploration using SQL and other tools.

I've already used it to see top lobbying contributions within the data. What can you find?