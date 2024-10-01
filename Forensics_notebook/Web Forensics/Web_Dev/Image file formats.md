There are many file types and another of my notes goes more in depth with some of them. This will be focused on image file formats and why they are used or not because of what they do or how they work. 

Some initial concepts to get familiar with are the following:
- raster graphics
- vector graphics
- lossy compression
- lossless compression
- color spaces
- bit depth
- alpha channels

Raster graphics is a method of making an image file using a grid of pixels (which is referred to as a bitmap). This has a set limitation of pixels so when you zoom in or scale up the image, the pixels forming the grid (bitmap) appear.

- Raster is great for images that have a defined size and do not need more scaling or zooming than necessary. They have the advantage of storing with less bits so their file size tends to be smaller.

Vector graphics uses geometric formulas to create a file and therefore, bypasses the pixel limitation of raster graphics. This means that when you zoom in or scale up, there is almost no loss to the sharpness (clarity) of an image.

- Vector is great for logos or any other media that needs more frequent sizing work done on it so their is no loss in clarity of the image. 

Lossy vs Lossless

Most raster formats (almost universally all) apply compression to make the file size more compact so that it is easier to send and receive it. A lossy compression achieves this by actually discarding data, deleting some 0's and 1's on the image which reduces its quality/sharpness/clarity. It uses what is called [[Discrete Cosine Transform]] (DCT) -this approximates the content of an image using trigonometric functions. 

Non-lossy compression reduces file size but retains all the bits by using run-length encoding (RLE) -this stores information of each bit and identifies if some have an identical value, it stores these sequences of identical bytes as a single value followed by a count on how many identical there are.

Color Channels:
There are a few ways that images store data which include RGB, CYMK, greyscale, BGR, HSV, RYB, LAB, and HSL. These are essentially just color combinations to get specific tones, shades, and colors. There are specific purposes for them or application. For example, in printing, CYMK is the standard because it allows for an image to be separated into cyan, yellow, magenta, and black. Other areas where they are used include research since sensing and computer vision require understanding of the visible spectrum and some invisible such as infrared. 

Here are a couple of educative resources:
[75 Years of Innovation: Color television | by SRI International | The Dish | Medium](https://medium.com/dish/75-years-of-innovation-color-television-3991507bb0d1)

This one I really enjoy because I love astronomy:
[How Are Webb’s Full-Color Images Made? | Webb (webbtelescope.org)](https://webbtelescope.org/contents/articles/how-are-webbs-full-color-images-made)

This one is extremely helpful and uses Python to help make sense of what is under the hood:
[Understanding the concept of Channels in an Image | by Maximinusjoshus | featurepreneur | Medium](https://medium.com/featurepreneur/understanding-the-concept-of-channels-in-an-image-6d59d4dafaa9)
