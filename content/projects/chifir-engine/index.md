+++
draft = false
title = 'Chifir Engine'
+++

{{< figure src="chifir.png" >}}

Chifir Engine was my second game engine project, and in many ways was better than Purpl.
I wrote it without using the C runtime or C++ STL and very few outside libraries. I never
really reached the point of it being anything close to an engine, but I designed and partly
implemented an RHI, and a lot of support code. After a certain point it was more of an
exercise in writing support code and platform glue than an engine, but I learned a lot from it.

A lot of what I did in Chifir would probably be terrible in a commercial product, but was very
valuable for learning how a lot of things work.

It supported a lot of platforms:

- Windows XP to 11, Universal Windows Platform, and Xbox One/Series X|S all in a single binary
- Xbox 360
- Original Xbox
- Nintendo Switch
- Linux

It dynamically detected CPU features at runtime, to allow older CPUs to work.

The RHI had backends for Vulkan, and Direct3D 8, 9, and 12. I also implemented a command buffer
system for the legacy Direct3D versions, so I could have eventually done multithreaded rendering
with them.

Chifir is an extremely strong tea drank in Russia. The logo I made is a commemorative Soviet postage
stamp of a samovar, which is a tea brewing device used in Russia. Chifir has a lot of caffeine,
and I drank it sometimes when I was writing the engine.
