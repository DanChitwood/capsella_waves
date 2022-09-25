# *Capsella* waves
*a function that continuously models leaf lobes across the leaf*

# The `model_leaf` function

**A function `model_leaf` that takes inputs of:**

1. leaf trace coordinates
2. landmark coordinates
3. number of points to interpolate for the trace
4. number of landmarks (interpolated points within each lobe)
5. polynomial degree to model each landmark across leaf lobes
6. frames (or x values) to model across the leaf, apportioned to intervals between lobes by rounding

**The function returns:**

1. overall modeled x and y values. for both x and y values, this is a double list of lists structured first by frame, and the for each frame, modeled values for each landmark
2. interpolated trace lists for plotting
3. landmark lists that have been aligned to the trace (for plotting)

**Data for modeling four different *Capsella* leaves is from Figure 1A of:**

Iannetta PP, Begg G, Hawes C, Young M, Russell J, Squire GR. **Variation in Capsella (shepherd’s purse): an example of intraspecific functional diversity.** *Physiologia Plantarum*. 2007 Mar;129(3):542-54. [doi](https://doi.org/10.1111/j.1399-3054.2006.00833.x)

Code to visualize results and create an animated gif by frame is included at the end of the Jupyter notebook
