
  
   # **scan**

High Level

The `scan` method of the `sprite` class in the `sprite` module iterates over each pixel in the image and applies a callback function to each pixel. The callback function receives the x and y coordinates of the pixel, as well as the index of the pixel in the image data array.

## Why should I use this function?

The `scan` method can be used to perform various image processing operations, such as color replacement, image cropping, and image resizing.

## What is params or arguements required?

The `scan` method takes the following parameters:

* `x`: The x-coordinate of the starting pixel.
* `y`: The y-coordinate of the starting pixel.
* `width`: The width of the region to scan.
* `height`: The height of the region to scan.
* `callback`: The callback function to apply to each pixel.

## Prequsites

Before using the `scan` method, you must first import the `sprite` module into your project. You can do this by adding the following line to your code:

```
import { sprite } from 'sprite';
```

## How do I use this function?

To use the `scan` method, simply call it on the `sprite` object and pass in the appropriate parameters. For example, the following code will replace all red pixels in the image with transparent pixels:

```
sprite.scan(0, 0, sprite.bitmap.width, sprite.bitmap.height, function (x, y, idx) {
  const red = this.bitmap.data[idx + 0];
  const green = this.bitmap.data[idx + 1];
  const blue = this.bitmap.data[idx + 2];
  const currentColor = Jimp.rgbaToInt(red, green, blue, 255);

  // Calculate the color difference
  const colorDiff = Jimp.colorDiff({ r: red, g: green, b: blue }, Jimp.intToRGBA(colorToReplace));

  // If the color difference is less than the threshold, make it transparent
  if (colorDiff <= colorThreshold) {
    this.bitmap.data[idx + 3] = 0; // Set alpha to 0 (transparent)
  }
});
```
  
  