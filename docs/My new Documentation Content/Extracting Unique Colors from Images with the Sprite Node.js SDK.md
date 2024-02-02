
  
   # **getUniqueColors**

## High Level

The `getUniqueColors` function is a method exported from the `sprite` Node.js SDK. It can be used to extract all the unique colors from an image. This can be useful for a variety of purposes, such as creating a color palette for an image or identifying the most prominent colors in an image.

## Why should I use this function?

The `getUniqueColors` function can be useful for a variety of purposes, including:

* Creating a color palette for an image.
* Identifying the most prominent colors in an image.
* Generating a histogram of the colors in an image.
* Comparing the colors of two or more images.

## What are the parameters or arguments required?

The `getUniqueColors` function takes a single parameter:

* `imagePath`: The path to the image file.

## Prerequisites

Before using the `getUniqueColors` function, you must first install the `sprite` Node.js SDK. You can do this by running the following command:

```
npm install sprite
```

## How do I use this function?

To use the `getUniqueColors` function, simply import it from the `sprite` module and then call it with the path to the image file. The function will return an array of unique colors from the image.

Here is an example of how to use the `getUniqueColors` function:

```
const sprite = require('sprite');

const imagePath = '/path/to/image.jpg';

const uniqueColors = sprite.getUniqueColors(imagePath);

console.log(uniqueColors);
```

The output of the above code will be an array of unique colors from the image. Each color will be represented as a hexadecimal string.

## Conclusion

The `getUniqueColors` function is a powerful tool that can be used for a variety of purposes. It is easy to use and can be integrated into your existing projects with ease.
  
  