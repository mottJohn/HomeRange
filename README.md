# What is Home Rrange Analysis
A home range is the area in which an animal lives and moves on a periodic basis. It is related to the concept of an animal's territory which is the area that is actively defended. 

There are a few methods for estimating home range, such as [Maxmium Convex Polgyon (MCP)](https://en.wikipedia.org/wiki/Convex_polygon), and [Kernel Density Estimate](https://en.wikipedia.org/wiki/Kernel_density_estimation).

# What is Kernel Density Estimate
For a detail explanation on Kernel Density Estimate, I recommend you to visit this [wiki](https://en.wikipedia.org/wiki/Kernel_density_estimation), and watch this [YouTube video](https://www.youtube.com/watch?v=x5zLaWT5KPs).

In a nutshell, the Kernel Density Estimate is computed by following steps:

1. Compute the spatial distribution of points(sighting)
2. Assign the distribution to each points (With the integral of such distribution equals 1)
3. Sum all the distributions and divide by the total number of points (such that the integral of the sum equals 1)

To get the Utilization Distribution, further normalised the distributions by dividing it by the maximum density, i,e, z = z/z_max * 100. The 95% home range is therefore represented by z >= 5. Similarly, the 50%, 25% home range is represented by z >= 50 , and z >= 75 respectively.

# Tools for Conducting Kernel Density Estimate
## Opensource
[Animove](https://www.faunalia.eu/en/animove.html#animove-for-qgis), and QGIS version 2.X (Version 3 will not work).

Installation is a bit tricky. Please follow [this instructions](https://gitlab.com/faunalia/sextante_animove/blob/master/doc/installation_win.rst).

### How to use animove to conduct Home Range Analysis
1. Please watch this [YouTube video first](https://www.youtube.com/watch?v=98ORgGX8vSM).
2. The output files are polyline (contours), and raster (heatmap). The contours are actually generated from the raster.
3. The value of raster is the normalized density ranges from 0 to 100.
4. The contour line is incremented by 10. The inner contour represents the 10% home range. The outer contour represents the 90% home range.
5. Change the symbols of the raster layer to display the home range of 25%, 50%, and 95%

## License Software
[Geospatial Modelling Environment](http://www.spatialecology.com/gme/), and ArcMap (The tool is opensource, but it is such a pretty that ArcMap should be used together)

