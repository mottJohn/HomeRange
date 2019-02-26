# What is Home Rrange Analysis
A home range is the area in which an animal lives and moves on a periodic basis. It is related to the concept of an animal's territory which is the area that is actively defended. 

There are a few methods for estimating home range, such as [Maxmium Convex Polgyon (MCP)](https://en.wikipedia.org/wiki/Convex_polygon), and [Kernel Density Estimate](https://en.wikipedia.org/wiki/Kernel_density_estimation).

# What is Kernel Density Estimate
For a detail explanation on Kernel Density Estimate, I recommend you to visit this [wiki](https://en.wikipedia.org/wiki/Kernel_density_estimation), and watch this [YouTube video](https://www.youtube.com/watch?v=x5zLaWT5KPs).

In a nutshell, the Kernel Density Estimate is computed by following steps:

1. Compute the spatial distribution of points(sighting)
2. Assign the distribution to each points (With the integral of such distribution equals 1)
3. Sum all the distributions and divide by the total number of points (such that the integral of the sum equals 1)

To get the Utilization Distribution, further normalised the distributions by dividing it by the maximum density, i,e, $z = \frac{z}{z_max} * 100$. The 95% home range is therefore represented by $z \ge 5$. Similarly, the 50%, 25% home range is represented by $z \ge 50$, and $z \ge 75%$ respectively.

# Tools for Conducting Kernel Density Estimate
## Opensource

## License Software
