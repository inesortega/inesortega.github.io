---
title: "pelletMap — tracking the Galician pellet crisis in real time"
collection: personal
type: "Citizen-science platform"
permalink: /personal/pelletmap
date: 2023-12-15
project_link: https://noialimpapellets.publicvm.com/
---

On December 8th, 2023, the merchant ship CSAV Toconao lost half a dozen containers off the coast of Portugal, containing millions of plastic pellets. Weeks later, the spill reached the shores of Galicia, causing one of the largest environmental disasters in recent years.

![](/images/mapaPellets.png)

In order to monitor the evolution of the crisis, assess the impact, and provide information to the public about the state of the beaches and upcoming volunteer cleanup efforts, a massive data collection effort began through a web form where the state of the beaches and new cleanup events can be recorded.

So far, the processing of maps for visualization has been manual. In order to facilitate this task and enable automatic processing, over the course of a week I built a web application in R/Shiny to track the pellet crisis in real time — integrating automated data ingestion, geocoding, interactive map visualization, and statistical analysis.

You can access the website through this [link](https://noialimpapellets.publicvm.com/), or through the [Noia Limpa association's page](https://www.noialimpa.org/informacion-pellets-plastico-galicia), and join the effort of hundreds of volunteers in finding sustainable solutions for managing the environmental crisis.