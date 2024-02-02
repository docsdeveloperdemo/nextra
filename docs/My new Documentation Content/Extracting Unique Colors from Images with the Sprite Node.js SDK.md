
  
   # **getUniqueColors**

High Level

The `getUniqueColors` function is a method exported from the `sprite` Node.js SDK. It can be used to extract all the unique colors from an image. This can be useful for a variety of purposes, such as creating a color palette for an image or identifying the most prominent colors in an image.

## Why should I use this function?

The `getUniqueColors` function can be useful for a variety of purposes, including:

* Creating a color palette for an image.
* Identifying the most prominent colors in an image.
* Generating a histogram of the colors in an image.
* Comparing the colors of two or more images.

## What are the parameters or arguments required?

The `getUniqueColors` function takes a single parameter, which is the path to the image file that you want to analyze.

## Prerequisites

Before you can use the `getUniqueColors` function, you will need to install the `sprite` Node.js SDK. You can do this by running the following command in your terminal:

```
npm install sprite
```

Once the SDK is installed, you can import it into your project by adding the following line to your code:

```
import { sprite } from 'sprite';
```

## How do I use this function?

To use the `getUniqueColors` function, simply call it with the path to the image file that you want to analyze. The function will return an array of all the unique colors in the image.

Here is an example of how to use the `getUniqueColors` function:

```
const colors = sprite.getUniqueColors('/path/to/image.png');

console.log(colors);
```

The output of the above code will be an array of all the unique colors in the image, represented as hexadecimal strings.

## Conclusion

The `getUniqueColors` function is a powerful tool that can be used for a variety of purposes. It is easy to use and can be integrated into your projects with just a few lines of code.
  
  