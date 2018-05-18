---
title: Tessellating Polygons
description: Tessellating Polygons
ms.assetid: '3b219af0-96c3-4a83-8a40-bd7966d58398'
keywords: ["OpenGL Utility (GLU),tessellation", "GLU (OpenGL Utility),tessellation", "OpenGL Utility (GLU),simple polygons", "GLU (OpenGL Utility),simple polygons", "simple polygons OpenGL", "OpenGL Utility (GLU),complex polygons", "GLU (OpenGL Utility),complex polygons", "complex polygons OpenGL"]
---

# Tessellating Polygons

OpenGL can directly display only simple convex polygons. A polygon is simple if:

-   The edges intersect only at vertices.
-   There are no duplicate vertices.
-   Exactly two edges meet at any vertex.

To display simple nonconvex polygons or simple polygons containing holes, you must first triangulate the polygons (subdivide them into convex polygons). Such subdivision is called *tessellation*. GLU provides a collection of functions that perform tessellation. Note that the GLU tessellation functions can't handle nonsimple polygons; there is no standard OpenGL method to handle such polygons.

Because tessellation is often required and can be rather tricky, this section describes the GLU tessellation functions in detail. These functions take as input arbitrary simple polygons that might include holes, and they return some combination of triangles, triangle meshes, and triangle fans. If you don't want to deal with meshes or fans, you can specify that the tessellation functions return only triangles. However, mesh and fan information improves performance. The polygon tessellation functions triangulate a concave polygon with one or more contours.

**To use polygon tessellation**

1.  Create a tessellation object with [**gluNewTess**](glunewtess.md).
2.  Use [*gluTessCallBack*](glutess.md) to define callback functions you will use to process the triangles generated by the tessellator.
3.  With [**gluBeginPolygon**](glubeginpolygon.md), [**gluTessVertex**](glutessvertex.md), [**gluNextContour**](glunextcontour.md), and [**gluEndPolygon**](gluendpolygon.md), specify the polygon with holes or the concave polygon to be tessellated.

    When the polygon description is complete, the tessellation facility invokes your callback functions as necessary.

    You can destroy unneeded tessellation objects with [**gluDeleteTess**](gludeletetess.md).

For more information on saving the tessellation data, see [Using Callback Functions](using-callback-functions.md).

 

 



