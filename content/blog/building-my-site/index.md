+++
authors = ["Stepan Bargl"]
title = "How I built my blog"
description = "Building a blog site with Zola"
date = 2026-07-26
[taxonomies]
tags = ["tech", "self-hosting"]
+++
I got the urge to build a blog site after I saw Vasilios Syrakis' [site](https://vsyrakis.dev/blog/) where he's using **Zola** and **Duckquill**. For me I thought this was the perfect place where I could share my own work and other things. I always wanted a space where I could dish out my own thoughts and opinions without the need to perform a certain way or post certain topics.

To begin I researched how could I host such site without tearing my hair out. At first I tought the way to do it would be using a VPS. This wouldn't be the way as I was looking at it more and more. Then I discovered that Cloudflare provides a service called 'Cloudflare Pages'. Its essentialy a more automated way to create static sites. 

Luckily I already had a domain registered at cloudflare, so I was sort of familiar with the dashboard. Using the zola docs, I followed the instructions on how to create a Zola site with Pages. The link to the guide is [here](https://www.getzola.org/documentation/deployment/cloudflare-pages/).

That was the hosting part. Now came the actual building of the site. At first I was confused how Zola initialy worked. I expected it would be an engine running on a server, that would create sites using commands. 

In reality it isn't installed on a server, but on a client device. The user creates and edits the sites on their device. When they have edited everything they needed, they then use git to update the repository. When the repository is updated the Cloudflare Pages worker checks the repo for new updates. When new updates are detected, it starts creating/mirroring in the changes in repository. After it's gone through the changes Pages then publishes the site.

So now we have talked about hosting and building, but we also need a theme for our site. **Duckquill** struck me as perfect theme for blog site. It's relatively simple, however I do like the simple aesthetic of it. I understand it's not everyones cup of tea, but it's my site not yours.
This was the hardest part for me to figure out, since I never worked with markdown or anything of that sort.

The repo had already a few examples on how sites would look. I simply copy and pasted the examples to my blog and using trial and error method I slowly was shaping my idea for this blog site. It's not perfect, it might not even be good. But I am happy with how it turned out.

I want to keep this blog short. I wanted to do a step by step guide on how to set this up, but I got lazy and just wanted to put my experience out there. You can set it up on your own without anyones help. I know I did. It's not perfect, but I like the way it turned out.

Thank you to Vasilios Syrakis, daudix (creator of duckquill), Vincent Prouillet and other contributors of Zola for making these tools and inspirations.

If you have any questions or feedback please send me an email: <stepan@bargl.org>