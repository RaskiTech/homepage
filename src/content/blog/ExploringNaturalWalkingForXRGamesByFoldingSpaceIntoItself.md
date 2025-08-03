---
title: Exploring natural walking for XR games by folding space into itself
description: In the last half a year I have been working quite a lot with the meta quest headsets. I've noticed that in many games walking around is quite a poor experience - mainly done with the joystick. In this post I'd like to present some ideas for a way of movement that we see barely used.
pubDate: Aug 3 2025
---


In the last half a year I have been working quite a lot with the meta quest headsets. Through my work I have been able to test their functionality and develop applications for them. I can safely say they are really cool! However, in many games walking around is quite a poor experience - mainly done with the joystick. In this post I'd like to present some movement ideas that we as developers could consider as we develop games for these glasses.

There have been a bunch of science-fiction-like machines that are meant to simulate natural walking. The image below is not the kind of natural walking we're talking about today. The idea here is that the user has a fixed (rectangular) room area in real life where they are able to walk around, and we as game designers are trying to make the most out of that room. The real-life space could be 3m x 3m, but our game worlds are usually quite a bit bigger. So the question comes down to this: How can we fit as much in-game space into a fixed amount of physical space?

![](../images/naturalWalkingMachine.jpg)

### Exploiting verticality

While the user might have some space to walk on the ground, they likely aren't going to move that much vertically. We can use this to our advantage, and extend our virtual levels upwards. There are likely many different ways we can transfer between these vertical levels. I've come up with two different approaches I'll show here.

**Elevators** - This is the most straightforward solution, which is why I'll discuss it first. The idea is that some part of the player's real-life walking space moves them up in the virtual world, allowing the player to access new areas while still in the same physical space. Most of the time in the game this is implemented as an elevator, but it could be some sort of teleport pad as well.

**Stairs** - Stairs don't differ from the elevator that much - the main difference being that the user has to walk in a direction to move between floors. Honestly just these two techniques seem really powerful, and could be used to explore towers for example. I made a sample scene to test the stairs. It's hard to describe how much more immersive it feels to actually walk around as opposed to using a joystick, but I can assure you the experience is at least 3x better.

<video width="600" controls>
 <source src="/content/StaircaseVRDemo.mp4" type="video/mp4">
</video>

Here I'm accessing new areas in the virtual world while only doing circles in real life. These two techniques are just the ones that came to my mind. If you have other good ideas on traversing between floors, I'd be eager to hear them.

### Using non-Eucledian space with portals

Portals allow you to create space where there are none, so they are an effective solution to our problem. They are also really unique, as portals are something that don't exists in our universe. Therefore they break a bit of immersion, but are still really cool. They could work well in a sci-fi escape room, for example.

Not surprisingly I'm not the first to think of this concept. If you are interested in this concept, there is a fantastic paper by a couple researches from the University of Cape Town. The paper is called [VR Natural Walking in Impossible Spaces](https://people.cs.uct.ac.za/~jgain/wp-content/papercite-data/pdf/lochner2021.pdf) and it has explored this concept a lot. The general idea is that if your game or application is indoors, you can fuse many rooms on top of each other. As you go through the house you discover new rooms, even though you are only walking circles. In the game this seems like a non-euclidean space, but any sane developer will implement this using portals. You can put the portals seemlessly in corridors and alike to hide the transitions to different rooms. Watch the slightly comedic video below to see the effect.

<iframe width="560" height="315" src="https://www.youtube.com/embed/WErjyjvM0JY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="border-radius: 10px"></iframe>

Teleportation in its purest form could also be used: stepping onto a teleport zone instantly moves the player to a different level — no smokescreens, no disguises. While this does break immersion slightly, it's still a worthy tradeoff for preserving natural walking.

### Conclusion

The concept is really good, but it's not surprising not that many games actually use it. Finding a big enough room without any obstacles is not that easy, and it is a necessity for these games. It is also noteworthy that not all games can benefit from this, as some simply require way too much traversal. Luckily many VR games focus on not needing to move that much, so many actually could benefit from this kind of design. If you ever get the change, I'd recommend to test this kind of movement in a game. In the end, though, this strategy might be best suited for escape room venues that have designated areas for these games.