
# Deloitte Forage Simulation: Client Insights Dashboard

 **Simulation Provider:** Deloitte (via Forage)  
**Tool Used:** Tableau (public data view link included)

**Focus:** Visualizing client data to identify business insights and improve decision-making.

## Overview

As part of Deloitte's virtual job simulation on Forage, I was tasked with developing a client insights dashboard using Tableau. The project focused on key KPIs to help inform strategic consulting recommendations.

## Objectives
- This project analyzes telemetry data collected by Daikibo, a multinational manufacturing company with factories located in:

Meiyo (Tokyo, Japan)

Seiko (Osaka, Japan)

Berlin (Germany)

Shenzhen (China)

Each factory operates 9 machine types that transmit telemetry signals every 10 minutes. The data, unified into a single JSON file, reflects machine activity over a one-month period (May 2021).

## Business Objective
Daikibo leadership needed to answer two critical questions to improve operational reliability and reduce production downtime:

* Which factory experienced the highest machine failure (downtime)?

* Which machines contributed most to that downtime in the affected factory?

## Analysis Workflow

* Downloaded and unzipped the telemetry dataset: daikibo-telemetry-data.json

* Imported the JSON file into Tableau Desktop for visual analysis.

* Registered and set up Tableau using the licensed trial version.

* Created a calculated field in Tableau named "Unhealthy", which assigns a value of 10 minutes for every telemetry log labeled as "unhealthy".

Formula used: **IF [status] = 'unhealthy' THEN 10 ELSE 0 END**

*This metric estimates potential machine downtime per message since each machine sends data every 10 minutes.*


 **Sheet 1: “Down Time per Factory”**

* Created a bar chart showing total downtime (in minutes) for each factory.

* Allowed identification of the location with the highest overall machine failure.

 **Sheet 2: “Down Time per Device Type”**

* Built a second bar chart showing total downtime by machine type, segmented within each factory.

* Used to isolate the most failure-prone devices.

* Combined both sheets into a single dashboard.

* Configured “Down Time per Factory” bar chart as an interactive filter:

* Selecting a factory dynamically updates the device-level breakdown for that specific location.

  *This enabled granular insights into which machines were driving failures in the worst-performing factory.*

## Skills Demonstrated
- Data visualization & storytelling with Tableau
- Business intelligence interpretation
- Client-focused problem solving
- Practical exposure to consulting workflows

## Credential & Links
https://forage-uploads-prod.s3.amazonaws.com/completion-certificates/9PBTqmSxAf6zZTseP/io9DzWKe3PTsiS6GG_9PBTqmSxAf6zZTseP_bXc6ibNMZJQY5tcz2_1750143141652_completion_certificate.pdf

https://public.tableau.com/app/profile/titilayo.kuloyo7922/viz/daikibo-telemetry-data_17530340598540/Dashboard1



