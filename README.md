# DA1LiangBarskyLineClippingAlgorithm
This is Liang Barsky algorithm Tutorial video whose code is there in Github.  Its work is to clip the line using Parametric equation  and can be used to extend line clipping in 3D space.(Sorry Forgot to mention in the video) As it is very versatile in nature it finds in utility everywhere including the PIL library used in the code which uses the algorithm for drawing line inside our specified window.

# Link To Youtube Video :https://youtu.be/aXjq2Jov1E8

1.Set tmin=0, tmax=1.
#
2.Calculate the values of t (t(left), t(right), t(top), t(bottom)),
#
  (i) If t < tmin ignore that and move to the next edge.
#  
  (ii) else separate the t values as entering or exiting values using the inner product.
#
(iii) If t is entering value, set tmin = t; if t is existing value, set tmax = t.
#
3.If tmin < tmax, draw a line from (x1 + tmin(Δx), y1 + tmin(Δy)) to (x1 + tmax(Δx), y1 + tmax(Δy))
#
4.If the line crosses over the window, (x1 + tmin(Δx), y1 + tmin(Δy)) and (x1 + tmax(Δx), y1 + tmax(Δy)) are the intersection   point of     line and edge.
