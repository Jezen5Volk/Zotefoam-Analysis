Using a microscope without a scalebar, a number of images of zotefoam were taken. 
![image](https://github.com/user-attachments/assets/12d8d6b1-2693-4220-8d39-9d2a18ff0dcd)

Due to the lack of a scalebar, a novel (shitty) image calibration technique has been used. For each object to be imaged, 
the scalebar is extracted by taking four images: an origin, objective moved 100 microns to the right of the origin, objective
moved 100 microns down from the origin, and objective moved both 100 microns to the right and down from the origin.

By sliding pairs of images past each other a pixel at a time (ie: origin + right_shift), a set of residuals can be generated and
minimized to obtain the number of pixels corresponding to the size of the scalebar.

The rest of the code focuses on edge detection to extract cell boundaries and cell area in order to estimate the size of the average cell.
