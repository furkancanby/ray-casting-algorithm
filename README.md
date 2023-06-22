# ray-casting-algorithm

Ray casting is a technique used in computer graphics and computational geometry to determine whether a point is inside a polygon or to calculate the intersection of a ray with objects in a scene. It works by tracing a ray from an origin point in a specific direction and checking for intersections with objects or boundaries in the scene.

The basic idea behind the ray casting algorithm is to count the number of times a ray intersects the edges of a polygon. If the number of intersections is odd, the point is considered inside the polygon. If the number of intersections is even, the point is outside the polygon.

## Legend

**xp,yp** = x and y-axis of our arbitrary point

**x1,y1** first x and y-axis of the sequential point in the polygon path

**x2,y2:** second x and y-axis of the sequential point in the polygon path

> **First condition:** (yp < y1) != (yp < y2)

> **Second condition:** xp < ( x1 + (x2-x1)*(yp - y1)/(y2-y1) )
