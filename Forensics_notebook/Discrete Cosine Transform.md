[Discrete Cosine Transform Explained | Papers With Code](https://cs.paperswithcode.com/method/discrete-cosine-transform)

Use that website for more than just DCT, it is really useful.

This website tends to be less intense in their jargon and less academic so it is helpful to get a high-level understanding:
[Discrete Cosine Transform (Algorithm and Program) - GeeksforGeeks](https://www.geeksforgeeks.org/discrete-cosine-transform-algorithm-program/)

This is a very math oriented:
[3.8.2: Discrete Cosine Transformation - Engineering LibreTexts](https://eng.libretexts.org/Bookshelves/Electrical_Engineering/Signal_Processing_and_Modeling/Information_and_Entropy_(Penfield)/03%3A_Compression/3.08%3A_Detail-_2-D_Discrete_Cosine_Transformation/3.8.02%3A_Discrete_Cosine_Transformation)

For the sake of simplicity, I have not gone into explaining geometry to explain what cosine is but refer to texts or youtube for a better understanding of Pythagoras theorem.

The essential take away is that it is used in lossy image compression and reduces the size without a significant loss in quality. This is done by transforming the image into a new representation using matrices that are more efficient when storing and transferring as bits.

The equation works as follows:

$$
dct[i][j] = ci * cj (sum(k=0 to m-1) sum(l=0 to n-1) matrix[k][l] * cos((2*k+1) *i*pi/2*m) * cos((2*l+1) *j*pi/2*n)
$$
That is extremely complex looking but what it does should be made simpler to understand.

An image file, which is again, a composition of bits that represent color. For simplicity, use black and white examples. Only two "colors" are used to encode an image file so the amount of data is smaller, (i.e. there's less bits to represent). 

The second step, which is the first in the compression process is to divide an image into small 'blocks' of pixels. Each block of pixels is typically 8x8 pixels. Since a byte can be represented as a number from 0-255, a single block can be a large number. and each number is represented as 0's and 1's. 

These blocks are then operated on (the math is applied), by multiplying the pixel values by a set of cosine functions. Once the operation is completed, the image data transitions from a spatial "domain" of pixel values, to a frequency "domain" of coefficient representing different frequencies). 

The reason why things are simpler as frequencies is thanks to the fact that information is just an electrical signal/pulse (electrons moving). A binary is just electricity on or off (1 or 0).  This is covered in more detail and explained simply in another note; [[Binary]] and [[Capturing Lightning]]. 

The next step in DCT is to 'quantize'. This is the primary step in actually reducing the image file size since the previous steps were more meant to prepare the file for this process. Since the image is now in a frequency domain (coefficients representing different frequencies), it is ready to be quantized. A matrix is used to determine how much to reduce each coefficient. Coefficients representing low frequencies (important for overall image structure) are typically kept with higher precision, while coefficients representing high frequencies (fine details) can be reduced more.

The next step is to group the coefficients of similar frequency characteristics together. Those coefficient numbers closer to 0 get grouped together and those close to 1 get grouped together. This process is called zigzag scanning. 

After this, RLE or run-length encoding used  to reduce the amount of data needed to represent the image by storing the number of consecutive zero coefficients followed by the non-zero value. 

In order to further compress the data, entropy encoding assigns shorter codes to frequently occurring signs (zero coefficients) and longer codes to less frequent signs. 

When an image is to be displayed and seen again, it goes through the process of IDCT or inverse discrete cosine transform. This step decodes Huffman encoding, RLE is used to reconstruct the quantized coefficients, and IDCT is done to convert the coefficients back into pixel values. 

The last step reassembles the image by reconstructing blocks to form the final decompressed image.

**This entire process is used to make file size smaller when it is transported, going from one device to another.** 

**Frequency** in the context of DCT refers to how quickly the image's intensity changes. High-frequency components represent rapid changes, like sharp edges or fine details. Low-frequency components represent gradual changes, like large areas of similar color.
### A simplified explanation follows:

1. Divide and Conquer:
 - Cut the image into 8x8 pixel blocks
 
2. Frequency Magic:  
 - Turn pixel values into frequency numbers, higher numbers mean important details.
