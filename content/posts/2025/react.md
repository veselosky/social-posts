---
date: '2025-09-04T07:30:00-04:00'
datePublished: '2025-09-04T07:30:00-04:00'
dateCreated: '2025-09-01T18:59:07-04:00'
title: 'React'
---
Unpopular opinion: The whole React/JSX ecosystem is a boondoggle that web developers should run, not walk, away from.

I just wonder what the conversation sounded like when this stuff was invented.

Jr. Dev: We have a lot of web pages to produce. I better get started coding that HTML.

Sr. Dev: No way! I'm a programmer! HTML isn't even a programming language. I have a much better idea. Let's invent a new programming language that kinda looks like HTML, but uses JavaScript syntax. Then we'll write a compiler that turns that into a JavaScript file. We'll ship the JavaScript to the client, and THAT will build the page.

Jr. Dev: Buuut... won't that be pretty inefficient, building the whole UI on the one JavaScript thread, instead of letting the browser's optimized, hardware-accelerated native code do the work?

Sr. Dev: Nah, I've got a solution for that. We'll write a runtime engine that we ship to the client too. Instead of doing all those slow DOM operations, the runtime will make a copy of the entire DOM using JavaScript objects. And it will operate on a clone of that instead. Then we'll do a diff between the two fake DOMs to determine the minimal actual DOM operations to perform. So efficient!!

Jr. Dev: That sounds like it would eat up a lot of memory unnecessarily.

Sr. Dev: Who cares? Everyone has 64GB now.

Jr. Dev: In their phone? And, I still don't see how that would speed up the initial page load. Parsing and executing all that JavaScript—

Sr. Dev: You worry too much! This will be great! 

Jr. Dev: You know what? My uncle has a landscaping business. I'm gonna go work for him. This job really isn't for me.

Sr. Dev: Whatever, it's your loss. I'm going to start writing a code generator to generate all this boilerplate I just invented!

----

Don't agree? Alex Russel has a four-part series of posts that may change your mind: https://infrequently.org/2024/08/the-landscape/
