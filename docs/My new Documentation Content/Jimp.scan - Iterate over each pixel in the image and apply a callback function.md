
  
   # **Jimp.scan**

High Level

The `scan` method of the `Jimp` class iterates over each pixel in the image and applies a callback function to each pixel. The callback function receives the x and y coordinates of the pixel, as well as the index of the pixel in the image data array.

## Why should I use this function?

The `scan` method can be used to perform a variety of image processing operations, such as:

* Converting an image to grayscale
* Applying a color filter to an image
* Detecting edges in an image
* Resizing an image

## What is params or arguements required?

The `scan` method takes the following parameters:

* `x`: The x-coordinate of the starting pixel.
* `y`: The y-coordinate of the starting pixel.
* `width`: The width of the region to scan.
* `height`: The height of the region to scan.
* `callback`: The callback function to apply to each pixel.

The callback function receives the following parameters:

* `x`: The x-coordinate of the pixel.
* `y`: The y-coordinate of the pixel.
* `idx`: The index of the pixel in the image data array.

## Prequsites

There are no prerequisites for using the `scan` method.

## How do I use this function?

The following code sample shows you how to use the `scan` method to convert an image to grayscale:

```
const image = new Jimp(200, 200);

image.scan(0, 0, image.bitmap.width, image.bitmap.height, function (x, y, idx) {
  const red = this.bitmap.data[idx + 0];
  const green = this.bitmap.data[idx + 1];
  const blue = this.bitmap.data[idx + 2];

  const grayscale = (red + green + blue) / 3;

  this.bitmap.data[idx + 0] = grayscale;
  this.bitmap.data[idx + 1] = grayscale;
  this.bitmap.data[idx + 2] = grayscale;
});

image.write('grayscale.png');
```

The above code sample will create a new image called `grayscale.png` that is a grayscale version of the original image.

## Conclusion

The `scan` method is a powerful tool that can be used to perform a variety of image processing operations. By understanding how to use the `scan` method, you can create custom image processing scripts that can meet your specific needs.
  
  