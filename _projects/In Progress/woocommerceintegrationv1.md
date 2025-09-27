---
title: "Woocommerce Integration Version 1"
thumb: /assets/images/generic-thumb.jpg
summary: "An Ecommerce to ERP solution"
tags: [C#, WooCommerce]      
featured: false
layout: default    
---
## Project Overview

-   **Span:** May – June 2023
    
-   **Context:** We needed a way to connect order completed in our webstore to our ERP system.
    
-   **Impact (TL;DR):** 2–3 bullets with measurable results (speedup, error reduction, adoption, etc.).

## Our Solution
Once again we visited the idea with the integration toolkit provided by our ERP system. This time, however, instead of using the binaries that allowed me to engage with Inventory documents, I was able to create Full on Customer Orders. The data flow went as follows:
```mermaid
graph LR
A(WooCommerce Order marked Completed) -- Webhook Payload --> B(WebOrderAPI) -- Transformed Order Information --> C(Infor VISUAL)
```
We chose to have the webhook trigger on "Completed" because we were using a 3PL company in order to actually fulfill our orders. The orders being created in our ERP were to mirror the actual cost and inventory flow out of 3PL. When the 3PL company would complete an order, their system would mark it "Completed" in our WooCommerce store.   

### The Backend
#### .NET Framework 4.8 hosted via IIS
Although many of my core bachelors degree classes were in .NET Core, the Toolkit used to communicate with our ERP system only supports up to .NET Framework 4.8. After *a lot* of Google research, consulting the Toolkit documentation, and a little bit of idea bouncing on ChatGPT, I was finally able to piece together a working monolithic project that I could host on our on-premises IIS server. 
#### Microsoft SQL Server
Although primarily interacted through by using the provided ORM, some data and checks were retrieved with direct queries to the on-prem Microsoft SQL Server using MSSQL.

### External Connections
#### WooCommerce
I had never worked with WooCommerce before this project. I found it very straightforward to set up a Webhook, and the pre-built trigger topics were extensive enough to cover my use case perfectly. I also think they have excellent documentation for their [Rest API](https://woocommerce.github.io/woocommerce-rest-api-docs/) which allowed me to understand the footprint of the JSON objects used by WooCommerce.

### What Worked Well
### What Didn't Work Well





> Written with [StackEdit](https://stackedit.io/).## Project Overview


<!--stackedit_data:
eyJoaXN0b3J5IjpbMjAwOTExMzA1NiwxNDA5MjcwNzk3XX0=
-->