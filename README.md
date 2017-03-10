# Star_Cluster_Simulation_Analysis
EDA and statistical analysis of a globular cluster

Globular clusters are collections of hundreds of thousands of stars that are tightly bound by gravity which gives them their spherical shapes.

There are about 158 globular clusters in the Milky Way, while giant elliptical galaxies like M87 may have as many as 13,000 globular clusters.

These Clusters normally consist of Population II stars, which have a low proportion of elements other than hydrogen and helium. This is an indication of their old age.

Why would anyone want to study simulations?
  Astronomy is an observational science so often we are not able to observe and collect all the information we want. The      simulations allow us to use collected data to extract or derive new features that we are interested in.
  
I got the idea to read all of my files from the Data Star Cluster kernel on kaggle.
Since the data files have similar names that vary only by an integer I can read and append 
them using a for loop with a 'step'. This step incriments the name for the file to be read.
To each data file I add a time column to distinguish the data based on time. Also a radius magnitude, 
speed, and kinetic energy column in order to have more features to analyze. 

I plot the different projections of the stars positions durint t = 0, and t = 1800 in order to see if the cluster
has spherical symmetry.

Then I use plotly to plot a sample of the stars from the cluster at t = 0 and t = 1800 in 3-D to get a 
a visiual comparison of their positions.

Next I look at the distribution of the velocity and the radius of the stars during the first snapshot and the last one and find the best fitting distribution. Normal for the velocity, and lognormal for the radius.

I also set out to see if I can find a reason why these stars have escaped.. maybe they continuously got further and further from the center of the cluster, or maybe due to their interactions with other stars their velocities reached peak velocity and they where flung out of the cluster.

Lastly I calculate the velocity dispersion and from it the effective radius. This result of course comes with a lot of error due to the fact that our data set is unit-less.
