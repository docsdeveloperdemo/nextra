
  
   # **Remove Background Color**

High Level

The `removeBackgroundColor` function is a method that is exported from the `sprite` Node.js SDK. It allows you to remove the background color of an image. This can be useful for creating transparent images or for removing unwanted backgrounds from images.

## Why should I use this function?

The `removeBackgroundColor` function can be used for a variety of purposes, including:

* Creating transparent images: You can use the `removeBackgroundColor` function to create transparent images by removing the background color of an image. This can be useful for creating logos, icons, and other graphics that need to be placed on a variety of backgrounds.
* Removing unwanted backgrounds: You can use the `removeBackgroundColor` function to remove unwanted backgrounds from images. This can be useful for improving the appearance of images or for making them easier to edit.

## What are the parameters or arguments required?

The `removeBackgroundColor` function takes the following parameters:

* `inputPath`: The path to the input image.
* `outputPath`: The path to the output image.
* `targetColor`: The color you want to remove from the background of the image.
* `colorThreshold` (optional): The maximum color difference between the target color and the pixels in the image that will be made transparent. The default value is 0.

## Prerequisites

Before you can use the `removeBackgroundColor` function, you must install the `sprite` Node.js SDK. You can do this by running the following command:

```
npm install sprite
```

## How do I use this function?

To use the `removeBackgroundColor` function, you can import it from the `sprite` Node.js SDK and then call it with the appropriate parameters. The following code sample shows you how to use the `removeBackgroundColor` function to remove the white background from an image:

```
const sprite = require('sprite');

async function removeBackgroundColor() {
  const inputPath = 'path/to/input.png';
  const outputPath = 'path/to/output.png';
  const targetColor = '#FFFFFF';

  await sprite.removeBackgroundColor(inputPath, outputPath, targetColor);
}

removeBackgroundColor();
```

## Conclusion

The `removeBackgroundColor` function is a powerful tool that can be used to remove the background color of images. This can be useful for creating transparent images or for removing unwanted backgrounds from images.
  
  