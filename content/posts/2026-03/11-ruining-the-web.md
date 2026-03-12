---
dateCreated: '2026-03-11T07:30:00-05:00'
datePublished: '2026-03-11T07:30:00-05:00'
title: 'Ruining the Web'
---
When you go to apply for a web development job,
but you CAN'T because the application form is broken.
🤦 Incompetent React developers are destroying the web!

It's a web form! A simple form. Some text inputs. A couple of select drop downs. A file upload. It's dead simple. Raw HTML has had the tools to do this since the 1990s! There's nothing for JavaScript to do here, let alone a full UI framework.

Yet some React jockey decided that this very basic form needed to be a Single Page App. And also decided that HTML's SELECT element is far too pedestrian and should be replaced by a stack of DIVs with dozens of ARIA attributes. But then failed to test their work on any browser other than Chrome, and so didn't know that their control is totally unusable in Firefox. And wouldn't it be cool to have a nice hover effect on the submit button? It would, but you screwed that up and the button becomes invisible when you hover. Even in Chrome.

If you're using React/Vue/Angular to build bog standard web forms, please, for the love of Sir Tim, STOP! You're not using that hammer to drive a nail. You're not even using a hammer to drive a screw. You're using a hammer to paint a window frame! If the features are supported in HTML, 
JUST USE HTML!
