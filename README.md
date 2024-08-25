Using a microscope without a scalebar, a number of images of zotefoam were taken. 

![image](https://github.com/user-attachments/assets/b6ad8666-e953-48c8-990f-88890e4ff891)

Due to the lack of a scalebar, a novel (shitty) image calibration technique has been used. For each object to be imaged, 
the scalebar is extracted by taking four images: an origin, objective moved 100 microns to the right of the origin, objective
moved 100 microns down from the origin, and objective moved both 100 microns to the right and down from the origin.

By sliding pairs of images past each other a pixel at a time (ie: origin + right_shift), a set of residuals can be generated and
minimized to obtain the number of pixels corresponding to the size of the scalebar.

The rest of the code focuses on applying (unsuccessfully) a grab bag of techniques to attempt to detect edge pixels and interior pixels and use this
to binarize the image. 
