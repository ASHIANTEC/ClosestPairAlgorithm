# ClosestPairAlgorithm
1.To find the middle point in the orrted array ,use p[n/2].
2.Divide the middle array in two halves.The first subarray contains the points from p[0] to p[n/2]
  The second subarray contains points from p[n/2+1] to p[n-1].
3.Recursively find the samllest distances in both subarrays.
  let the distances be dl and dr.
4.Sort the array strip[] according to y coordinates.
  It cn be optimized to O(n) by recursively sorting and merging.
5.Find the smallest distance in strip[].
   
Program:

1.creating a class to represent a point in 2D plane.
2.Create a utility function to find the distance between two points.
3.And use a Bruteforce function to return the smallest distance between two points
  in p[] of size.
4.Initialize the minimum distance as d.
5.Pick all points one by one and try the next points till the difference
  between y coordinates is smaller than d.
6.Create a recursive function to find the smallest distance.
7.Find the middle point.  
8.The smallest distance dl on left of middle point and dr on right middle point.
9.Find the smaller of two distances.
10.And Build an array strip[] that contains points close to the line passing through the middle point.
11.Find the closest points in strip.Return the minimum of  d and closest distance is strip[].
12.The main function finds the smallest distances.this method used closesutil()
13.Use recursive function ClosestUtil() to find the smallest distances
