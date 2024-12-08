
# Padding and Strides in CNN

## Padding
Padding refers to adding extra layers of zeros around the input image. It is done for several reasons:
1. **Maintain the size**: Without padding, the size of the image reduces after every convolution. Padding helps preserve the original dimensions.
2. **Focus on edge features**: It allows the convolutional filter to better capture features at the edges of the image.

### Types of Padding
- **Valid Padding (No Padding)**: No extra pixels are added, which causes the output size to shrink.
- **Same Padding**: Zeros are added so that the output size remains the same as the input size.

## Strides
Stride refers to how the filter moves across the image:
1. **Stride of 1**: The filter moves one pixel at a time, resulting in a detailed analysis of the input.
2. **Stride of 2 or more**: The filter skips pixels as it moves, reducing the output size and computational cost.

## Example
- **Padding**: If you have a 3x3 filter and a 5x5 image, without padding, the filter can only scan the central 3x3 area, reducing the effective image size. With padding, you can keep the full area in scope.
- **Strides**: If the stride is 2, the filter jumps 2 pixels instead of 1, effectively scanning fewer parts of the image.

