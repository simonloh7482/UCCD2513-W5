# UCCD2513-W5
 UCCD2513 T14 Week 5 Activity

1. Convert the code chunk found under section Divide an image into smaller patches using cropping into a function with the following signature:
 ```
 crop_grid(img, num_horizontal_grid, num_vertical_grid, line_color)
 # img is the source image
 # num_horizontal_grid and num_vertical_grid are the number of patches along x and y axes.
 # line_color is the color of the grid line.
 # The output of the function should be image with grids
 ```

2. Display image sequences of smooth transition of two images with different values of α. Refer to code in section "Image blending". Use "lena.jfif" and "coins.jfif" as the base images.

3. Rotate image by 45 degrees without cropping the sides of the image. (Hint: There are 2 strategies to tackle these problems). Use "lena.jfif" as the input image.
 - Use external libraries imutils.
 - Modify the transformation matrix.

4. Use the images with titles: "flower.jfif" and "native-bee.png". I want to put flower above an image. If I add two images, it will change color. If I blend it, I get a transparent effect. But I want it to be opaque. If it was a rectangular region, we could use the ROI as we did in the previous section. But flower is not a rectangular region. This is where bitwise operations, like AND, OR, NOT and XOR really come in handy. The associated functions are `cv.bitwise_and()`, `cv.bitwise_or()` and `cv.bitwise_not()`. You need to use `cv.threshold` function to segment the flower. Please refer to ![online documentation](https://docs.opencv.org/4.x/d2/de8/group__core__array.html#ga60b4d04b251ba5eb1392c34425497e14) for more info. The result should resemble the following:
 ![activity3](https://user-images.githubusercontent.com/70535150/179164088-35d7ee40-dba3-497a-98eb-98d19e229f4f.PNG)
