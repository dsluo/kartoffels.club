---
title: Projects
date: 2022-03-03T21:49:40-05:00
draft: false
showAuthor: false
showDateUpdated: true
showPagination: false
showReadingTime: false
---

# Hobby Projects Only

I have done a lot of various projects for different programs and games. To get put on this list it has to meet one or more of these criteria:
1. Personal Favorite
2. Technically Difficult
3. Very Popular

If a project isn't on here you can find it on my Nexus or my GitHub, both are linked on the main page of the site.


# Final Fantasy XIV

I maintain a series of Upscaled Textures for the game.

They can be found at this address:
[Heliosphere](https://heliosphere.app/user/46fzf43g8s34q1x9z9xd8q7xkr)


This is the most technically challenging project due to:
1. The game frequently updates
2. The corpus is very large, so to avoid drowning users in 100s of GBs of data I have to pick and choose formats and scale factors carefully
3. The way the image data is stored varies wildly and some is entirely unique to the game. In many cases I have had to write my own code to extract, transform and load the data.

Here are several github pages related to my work on ffxiv.

- [migration to the latest game version which overhauled a LOT of data](https://github.com/emarron/ffxiv_7_0_upscaled_textures_migration)

- [a tool to handle the proprietary FFXIV image format](https://github.com/emarron/ffxiv-tex-converter)

- [a uv island padder related to the scripts/id_bands/* of ffxiv_7_0_upscaled_texture_migration repo](https://github.com/emarron/island-padder)
- [a fork of an existing FFXIV tool with some batch data tools added](https://github.com/emarron/FFXIV_TexTools_UI)
# Baldur's Gate 3

[Unique Tav Custom Appearance](https://www.nexusmods.com/baldursgate3/mods/2754)

Separates the NPCs' customization options from the Player's. This is done via redirecting large amounts of XML chains. This mod is very popular.

The github repository is [here](https://github.com/emarron/unique_tav)

# Elder Scrolls Projects


### Overall
[Elder Scrolls Lore Bots](https://github.com/emarron/elderscrolls-lore-bots)
Small weeklong project to test vector embeddings on common LLMs. The Chatgpt one is quite good. Basically you can ask the model a question about Elder Scrolls game lore and it will be able to answer you and cite the source. I cleaned about 8k in-game books for this.

I wouldn't really define this as technically difficult. However it's outside of my normal line of work, and LLMs are all the rage these days.

### Skyrim SE

[Cleaned Skyrim SE Textures](https://www.nexusmods.com/skyrimspecialedition/mods/38775)

One of the first mildly complicated data engineering projects. I had to identify
1. What was upscaled poorly by bethesda by checking delta's from Skyrim Legendary HD, and reverting to that.
2. Then 'cleaning' all the data and saving it to DDS BC7 format for higher quality at a very small cost.
3. As a result this mod makes the game look AND perform better (to the tune of 500mb of VRAM saved)

This mod is something I've been particularly proud of and as is very popular.

### **Morrowind**

[Facelift](https://www.nexusmods.com/morrowind/mods/47617)
and
[Facelift Tamriel Rebuilt](https://www.nexusmods.com/morrowind/mods/53935/)

This improves the meshes (and textures) of the original morrowind heads to animate properly and remove various issues. It's a personal favorite just because I enjoy tweaking the faces.

### **Oblivion**

[Oblivion Upscaled Textures (OUT)](https://www.nexusmods.com/oblivion/mods/49351)

[DLC Upscaled Textures (DLCUT)](https://www.nexusmods.com/oblivion/mods/49798)

[Shivering Isles Upscaled Textures (SIUT)](https://www.nexusmods.com/oblivion/mods/49645)

These are my first large projects. This is around when video game upscaling via ESRGAN became viable. It would not meet my current standards, but as I said, these were my first large projects so I had to include it. It's also quite popular still.