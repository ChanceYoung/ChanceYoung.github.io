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
## The Solution
Once again we visited the idea with the integration toolkit provided by our ERP system. This time, however, instead of using the binaries that allowed me to engage with Inventory documents, I was able to create Full on Customer Orders. The data flow went as follows:
```mermaid
graph LR
A(WooCommerce Order marked Completed) -- Webhook Payload --> B(WebOrderAPI) -- Transformed Order Information --> C(Infor VISUAL)
```
## Technologies 

### WooCommerce
I had never worked with WooCommerce before this project. I found it very straightforward to set up a Webhook, and the pre-built trigger topics were 
> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTI3NDExOTU2LC0xODYwMzkwNTQ5LC01OT
cxMjA2MjQsLTE1NTYxNDI4MjIsMTc3MDI2Nzg2XX0=
-->