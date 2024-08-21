# Making Art with AI

The AI station is set up for AI image generation.

TODO write this while at the Hacklab...

## Running

For beginners, run InvokeAI. This is a straightforward UI geared towards artists, while hiding away some of the more advanced options.

For more advanced usages, locate ComfyUI. This is a node-based tool that you can use to build advanced image generation and processing pipelines.

## Common Parameters

- *CFG*: Controls how much the text prompt affects the image.  Its
  effect will depend on the model, but generally lower values (**1 -
  4.5**) will provide a bit more "chaos" in the image usually with some
  desaturation, and higher values (**6.5 - 10**) will increase the
  saturation but may lead to "overcooking".
  
- *Resolution*: Many models are trained using images with around
  **1024x1024** pixels, with varying ratios. E.g. for portrait you may
  use **768x1280**, or the opposite for landscape.  Other resolutions
  may work, but higher resolutions increase the chances of duplicate
  objects, and increase VRAM usage and decrease speed.
