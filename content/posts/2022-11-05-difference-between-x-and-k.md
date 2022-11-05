---
title: difference between x and K
date: 2022-11-05T07:23:24.933Z
description: honk
categories:
  - upscale
  - tutorial
showTableOfContents: false
draft: true
---


## I HAVE HAD TO EXPLAIN THE DIFFERENCE BETWEEN "x" AND "K" SO MANY TIMES, PLEASE READ THIS.

N = number
x = any given resolution
K = usually 1000 or 1024 resolution
texture = image that a game reads and puts onto a 3d model

#### example:
4x = 4 times the given resolution of a texture
4K = 4096x4096 texture

2x = 2 times the given resolution of a texture
2k = 2048x2048 texture

## Okay, why are you defining your packs by 4x, 2x, 1x?

When I say my textures are 4x, it means they are 4 times the resolution of each image within the set. Each set has a massive amount of textures of different sizes. I have a small sample set to illustrate this below.
#### example:
we have a set of armor:
`set = [head, body, hands, legs, feet]`
the resolution of the set is as follows:
`set_resolution = [512x512, 1024x512, 512x512, 512x512, 256x256]`
we upscale it by a factor of 4:
`4(set_resolution) = [2048x2048, 4096x2048, 2048x2048, 2048x2048, 1024x1024]`
Basically, it would be a misnomer to identify the set by the highest resolution, when there are hundreds or even thousands of images in a set.

### Why are textures different sizes?

Imagine you are a game dev. If I have a coin, does it need to have 4k textures? No, because a coin is really small and no one looks at them. What about a huge city door? Yes, you may want 4k here. Players like to ram their faces into doors and this door is huge anyway. The combo of large world space and large screen space means higher resolution is better. All game developers (hopefully) optimize the items around these principles:

 - Insignificant and small = low resolution 
 - Significant and large = high resolution

**AND**

 - How good/bad are the computers the game is running on?

## So you just use a scalar?

The original developers have already selected the size ratios for the textures of each model. So to upscale the textures I can just slap a scalar onto them for better computers and higher resolution / larger monitors. 

There is a lot more that goes into then the scale factor, like:
data locating, data extraction, data identification, data partitioning, appropriate cleaning model for data, appropriate super-resolution model for data, more resizing, compression, more compression, QCing, packaging...
but yeah, in a nutshell bigger number == better.

### Something about monitors?
Remember above I talked about screen space? In a nutshell, the better your monitor is the more you will notice low resolution textures. The sad thing about a better monitor is that it taxes your system more, AND then you also notice how low resolution some things are, AND in order to use high resolution upscales you need to tax your system even more. 

