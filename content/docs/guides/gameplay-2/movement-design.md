---
draft: false
authors:
  - interestex
title: Movement Design
weight: 7190
date: 2024-11-30T00:00:00.000Z
contributors:
  - interestex
  - illusion2
  - psytrancegd
description: Movement is a core aspect of any game, and can make or break a
  game’s immersion and enjoyability. This guide will cover many fundamental
  details in the process of designing good movement systems.
tags:
  - Grade 2
  - Game Design
---
{{< callout context="note" title="TLDR - What this guide covers" icon="outline/info-circle" >}}




- Movement is the core of most systems and can make something as simple as traversing feel fun.
- Players should be able to see, hear, and expect a motion as soon as an input is executed.
- Movements should feel consistent to refine accuracy and skill as opposed to feeling random.
- Moving around should feel dynamic and satisfying, and the system should be easy to use.
- When travelling around, players shouldn’t be able to abuse the movement system to bypass everything, yet it shouldn’t feel like a chore to use.





{{< /callout >}}

- - -

# 1: What Is Movement Design?

**Movement design** usually refers to **how (and in what ways) the player moves around in their environment**. This is pretty crucial if you want to make a fun game, since the player spends most of their time using these mechanics to navigate—it wouldn't really be a fun game if you had to fight the controls to get to where you want to go.

# 2: What Makes Good Movement Design?

## Responsive Controls

If you want your player to feel like their inputs are WORKING in your game, you’re going to need responsive controls. **Responsiveness** refers to **the time in which the action pressed corresponds to the actual movement of your player**. If I press the right arrow key, the player should (as crazy as it sounds) move right, but good responsive controls let the player KNOW that the action is happening within a reasonable amount of time.

\-# *When swapping directions, you don’t immediately reverse which can lead to unintended results like falling off the platform at the end.*

{{< img src="https://lh3.googleusercontent.com/d/1wCsCU9JSutEoJEvGRiDxjAYUOUp5Oysk" >}}

This can be incredibly important depending on the game you’re making. For instance, if you want to make a precise platformer, you need your controls to be responsive to the point where the action happens *immediately* after the button is pressed. Input delay would make the game seem extremely unfair and annoying (which probably isn't fun). It isn’t a be all end all though, because unresponsive controls can feel more limiting which will need to new forms of gameplay as mentioned later on in the guide and also in [Mechanics 5](/docs/guides/gameplay-2/mechanics-5-limitations-strategy/), as long as it feels intended and still fun to use.

## Consistency

**Consistency** is **the accuracy of the same movement under repeated inputs**. If the player jumps, it should be to reach the same height no matter how many times it repeats. If a certain movement isn't consistent (meaning that it varies every time it's activated), it may seem like RNG for an input to happen correctly, since you’re pretty much at the game’s mercy of it working or not.

\-# *Small differences can lead to different results, even though the player did almost all of the inputs correctly. This is an example of a small part from Zip Lash by GD Colon*

{{< img src="https://lh3.googleusercontent.com/d/1I-RfBmkkp8kv6X_L84J3iHyHwh-2CqnQ" >}}

This might seem easy to do, but it really depends on how your mechanics are made. Having a movement that’s heavily influenced by other subtle aspects can feel inconsistent, even though you still generally get the same movement, because small things like the timing and the direction you’re moving can change a lot.

## Level design

Level design comes into play when you have a certain mechanic you want to use in the level. If you want your movement to seem like it's actually *useful* in your game, make sure the level requires them to use it when needed. If I have a dash mechanic, and nowhere in the level does it feel useful, why would I ever need it (if not to wave dash back and forth whenever I get bored ???) For every mechanic, there should be areas in the game where the player would find that “X mechanic works best here.”

There are plenty more layers to level design, but that’s outside the scope of this guide, so instead I’ll link you to the [Level Design](/docs/guides/gameplay-2/level-design/) guide.

## Player Feedback

**Player feedback** is **the visual/audible response given to the player after executing a certain input**. Although not as important, you should 100% keep this in mind to make it more obvious that input was performed successfully, instead of observing just off of movement alone. This especially comes into play when you want the player to execute several actions consecutively, by letting them know what the input was and when it happens. This is covered more in [Mechanics 3](/docs/guides/gameplay-2/mechanics-3-feedback/) as well.

\-# *The movement feels much more substantial and satisfying after the visuals and sound effects.*

{{< img src="https://lh3.googleusercontent.com/d/14pIqcMEaQ7dlxPZPdq_hcRqbvHBEVGjD" >}}

Here are also some more complex, but important ideas that should be thought about:

* Dynamism: **Dynamism** is pretty much **how dynamic (or fluid) the player’s movement is**. The player should be able to execute actions in a smooth manner that “flows nicely” with the main premise of the level. Adding this makes your game feel satisfying to go through and not feel so stiff. Without any type of dynamic movement, the movement can feel unpolished and annoying to use.

For example, if I was to make a platformer that uses different abilities consecutively to move from one area to another, it should be dynamic to the point where it’s easy to execute this sequence of actions without feeling too clunky/rigid. Player feedback plays a big role in this too, because having something feel satisfying can make it flow better too.

* Limitations/Freedoms: Limitations and Freedoms are 100% necessary for well-balanced movement, basically referring to what the player can (and can’t) do with their movement (i.e. I shouldn’t be able to skip whole parts of a level due to how broken a certain mechanic is). Limitations allow you to construct your main gameplay around a balanced movement system, allowing for some creativity when it comes to applying it to a game.

It is also pretty important to balance the player’s freedom’s and limits in a game. There shouldn't be too many limits to the point where the player has no freedom in executing something (making the game seem like a chore), and there shouldn't be too many freedoms to the point where the player can do literally everything, making them overlook your intended way of playing the game. For more on this, see the [Limitations](/docs/guides/gameplay-2/mechanics-5-limitations-strategy/) guide.

- - -

* Manageability: **Manageability** is **the idea of how manageable the required inputs are for an average player**. The player should be able to accurately execute controls that relate to what they want to do without it seeming confusing. If somebody had to press 2 or more different keys or press several keys at the same time like it’s Mortal Kombat in order to do a simple jump or dash, that wouldn't be very fair or manageable. The controls for your game should be simple and fair to execute, especially with the limited amount of keys GD has for platformer mode.

# 3: Examples

## Bad Movement System 1 (Dash)

{{< img src="https://lh3.googleusercontent.com/d/1iEdcQ5wbtVvOK2AJBa0KgNFkLWoSs6Iw" >}}

This is an example of a bad movement system. For starters, the dash feels WAY too inconsistent and unresponsive, making it hard to use it in the right way when it’s needed. Also, there’s no feedback for the player to know that a dash was used, apart from the movement alone.

{{< img src="https://lh3.googleusercontent.com/d/1JayiH2lnkK4pU5nVVRauuddc9fuoBN97" >}}

- - -

How do we fix this? We can try making the dash more consistent by using two teleport triggers instead of a force block, allowing the player to dash the same length with high speed. You can even add simple feedback to it, like a flash and a screenshake to show the player they executed the action.

## Bad Movement System 2 (Wall Jump)

{{< img src="https://lh3.googleusercontent.com/d/1BUNk82LoHKGpHUhVYSgtunjZzf0xcFzV" >}}

Here’s another example; a basic wall jump that you see in lots of levels. It gets the job done, but not only does it lack player feedback (which is extra annoying in this example as it just looks like weird sliding), but the weird bouncing makes the wall jump feel uncontrollable and inconsistent, making it less dynamic and harder to manage.

{{< img src="https://lh3.googleusercontent.com/d/1pWA8zpVtUKALnuj8BHd5zU0GtbwTAoty" >}}

- - -

To fix the player feedback, we can just simply add more **cues** (**visual/audio effects for the player to see**). Particles now appear when you wall jump, and a sound effect plays when you grab a wall, helping the player know that they *can* wall jump. The wall jump also now bounces the player out a bit, making the jump feel smoother (and actually like a jump) instead of weird sliding, while adding another visual cue to the wall jump. The player can also now slide down the wall rather than just fall, giving more overall freedom and making it more obvious (and noticeable) that the player can wall jump.

# 4: Advanced/Specific Concepts

These are the concepts that will take your movement system from a *good, fun* movement system to a *great, memorable* movement system; not required, but extremely useful for making your movement **stand out**.

## Innovation

The first step to make a unique and refreshing movement system is to make the mechanics themselves **unique and rarely done before**; in other words, **innovating**. These mechanics don't need to fundamentally be unheard of, but they should ideally be different enough to *feel* different. 

There's no easy way to innovate, as it all stems from the idea phase and being able to make unique ideas. However, it's still something to keep in mind when forming the concept for your mechanic.

Here's an example of innovating on a regular mechanic; the **strider** ability in **MIO: Memories In Orbit** turns a regular wall-climb into a spider-like mode that allows you climb quickly on *any* surface, on a limited supply of energy. 

{{< img src="https://lh3.googleusercontent.com/d/1g5c_L-NxCtGyffhcjLwWvpfX8vxIDSMC" >}}

This innovates in multiple ways:

* Allows you to climb on *any* surface, not very common
* Combines a "sprint" with a wall-climb 
* Limited energy turns wall-climbing into a resource, again not very common
* It *feels* different; the "function" is the same, but you aren't jumping off and onto walls like regular games.

## Expression

**Expression** refers to when **players are given freedom in how they progress through a part; how they express themselves**. The key point is that the movement system is incredibly versatile, and it's up to the player to figure out how they want to use this versatile movement to progress. Here's the fundamentals of versatile and expressive movement:

* **Innovation.** A new mechanic creates opportunities for creators to incorporate freedom and players to learn and express themselves. You won't be able to create expression with the usual mechanics everyone is used to.
* **Simple, with lots of interactions**. A simple component is able to be used in multiple different ways, and letting the player choose how to combine simple mechanics allows them to express themselves.
* **Level design**. Rooms designed around one critical path, such as a majority of rooms in Celeste, tend to limit expression and focus more on puzzles. However - this guide is on movement, so let's get back to that.
* **Sauce**. It's hard to describe, but it's simple; if your movement feels really sick and saucy, players *will* want to do cool things with the movement, and that leads to expression.

Expression in some ways is like a puzzle where players, while figuring out the solution, create their own unique and personal path through the section. As such, most expressive platformers tend to seem very barebones; you have simple movement mechanics, a starting point, and a vague destination. It's not instantly clear how to progress until you throw yourself at the wall and figure it out on the fly. 

Alongside extremely fun mechanics, this is what most people call **schmoving**; when you're set free and get to do *insanely cool things that feel personal*, rather than being guided through a set path by the creator.

## Movement Tech

Movement tech is short for **movement techniques**, which are **higher-level techniques within the movement system that allows the player to do more things**. While previously we went over *creative expression*, movement tech creates *skill expression* for players to learn even after completing the game.

Here's a quick example of movement tech in Hollow Knight: Silksong. This gif showcases regular sprinting first, before showcasing "dash jumping" and then "wavedashing"; all ways to move faster than regular movement.

{{< img src="https://lh3.googleusercontent.com/d/1DZyOMSqRtCGKyBq1PocrB_r7O7irLUzy" >}}

The best way to incorporate movement tech is via playtesting, and finding out what kind of cool things you can do with your movement. It's not easy, but creative minds and a good community will *always* find movement tech; you just need to find it first.

In addition to creating a small bit of expression (the player is doing cool things separate from the creator's guidance), what matters most is the **skill expression**. Most tech are too difficult to pull off in a blind playthrough, which adds more things to learn after the game, creating replayability and ultimately making the movement more memorable. The sense of difficulty also adds to the sense of accomplishment; mastering a difficult technique *feels good*. 

Additionally, a majority of
