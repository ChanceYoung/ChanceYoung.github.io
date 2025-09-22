---
title: "Firearms Packaging Solution Version 1"
thumb: /assets/images/generic-thumb.jpg
summary: "An inventory and packaging web application."
tags: [Node, React, C#]      
featured: false
layout: default    
---
## Project Overview
#### Project Span: September 5-13 2023
### The Problem
Our team was asked if there was a way to reduce the human error in manual entry of a serial number into our ERP system. See, they were manually entering serial numbers into the system, which at its peak was over 300 guns per day. Thats a LOT of room for human error to creep in. A poorly written letter here, and 8 that looks like a B there, all leading to transactional issues and lost company time.

### Our Solution
The ERP system we used provided an integration toolkit written in .NET that used an ORM library in order to create business documents. After a little bit of research I discovered I could use it to create transactions within our ERP, if given all the information about the Work Order. This would found the basis of our Backend functionality. In an attempt to kill two birds with one stone, I also discovered [Label LIVE](https://label.live/), a label design and printing software, which could be sent standard HTTP requests in order to print out labels. This lead to the basis of our Frontend design, which would end up orchestrating the sending of a transaction request to our backend, as well as retrieving information and requesting printing from our Label LIVE software. 
### What Worked well
### What Didn't 
### The Backend
### The Frontend


## Project Overview

-   **Span:** September 5 – September 13, 2023
    
-   **Context:** The packaging team needed to stop entering Serial Numbers manually while receiving new guns into inventory.
    
-   **Impact:**
	- At peak over 300 firearms/day automatically received into system
	-  
    

## The Problem

The Final Assembly and Packaging team was receiving new firearms into our inventory while entering in Serial Numbers manually. We were asked to solve this problem in order to prevent future errors in Serial Number entry for ATF compliance. 
Describe the issue you were solving in clear terms. Who was affected, and what were the stakes?

## Constraints & Requirements

What made this challenging? (e.g., compliance, scale, time, legacy systems, cost).

## The Solution

High-level explanation of what you built and why. 2–3 paragraphs max.  
_(Insert Mermaid flowchart or diagram if relevant.)_

## Technical Implementation

### Backend

-   Tech stack, main services, architecture choices.
    
-   Key challenges & solutions.
    

### Frontend

-   Frameworks, UX decisions, key workflows.
    
-   User safeguards, accessibility, etc.
    

### Integrations

-   Third-party tools (APIs, SDKs, printers, etc.).
    
-   How you orchestrated data flow.
    

## Results

-   Quantitative outcomes (performance, errors, throughput).
    
-   Qualitative outcomes (user feedback, process improvements).
    

## What Worked Well

Bullets or short sentences.

## What Didn’t Work

Be honest — highlight tradeoffs, pitfalls, or learning opportunities.

## Future Improvements

What you’d like to add, refine, or expand on later.


> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE1OTU1NDYyMjAsMTI2ODExNTAyMSwxMz
E1MDg0ODk2LC0xNzQ2Njg4ODY2LC0xMTk5ODUwMTU3XX0=
-->