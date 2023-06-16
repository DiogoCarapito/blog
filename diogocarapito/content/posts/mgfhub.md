+++
date = 2023-05-02T00:41:49+01:00
title = "mgfhub.com is now live!"
categories = ['projects', 'datavis', 'healthcare']
slug = ""
authors = []
tags = []
externalLink = ""
series = []
+++

I'm excited to announce that [mgfhub.com](https://mgfhub.com) is now live!

![](mgfhub.png "mgfhub.com"){ width=50% align="center" }

It's as a sort of "data visualization " for KPI's (indicadores) in Portuguese Primary Care.
I imagined it for more than a year, and it's trying to answer questions that I have in my day to day work:

- How many do exist?

- How do this KPI's work

- How to find specific KPI's (eg: which are related to diabetes?)

- What's the impact of each KPI in the main performance index (IDG)?

![](mgfhub_page.png "mgfhub indicadores"){ width=100% align="center" }

I also wanted to provide an easy link to SDM, a official platform with all the details of each KPI, but navigation is not very intuitive (you had to know the number of the KPI and then put it on a hiperlink. It's messy).

I've used Flask as my framework, Dash and Bootstrap to make it pretty.
I've hosted it on Render and the Cloudflare to manage the domain.

There are still some rough edges, it's a work in progress, but I'm happy with the results so far. =)