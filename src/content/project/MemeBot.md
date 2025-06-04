---
title: 'Memebot discord bot'
description: 'A python implementation of a discord bot for interacting with the memesite API'
pubDate: 'Mar 20 2021'
heroImage: '/Memebot.webp'
tags: ["Python", "Graphics"]
sortNumber: 100
---
## Summary

MemeBot is a Discord bot designed to interface with the MemeSite project. This bot allows users to engage with [Memesite](https://madswolf.dk/projects/memesite) by performing two main functions: uploading memes and fetching randomized memes based on a seed.

The randomization included many different possible operations:

- Mirroring
- Change saturation
- Pixelation
- Increaing noise
- Sharpening
- integration with random faces

The project included an integration with one of my friend's projects where a random face was generated based on a seed. His project can be found [here](https://tobloef.com/projects?project=face-generator).
The faces would be generated based on the same seed as the rest of the meme, and then a placement and orientation would be chosen randomly. A fun extra feature for this integration would be to use CV to detect faces in memes and randomly replace the face with one of the random ones.

The randomization features provide a many different variation with little seed content and is a entertaining way for users to interact with memes.

## Insights

During this project is learned a lot about self hosting a service as i hosted it on my own rasberry pi at home.
I also learned the strength of choosing the right language for the job, python was definetly the way to go for this project, as the ease of use and relatively small amount of code is just right for python.

## Links

The projects code can be found [here](https://www.github.com/madswolf/memebot).
