
  
   # **removeBackgroundColor**

High Level

The `removeBackgroundColor` function is a powerful tool that allows you to easily remove the background from an image. This can be useful for a variety of purposes, such as creating product images, removing unwanted objects from photos, or simply changing the background of an image.

This function is exported from our Node.js SDK, which you can install from NPM. To use it, simply import the `sprite` object and call the `removeBackgroundColor` function.

```
import { sprite } from sprite

sprite.removeBackgroundColor(inputPath, outputPath, targetColor, colorThreshold)
```

## Why should I use this function?

The `removeBackgroundColor` function can be used for a variety of purposes, including:

* Creating product images: By removing the background from product images, you can create a more professional and polished look.
* Removing unwanted objects from photos: If there is an unwanted object in a photo, you can use the `removeBackgroundColor` function to remove it.
* Changing the background of an image: You can use the `removeBackgroundColor` function to change the background of an image to anything you want.

## What are the parameters or arguments required?

The `removeBackgroundColor` function requires the following parameters:

* `inputPath`: The path to the input image.
* `outputPath`: The path to the output image.
* `targetColor`: The color you want to remove from the background.
* `colorThreshold` (optional): The maximum color difference between the target color and the pixels in the image.

## Prerequisites

Before using the `removeBackgroundColor` function, you must have the following installed:

* Node.js
* The sprite Node.js SDK

## How do I use this function?

To use the `removeBackgroundColor` function, simply follow these steps:

1. Import the `sprite` object from the sprite Node.js SDK.
2. Call the `removeBackgroundColor` function, specifying the input path, output path, target color, and color threshold (optional).
3. The function will remove the background from the input image and save the output image to the specified output path.

Here is an example of how to use the `removeBackgroundColor` function:

```
const sprite = require('sprite')

sprite.removeBackgroundColor('input.jpg', 'output.jpg', '#FFFFFF')
```

This will remove the white background from the input image and save the output image to the output path.

## Conclusion

The `removeBackgroundColor` function is a powerful tool that can be used for a variety of purposes. By following the steps outlined in this document, you can easily use this function to remove the background from images and create professional-looking results.
  
  