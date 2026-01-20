---
title: Building a ship-wide peer network to allow offline messaging on cruise ships
description: During one of our student cruises, we built and tested a large-scale offline messaging system to allow communicating even when there is no internet. Let's see how it went.
pubDate: Jan 20 2025
public: "False"
---
If you aren't aware, it is totally possible for phones to communicate without the need for the internet. Even if you travel far into the forest or deep underground, where the only thing you can play is the t-rex game, you can still message your friends. Provided they are nearby. Your phones can send signals to each other through the air.

Usually this is not practical, but in certain situations - like in cruise ships - this could work quite well. The main problem is that the signal is quite faint. The idea is, however, that once someone has a message, they can distribute it to other people. This way the original sender doesn't even need to connect to all people. I'll go more into the details of this in the technical section. 

These kind of messaging apps of course require quite many users to be effective, but we had a unique opportunity to test this in the wild. At the end of the fall we had _Otacruise_. It is a trip to Stockholm with a boat full of Aalto-students. The whole boat is booked for us, so practically no outsides can get in. In the previous year we had problems with the internet, so a working messaging app would be very appreciated. Me and couple others then gathered a team and together we built a prototype of the idea, and tested it with a reasonably-sized group during the cruise. The idea would be that we would distribute the app just among our school, and when the time comes see if these kind of messaging system have any merit.


### Building & Technical details

We aren't the first to come up with this idea, but most people cannot test it in a large environment. Also some previous students have came up with this idea, but they have resorted to using some existing apps. We tested a couple and they were sub-par, requiring login or straight-up not working. We built our own version for three reasons.
1. We could say it was built for Otacruise, and we could add stickerse as memes. This would hopefully get people to use it more.
2. We don't need sign up. The easier it is to use the better.
3. We can gather telemetry data and actually see how well works.

Let's go through the idea more clearly
random walk

Intro
Building
Technical details
- internet vs bluetooth
- android vs apple
Results
- 