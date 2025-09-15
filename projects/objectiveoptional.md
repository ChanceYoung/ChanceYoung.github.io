---
title: "Shipping My First Finished Game (10-Day Jam)"
permalink: /projects/objectiveoptional/
thumb: /assets/images/generic-thumb.jpg
summary: "How I scoped, built, and shipped my first finished game in 10 days."
tags: [gamedev, godot]
order: 10          # lower shows earlier in the list
featured: true     # appears on the home page grid
---

## Context
[*Objective Optional*](https://kiriyai.itch.io/objective-optional) was created for the [2025 Shovel Jam](https://itch.io/jam/shovel-jam-2025) and marks the first published game by **Fuzzy Stego Studio**.

The theme for the Jam was "Just Get Started". My wife and I began to brainstorm, and spent 3 of the 10 days discussing what we would do. We landed on the idea of an astronaut that keeps getting distracted by tasks on his way to actually start his mission. 

## Initial Design

We decided that we wanted this little astronaut to be woken up by an AI stating something along the lines of "Good morning, please get to the console to begin our mission. Oh and captain...dont dawdle." This meant that we needed a dialogue system of some kind, so it went on the todo list. 

We then started brainstorming tasks that would distract our poor astronaut from getting to his mission. We came up with the following list:
- Getting a cup of Coffee
- Repairing something in the ship

At that point, it

## Hardest Decision
```gdscript
if Input.is_action_just_pressed("jump") and is_on_floor():
    state = "jumping" 
   ```
  
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEwNDI0NzQzNjIsLTY1MzczMjQxMSw5OT
EzNzM5ODNdfQ==
-->