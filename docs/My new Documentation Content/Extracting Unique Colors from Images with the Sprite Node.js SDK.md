
  
   # **getUniqueColors**

## High Level

The `getUniqueColors` function is a method that is exported from the `sprite` Node.js SDK. It can be used to extract all of the unique colors from an image. This can be useful for a variety of purposes, such as creating a color palette for an image or identifying the most prominent colors in an image.

## Why should I use this function?

The `getUniqueColors` function can be used to:

* Create a color palette for an image.
* Identify the most prominent colors in an image.
* Generate a histogram of the colors in an image.
* Compare the colors in two or more images.

## What are the parameters or arguments required?

The `getUniqueColors` function takes one parameter:

* `imagePath`: The path to the image file.

## Prerequisites

In order to use the `getUniqueColors` function, you must have the following installed:

* Node.js
* The `sprite` Node.js SDK

## How do I use this function?

To use the `getUniqueColors` function, you can follow these steps:

1. Import the `sprite` Node.js SDK into your project.
2. Call the `getUniqueColors` function with the path to the image file as the argument.
3. The function will return an array of the unique colors in the image.

Here is an example of how to use the `getUniqueColors` function:

```javascript
const sprite = require('sprite');

const imagePath = '/path/to/image.png';

const uniqueColors = sprite.getUniqueColors(imagePath);

console.log(uniqueColors);
```

The output of the above code will be an array of the unique colors in the image. Each color will be represented as a hexadecimal string.

## Additional Information

The `getUniqueColors` function can be used to extract colors from any type of image file that is supported by the `Jimp` library. The `Jimp` library supports a wide variety of image file formats, including PNG, JPEG, BMP, and GIF.

The `getUniqueColors` function can also be used to extract colors from a specific region of an image. To do this, you can use the `crop` function to crop the image to the desired region before calling the `getUniqueColors` function.

Here is an example of how to use the `crop` function to extract colors from a specific region of an image:

```javascript
const sprite = require('sprite');

const imagePath = '/path/to/image.png';

const image = await Jimp.read(imagePath);

const croppedImage = image.crop(0, 0, 100, 100);

const uniqueColors = sprite.getUniqueColors(croppedImage);

console.log(uniqueColors);
```

The output of the above code will be an array of the unique colors in the cropped region of the image.
  
  