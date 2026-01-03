---
date: '2025-09-08T09:00:00-04:00'
datePublished: '2025-09-08T09:00:00-04:00'
dateCreated: '2025-09-07T11:35:39-04:00'
title: 'React Apology'
---
𝗗𝗼 𝗜 𝗼𝘄𝗲 𝗥𝗲𝗮𝗰𝘁𝗝𝗦 𝗮𝗻 𝗮𝗽𝗼𝗹𝗼𝗴𝘆? 𝗣𝗮𝗿𝘁 1

I posted an unpopular opinion. Pushback flooded in. Here's what happened:

> Unpopular opinion: The whole React/JSX ecosystem is a boondoggle that web developers should run, not walk, away from.

I posted that with a humorous anecdote criticizing some React design decisions. Some people didn't appreciate my sense of humor!

Many devs defended React and its design to varying degrees. Their consensus: my bad impression of React comes not from its proper use, but from its misuse.

Nayan Sawyer pointed out: "It was created specifically to solve the problems of handling complex state on the client side".

Dave Edelhart explained: "React is a view management engine - it was never supposed to be an application framework."

Marc H. Weiner acknowledged some React apps suffer from "skill issues" when he said: "I have no issues creating super fast, lean UIs with React, in most situations. But it does take a fair amount of discipline."

🎴David Elster perhaps summed up this argument best: "Just use the tool right, stop blaming the hammer for people using it on screws."

In principle, I accept these arguments and agree. React was designed to solve the problem of maintaining a complex, highly interactive Single Page Application, replacing bug-prone spaghetti code of imperative DOM manipulations clobbering each other and generally being a nightmare to maintain.

On the other hand, Mason Wheeler countered by stating "if you're doing any non-trivial amount of coding on the frontend, 9 times out of 10 you're doing something very wrong". In other words, it's not your choice of tool, but your architecture that's at fault.

There was wide disagreement about where the line is between complex enough to require something like React vs simple enough to be done with progressive enhancement and lighter tools. 

James Hutchinson leaned far to the React side, declaring that an app with "even the smallest amount of complexity" will benefit greatly from React. 

My opinion is at the opposite end of the spectrum: if you're building 3D modeling software like OnShape or a Photoshop type app, you're basically building desktop software in a browser, and you're going to need specialized tools. Other projects would be better served by a progressive enhancement approach.

I acknowledge React has a niche. I just disagree with much of the industry about how big that niche is. I believe progressive enhancement is the correct approach for the vast majority of webapps. We should not be teaching new web devs that every project begins with create-react-app. We should start with functional HTML and forms, style it with CSS, and enhance the experience as needed with lightweight tools like HTMX. React can be added 𝘢𝘴 𝘢𝘯 𝘦𝘯𝘩𝘢𝘯𝘤𝘦𝘮𝘦𝘯𝘵 — without taking over the whole application — if that level of tool is called for in some specialized cases. But ALWAYS with a focus on accessibility and user experience.

Tomorrow: Part 2.
