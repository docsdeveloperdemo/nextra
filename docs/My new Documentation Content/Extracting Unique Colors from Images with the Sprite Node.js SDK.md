
  
   # **getUniqueColors**

## High Level

The `getUniqueColors` function is a method that is exported from the `sprite` Node.js SDK. It can be used to extract all of the unique colors from an image. This can be useful for a variety of purposes, such as creating a color palette for an image or identifying the most prominent colors in an image.

## Why should I use this function?

The `getUniqueColors` function can be useful for a variety of purposes, including:

* Creating a color palette for an image.
* Identifying the most prominent colors in an image.
* Generating a histogram of the colors in an image.
* Comparing the colors of two or more images.

## What are the parameters or arguments required?

The `getUniqueColors` function takes a single parameter, which is the path to the image file that you want to analyze.

## Prerequisites

In order to use the `getUniqueColors` function, you will need to have the following installed:

* Node.js
* The `sprite` Node.js SDK

## How do I use this function?

To use the `getUniqueColors` function, you can follow these steps:

1. Import the `sprite` Node.js SDK into your project.
2. Call the `getUniqueColors` function, passing in the path to the image file that you want to analyze.
3. The function will return an array of unique colors that were found in the image.

Here is an example of how to use the `getUniqueColors` function:

```javascript
const sprite = require('sprite');

const imagePath = '/path/to/image.png';

const uniqueColors = sprite.getUniqueColors(imagePath);

console.log(uniqueColors);
```

The output of the above code will be an array of unique colors that were found in the image. Each color will be represented as a hexadecimal string.

## Conclusion

The `getUniqueColors` function is a powerful tool that can be used to extract all of the unique colors from an image. This can be useful for a variety of purposes, such as creating a color palette for an image or identifying the most prominent colors in an image.
  
  