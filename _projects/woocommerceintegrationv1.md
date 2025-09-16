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
I had never worked with WooCommerce before this project. I found it very straightforward to set up a Webhook, and the pre-built trigger topics were extensive enough to cover my use case perfectly.

## The Solution
Once again we visited the idea with the integration toolkit provided by our ERP system. This time, however, instead of using the binaries that allowed me to engage with Inventory documents, I was able to create Full on Customer Orders. The data flow went as follows:
```mermaid
graph LR
A(WooCommerce Order marked Completed) -- Webhook Payload --> B(WebOrderAPI) -- Transformed Order Information --> C(Infor VISUAL)
```
We chose to have the webhook trigger on "Completed" because we were using a 3PL company in order to actually fulfill our orders. The orders being created in our ERP were to mirror the actual cost and inventory flow out of 3PL. When the 3PL company would complete an order, their system would mark it "Completed" in our WooCommerce store.   





> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExNDAyNzcwMTcsLTE4NjAzOTA1NDksLT
U5NzEyMDYyNCwtMTU1NjE0MjgyMiwxNzcwMjY3ODZdfQ==
-->