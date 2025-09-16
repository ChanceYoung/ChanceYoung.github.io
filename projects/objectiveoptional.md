
---
title: "Shipping My First Finished Game (10-Day Jam)"
permalink: /projects/objectiveoptional/
thumb: /assets/images/generic-thumb.jpg
summary: "How I scoped, built, and shipped my first finished game in 10 days."
tags: [gamedev, godot]
order: 10          
featured: true    
---

## Context

[*Objective Optional*](https://kiriyai.itch.io/objective-optional) was created for the [2025 Shovel Jam](https://itch.io/jam/shovel-jam-2025) and marks the first published game by **Fuzzy Stego Studio**.

The theme for the jam was **"Just Get Started."** My wife and I spent the first three of the ten days brainstorming what we wanted to make. We landed on the idea of a little astronaut who keeps getting distracted by odd jobs on his way to finally begin his mission.

## Initial Design

We decided that our astronaut would be woken up by the ship’s AI with a message like:

> **"Good morning. Please proceed to the console to begin our mission. Oh, and Captain... don’t dawdle."**

Naturally, this meant we’d need a **dialogue system**—so it immediately went onto the to-do list.

From there, we brainstormed small tasks that could delay the player. Our initial list included:

- Getting a cup of coffee  
- Repairing something on the ship

At this point, we were already three days in—and the itch to *actually start building* got too strong. I jumped in and began setting up a **standard character scene** in the **Godot Game Engine**.

## The Long, Winding Road

I spent a chunk of time experimenting with mechanics until I landed on a fun little **"weighted object"** system and a **slippery surface** mechanic. I used a collection of `TileMapLayer` nodes to toggle surfaces between normal and slippery, allowing for dynamic movement challenges as well as.

Additionally, I set up:
- Door connection points for navigation  
- Trigger zones and toggles for interactable elements  
- A lightweight object-pushing mechanic that tied into certain puzzles

It took more iteration than I expected to make something feel polished *and* playable.

## The Mad Dash

As the deadline loomed, things got hectic.

While my wife handled some UI assets and design, I dove into **level design**—which, in hindsight, I *really* should’ve started with. It’s one thing to make cool mechanics in a test room, but integrating them into a cohesive game space? That’s a whole different beast.

Deciding how to teach the player what to do was especially tough. We didn’t have time to implement the fully-featured dialogue system we had envisioned. So, we hacked together a crude but functional **task list**, then I quickly set up:
- Trigger zones for tasks
- A basic task manager system to track progression
- A start-to-finish gameplay loop that (mostly) worked

It wasn’t elegant, but it got the job done.

## Conclusion

We ended up placing **183rd overall out of 1100+ entries**, which I think is pretty great for our first finished game project.

Here’s what I learned:

- Everything takes more time than you think—even if you already know what you’re doing  
- Working on a team is both rewarding and stressful. It was a great chance to teach my wife some of the basics of Godot, programming, and game design  
- I struggle with accepting “good enough,” which might be why I’ve abandoned other projects in the past. Shipping something—even if it’s not perfect—feels incredible  
- Fun is subjective, but **designing the space where fun can happen** is a tangible and achievable goal

---

Want to try the game?  
 [**Play Objective Optional on Itch.io**](https://kiriyai.itch.io/objective-optional)
  
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM4Njc5OTAyMSwtMTA1MDY3MzQ3NSw2Nz
Q3MzE0ODYsLTY1MzczMjQxMSw5OTEzNzM5ODNdfQ==
-->