# RIC (Reversible (lossless) Image Compression)

RIC is an image compressor that conserves the information of the image. It exploits the spatial and color redundancy using reversible transforms and entropy coding.

The basic encoding algorithm is:

1. Compute the YCoCg (luminance/orange-chroma/green-chorma) color transform transform, if the image is RGB. Otherwise, skip this step.
2. Compute the DWT (Discrete Wavelet Transform).
3. Compress the coefficients using Optimized-PNG (Portable Network Graphics).
