---
date: '2025-09-09T07:30:00-04:00'
datePublished: '2025-09-09T07:30:00-04:00'
dateCreated: '2025-09-08T08:25:44-04:00'
title: 'React Apology 2'
---
**Do I owe ReactJS an apology? Part 2**
I posted an unpopular opinion. Pushback flooded in. Here's what happened:

> Unpopular opinion: The whole React/JSX ecosystem is a boondoggle that web developers should run, not walk, away from.

I've written in another post about the many developers who said the problem is not React, it's people misusing React.

Today I want to address some of the other responses.

While developers opinions on React were mixed, comments from people whose jobs center on site reliability and performance almost universally concurred with my opinion. I can't say this surprises me much. One of my biggest complaints about React apps in the wild is that they so often become bloated blobs of JavaScript that drag performance in the wrong direction. React itself is not so large, but apps built around it easily become so.

There was another common refrain in the comments that I take as legit criticism. In summary, it amounts to "good or bad, it's where the jobs are, so we have to use it."

That point is hard to argue against. I occasionally have to work on React apps myself, not because I like it, but because that's where the work takes me. It's a tough market to be job hunting, so having the skills requested by employers is essential. As individual developers, we don't have the level of influence necessary to turn a whole industry, even if we want to. We have to do the work that's available. You can't fight the system.

In the final analysis, has my opinion changed?

With a few caveats, no, my opinion is the same as before. But taking into account the above, I feel my message needs to be refined.

To senior developers and architects making technology choices, I say:

- If you're wondering whether you need React — you don't.
- If you think you might need React — you probably don't. Start with progressive enhancement and only pull in something like React when you truly hit a wall.
- If you're sure you need React — investigate alternatives anyway, and maybe do a quick spike with a simpler tech first before you make your final decision.

But, to junior developers trying to break into the industry, or journeyman developers who need to put food on the table: 

- Yes, learn (and advertise) React skills, if that's what the market demands.
- React is a sharp power tool, dangerous when used improperly. **TEST** for **performance** and **accessibility**, not just functionality.
- Level up your skills with other technologies, so that when you get to make the decisions, you can make well-informed ones.
