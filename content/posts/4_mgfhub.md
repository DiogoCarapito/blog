---
date: 2023-05-02T00:41:49+01:00
title: "mgfhub.com is now live!"
authors: ["diogo carapito"]
tags: ["projects", "datavis", "healthcare"]
cover:
    image: 4_mgfhub.png
    alt: "mgfhub.com"
---

I'm excited to announce that **[mgfhub.com](https://mgfhub.com)** is now live!

It's as a sort of search tool with data visualization components for KPI's (indicadores) that exists in Portuguese Primary Care.
I imagined it for more than a year, and it's trying to answer questions that I have in my day to day life as a Family Medicine Resident when I'm working with KPI's:

- How many KPI's exist?

- How do KPI's work?

- How to quickly find specific KPI's (eg: which KPI's are related to diabetes?)

- What's the impact of each KPI in the main performance index (IDG)?

Information was scattered in different places.
I ended up scrapping the data from the official platform (**[SDM](https://sdm.min-saude.pt/BI.aspx?id=001&CLUSTERS=S)**) and creating a database with all the information I needed.
I merged the info with the official documentation and created a webapp.

The information is displayed in **table** form, with filters and a search bar using fuzzy logic search. There is an alternate card form with some graphics too.

![mgfhub table](/post_images/4_mgfhub_table.jpg#center)

There is also a **sunburst** chart to visualize the weight of each KPI in the main performance index (IDG).

![mgfhub sunburst](/post_images/4_mgfhub_sunburst.jpg#center)

I've used **[Flask](https://flask.palletsprojects.com/en/2.3.x/)** as my framework, **[Dash](https://dash.plotly.com/)** and **[Bootstrap](https://dash-bootstrap-components.opensource.faculty.ai/)** to make it pretty.
I've hosted it on **[Render](https://render.com/)** and the **[Cloudflare](https://www.cloudflare.com/)** to manage the domain (even though for my subsequent projects I ended up using **[Porkbun](https://porkbun.com/)**, it's way simpler and close to the same price). 

There are still some rough edges, it's a work in progress, but I'm happy for what I've accomplished so far.