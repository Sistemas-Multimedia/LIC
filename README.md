# RIC (Reversible (lossless) Image Compression)

RIC is an image compressor that conserves the information of the image. It exploits the spatial and color redundancy using reversible transforms and entropy coding.

## Color transform
Currently, RIC finds the most suitable color transform between:

1. Integer YCrCb (luminance/red-chroma/blue-chroma) transform.
2. Integer color-DCT (Discrete Cosine Transform).
3. YCoCg (luminance/orange-chroma/green-chorma) transform.
4. None.

## Spatial transform
In each color channel, currently RIC searches between:

1. 2D DPCM (Differential Pulse Code Modulation).
2. Variable blocks-size integer DCT.
3. Integer dyadic-DWT (Discrete Wavelet Transform).
4. Integer packet-DWT.
5. None.

## Entropy coding

RIC checks:

1. Huffman.
2. Arithmetic coding.
3. DEFLATE.
4. Optimized PNG.
5. Lossless JPEG2000.
6. Lossless BGP.
