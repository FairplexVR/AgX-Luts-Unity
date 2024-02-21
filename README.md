## AgX Tonemapping for Unity

![Screenshot_7](https://github.com/FairplexVR/AgX-Luts-Unity/assets/31825109/c21a5d90-6ee3-43a6-8bff-c352057ed1d7)

### What is this?

AgX is the new color transform introduced in Blender 4.0, surpassing Filmic and ACES in many aspects. This repository contains a collection of AgX LUTs that are compatible with Unity BIRP and HDRP only. (Sorry URP!)

This Unity pack is inspired by the original [AgX by Troy Sobotka](https://github.com/sobotka/AgX) and the [Blender AgX implementation](https://github.com/EaryChow/AgX). The LUTs in the pack are configured to provide visual consistency with Blender's OCIO presets:

- Base Contrast
- Medium High Contrast
- High Contrast
- Very High Contrast
- Medium Low Contrast
- Low Contrast
- Very Low Contrast
- Punchy
- Greyscale

Check out the [Blender release notes](https://developer.blender.org/docs/release_notes/4.0/color_management/) for more information about AgX.

### Achieving a 1:1 View Transform between Blender 4.0 and Unity!

With AgX, you can now achieve a similar look between Blender and Unity:

![296376429-7d55092b-93c0-46a9-93dc-2c4eacde757d](https://github.com/FairplexVR/AgX-Tonemapping-Unity/assets/31825109/a4287499-fe71-46bd-9439-db3872e56894)
*<div align="center">The lightmap is baked using Cycles and supplied to a custom shader, resulting in a nearly identical appearance.</div>*

### Comparison between Tonemappers

![Screenshot_5](https://github.com/FairplexVR/AgX-Luts-Unity/assets/31825109/675911cb-5bf1-4b39-bbd5-7dee3e2af6a2)

### Installation

If you're not familiar with external LUTs in Unity, follow these steps to set it up. Assuming your project is configured in Linear Color Space with a working Post-Process, here's how to add the external LUTs:

1. Download the Unitypackage from from [the release page](https://github.com/FairplexVR/AgX-Tonemapping-Unity/releases/tag/1.0.0) and import it your Unity project.
2. In your global Post-Process Volume Component, add a Color Grading effect by clicking on Add Effect... > Unity > Color Grading.
3. Change the Mode to External.
4. In the Lookup Texture field, drag and drop a LUT of your choice.

Enjoy!
