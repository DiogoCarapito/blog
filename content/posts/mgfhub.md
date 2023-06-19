---
date: 2023-05-02T00:41:49+01:00
title: "mgfhub.com is now live!"
authors: ["diogo carapito"]
tags: ['projects', 'datavis', 'healthcare']
cover:
    image: mgfhub.png
    alt: "mgfhub.com"
---

I'm excited to announce that **[mgfhub.com](https://mgfhub.com)** is now live!

It's as a sort of search tool with data visualization components for KPI's (indicadores) that exists in Portuguese Primary Care.
I imagined it for more than a year, and it's trying to answer questions that I have in my day to day life as a Family Medicine Resident when I'm working with KPI's:

- How many KPI's exist?

- How do KPI's work?

- How to quickly find specific KPI's (eg: which KPI's are related to diabetes?)

- What's the impact of each KPI in the main performance index (IDG)?


I also wanted to provide an easy link to SDM, a official platform with all the details of each KPI, but navigation is not very intuitive (you had to know the number of the KPI and then put it on a hiperlink.
It's messy).

I've used **[Flask](https://flask.palletsprojects.com/en/2.3.x/)** as my framework, **[Dash](https://dash.plotly.com/)** and **[Bootstrap](https://dash-bootstrap-components.opensource.faculty.ai/)** to make it pretty.
I've hosted it on **Render** and the **[Cloudflare](https://www.cloudflare.com/)** to manage the domain (even though for my subsequent projects I've been using **Porkbun**). 

There are still some rough edges, it's a work in progress, but I'm happy for what I've accomplished so far.