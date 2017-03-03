# Geodesic-Distance-on-a-color-image
Find minimal Geodesic distance on an image (Im) between point x0,y0   and all other points in  the color image
%Find minimal Geodesic distance on an image (Im) between point x0,y0  
%and all other points in  the image 
%return distance map (DistMaP) as a 2d matrix in the size of the original image were
%the value in each element is the Geodesic distance of this pixel from coordinate x0,y0
%Use the image as topological map with color as height and use the
%Dijkstra's algorithm to find minimal geodesic distance to each point

%Input:

%Im color image (or other multichannel image) 

%x0,y0 coordinates (on the image) of the origin from the Geodesic distance
% The value of all points on the returned matrix (DistMap) will be their distance from x0,y0

%NumSteps optional parameter that allow  you to limit the number of cycle of the calculation this may result faster but less accurate calculation

%WeightDist the distance component have two parts distance travel on
%the image plane and distance in the color/grayscale value this parameter
%control the relative weight of the distance on the image plane  

%Output:
%DistMap a map of geodesic distance to coordinate x0,y0 

%Method:
%Use  the image as topological map and use the Dijkstra's algorithm to find geodesic distance to all points
