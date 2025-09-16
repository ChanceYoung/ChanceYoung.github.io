---
title: "Firearms Packaging Solution Version 1"
thumb: /assets/images/generic-thumb.jpg
summary: "An inventory and packaging web application."
tags: [Node, React, C#]      
featured: true
layout: default    
---
#### Project Span: September-
## The Problem
Our team was asked if there was a way to reduce the human error in manual entry of a serial number into our ERP system. See, they were manually entering serial numbers into the system, which at its peak was over 300 guns per day. Thats a LOT of room for human error to creep in. A poorly written letter here, and 8 that looks like a B there, all leading to transactional issues and lost company time.

## Our Solution
The ERP system we used provided an integration toolkit written in .NET that used an ORM library in order to create business documents. After a little bit of research I discovered I could use it to create transactions within our ERP, if given all the information about the Work Order. This would found the basis of our Backend functionality. In an attempt to kill two birds with one stone, I also discovered [Label LIVE](https://label.live/), a label design and printing software, which could be sent standard HTTP requests in order to print out labels. This lead to the basis of our Frontend design, which would end up orchestrating the sending of a transaction request to our backend, as well as retrieving information and requesting printing from our Label LIVE software. 
## The Backend
### What Worked
### What Didn't 
## The Frontend
### What Worked
### What Didn't 
> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTIwNDc4Mjg1XX0=
-->