+++
date = '2025-07-02'
draft = false
title = 'Minecraft WASM runtime'
+++

This project embeds a WebAssembly runtime into Minecraft, and also renders a framebuffer
into the world as blocks. I wrote a couple Python scripts to find the average colour of
each block texture in the game, and then map block names to a list of colours in a palette.
The guest program can swap the palettes and write to the framebuffer however it pleases, which
is enough to run DOOM's main menu. Had I figured out a good way to implement user input, the
game would have been fully playable within Minecraft. It uses a datapack containing the palettes
and program. Additionally, I had to write a script to dump DOOM's palette data so I could use it
in the mod.

[GitHub](https://github.com/MobSlicer152/mcraster)

{{< video src="doom.mp4" >}}
