
  
   # **scan**

High Level

The `scan` method is used to iterate over each pixel in an image and perform a specific operation on each pixel. This method takes a callback function as its first argument, which is called for each pixel in the image. The callback function receives the following arguments:

* `x`: The x-coordinate of the pixel.
* `y`: The y-coordinate of the pixel.
* `idx`: The index of the pixel in the image data array.

The callback function can perform any operation on the pixel, such as changing its color, setting its alpha value, or calculating a value based on the pixel's color.

## Why should I use this function?

The `scan` method is useful for performing operations on large images that would be inefficient to perform on the entire image at once. For example, you could use the `scan` method to:

* Change the color of all pixels in a specific region of an image.
* Set the alpha value of all pixels in an image to 0 (transparent).
* Calculate the average color of an image.

## What is params or arguements required?

The `scan` method takes the following arguments:

* `x`: The x-coordinate of the starting pixel.
* `y`: The y-coordinate of the starting pixel.
* `width`: The width of the region to scan.
* `height`: The height of the region to scan.
* `callback`: A callback function that is called for each pixel in the region.

## Prequsites

Before using the `scan` method, you must first import the `sprite` module into your project. You can do this by adding the following line to your code:

```
import { sprite } from sprite
```

## How do I use this function?

To use the `scan` method, simply call it on an image object and pass in the appropriate arguments. For example, the following code changes the color of all pixels in a 100x100 region of an image to red:

```
const image = new Jimp(200, 200);

image.scan(50, 50, 100, 100, function (x, y, idx) {
  this.bitmap.data[idx + 0] = 255; // Set red to 255
  this.bitmap.data[idx + 1] = 0; // Set green to 0
  this.bitmap.data[idx + 2] = 0; // Set blue to 0
});
```

The `scan` method can also be used to perform more complex operations on images. For example, the following code calculates the average color of an image:

```
const image = new Jimp(200, 200);

let totalRed = 0;
let totalGreen = 0;
let totalBlue = 0;

image.scan(0, 0, image.bitmap.width, image.bitmap.height, function (x, y, idx) {
  totalRed += this.bitmap.data[idx + 0];
  totalGreen += this.bitmap.data[idx + 1];
  totalBlue += this.bitmap.data[idx + 2];
});

const averageRed = totalRed / (image.bitmap.width * image.bitmap.height);
const averageGreen = totalGreen / (image.bitmap.width * image.bitmap.height);
const averageBlue = totalBlue / (image.bitmap.width * image.bitmap.height);

console.log(`Average color: ${averageRed}, ${averageGreen}, ${averageBlue}`);
```
  
  