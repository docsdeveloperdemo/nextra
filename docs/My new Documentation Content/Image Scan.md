
  
   # **Image Scan**

High Level

The `image.scan()` method is used to iterate over each pixel in an image and perform a specific action on each pixel. This method is useful for tasks such as image processing, color correction, and image manipulation.

## Why should I use this function?

The `image.scan()` method is a powerful tool for manipulating images. It allows you to perform a variety of operations on each pixel in an image, giving you complete control over the image's appearance.

## What are the parameters or arguments required?

The `image.scan()` method takes the following parameters:

* `x`: The starting x-coordinate of the scan.
* `y`: The starting y-coordinate of the scan.
* `width`: The width of the area to be scanned.
* `height`: The height of the area to be scanned.
* `callback`: A function that will be called for each pixel in the scanned area. The function will be passed the following arguments:
    * `x`: The x-coordinate of the current pixel.
    * `y`: The y-coordinate of the current pixel.
    * `idx`: The index of the current pixel in the image's data array.

## Prerequisites

Before using the `image.scan()` method, you must first import the `Jimp` library. You can do this by adding the following line to your code:

```
import Jimp from "jimp";
```

## How do I use this function?

The following code shows you how to use the `image.scan()` method to make all of the pixels in an image transparent:

```
const image = new Jimp(200, 200, 0xFFFFFFFF);

image.scan(0, 0, image.bitmap.width, image.bitmap.height, function (x, y, idx) {
  this.bitmap.data[idx + 3] = 0; // Set alpha to 0 (transparent)
});

image.write("transparent.png");
```

This code will create a new image that is 200 pixels wide and 200 pixels high. All of the pixels in the image will be transparent. The image will be saved to a file named "transparent.png".

## Conclusion

The `image.scan()` method is a powerful tool for manipulating images. It allows you to perform a variety of operations on each pixel in an image, giving you complete control over the image's appearance.
  
  