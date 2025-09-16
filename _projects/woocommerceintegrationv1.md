---
title: "Woocommerce Integration Version 1"
thumb: /assets/images/generic-thumb.jpg
summary: "An Ecommerce to ERP solution"
tags: [C#, WooCommerce,]      
featured: true
layout: default    
---
## The Problem
Our team was asked to connect the power of our WooCommerce Wordpress website with our ERP system. 

## Technologies 
### WooCommerce
I had never worked with WooCommerce before this project. I found it very straightforward to set up a Webhook, and the pre-built trigger topics were extensive enough to cover my use case perfectly. I also think they have excellent documentation for their [Rest API](https://woocommerce.github.io/woocommerce-rest-api-docs/) which allowed me to understand the footprint of the JSON objects used by WooCommerce.

### .NET Framework 4.8 hosted via IIS
Although many of my core bachelors degree classes were in .NET Core, the Toolkit used to communicate with our ERP system only supports up to .NET Framework 4.8. After *a lot* of Google research, consulting the Toolkit documentation, and a little bit of idea bouncing on Chat GPT, I was finally able to piece together a working monolithic project that I could host on our on-premises IIS server. 

### 
## The Solution
Once again we visited the idea with the integration toolkit provided by our ERP system. This time, however, instead of using the binaries that allowed me to engage with Inventory documents, I was able to create Full on Customer Orders. The data flow went as follows:
```mermaid
graph LR
A(WooCommerce Order marked Completed) -- Webhook Payload --> B(WebOrderAPI) -- Transformed Order Information --> C(Infor VISUAL)
```
We chose to have the webhook trigger on "Completed" because we were using a 3PL company in order to actually fulfill our orders. The orders being created in our ERP were to mirror the actual cost and inventory flow out of 3PL. When the 3PL company would complete an order, their system would mark it "Completed" in our WooCommerce store.   





> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5NzQ5OTMzOTQsLTE4NjAzOTA1NDksLT
U5NzEyMDYyNCwtMTU1NjE0MjgyMiwxNzcwMjY3ODZdfQ==
-->