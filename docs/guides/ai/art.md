# Making Art with AI

The AI station is set up for AI image generation.

## Running

### InvokeAI

InvokeAI is a user-friendly UI geared towards artists, and provides the usual image generation tools as well as an editing canvas.

There is an `invokeai-web` shortcut on the taskbar that can be used to start InvokeAI. From here you should navigate to http://192.168.42.118:9090 in the browser to load the UI.

InvokeAI also has a workflow tab that provides a more advanced node-based interface.

### ComfyUI

ComfyUI is also available for more advanced uses. This is a node-based tool that you can use to build in-depth image generation and processing pipelines.

Look in the start menu for **Stability Matrix**, you can run ComfyUI from within this interface, which should launch the browser window for you as well. You may have to close the InvokeAI terminal window first if this is running.

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
- *Denoising Strength*: When using image-to-image, this controls how much of the original image is preserved, with lower values preserving the input more, and higher values leading to more change.
