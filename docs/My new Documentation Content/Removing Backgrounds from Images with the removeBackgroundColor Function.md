
  
   # **removeBackgroundColor**

High Level

The `removeBackgroundColor` function is a powerful tool that allows you to easily remove the background from an image. This can be useful for a variety of purposes, such as creating product images, removing unwanted objects from photos, or simply changing the background of an image.

This function is exported from our Node.js SDK, which you can install from NPM and import from the `sprite` object like below:

```
import { sprite } from sprite
```

## Why should I use this function?

The `removeBackgroundColor` function is a great choice for removing the background from images because it is:

* **Simple to use:** The function only requires a few parameters, and it can be easily integrated into your existing code.
* **Efficient:** The function is optimized for performance, so you can process images quickly and efficiently.
* **Versatile:** The function can be used to remove the background from a variety of image types, including JPEGs, PNGs, and GIFs.

## What are the parameters or arguments required?

The `removeBackgroundColor` function requires the following parameters:

* **inputPath:** The path to the input image.
* **outputPath:** The path to the output image.
* **targetColor:** The color you want to remove from the background.
* **colorThreshold:** (Optional) The maximum color difference between the target color and the pixels in the image.

## Prerequisites

Before you can use the `removeBackgroundColor` function, you will need to:

1. Install the Sprite SDK from NPM.
2. Import the `sprite` object into your code.

## How do I use this function?

To use the `removeBackgroundColor` function, simply call the function and pass in the required parameters. For example, the following code removes the white background from an image and saves the result to a new file:

```
const sprite = require('sprite');

sprite.removeBackgroundColor('input.jpg', 'output.jpg', '#FFFFFF');
```

## Conclusion

The `removeBackgroundColor` function is a powerful tool that can be used to easily remove the background from images. This can be useful for a variety of purposes, such as creating product images, removing unwanted objects from photos, or simply changing the background of an image.
  
  