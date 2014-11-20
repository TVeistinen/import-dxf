# Modifications
* I  modified the ULP for my needs. I ran into the problem that you cannot convert lines and arcs into polygons with this ULP though it is possible to use them in EAGLE.
* The modifications are in two parts, first the arcs are created now in wires rather than arcs. This enables easier debugging of polygons that are created using arcs.
* I added a check box for using lines and arcs for polygon creation. When the box is checked lines and arcs are combined to create polygons.
* LWpolyline now works as it is meant in DXF format

## Instructions

#### Creating the DXF
* Design your DXF file using for example AutoCad
* EAGLE does not support arcs in polygons, which have the radius centerpoint on the positive side. 
	* To fix this: break the arc into two pieces. 
* Join your design into one polyline
* Use the software as usual

#### Other notes
* At this time the "lines and arcs to polygon" function only supports one continuous line and arc combination at a conversion
  * A demo file for this is in the repo
* "Lines and arcs to polygon" function is pretty useless now when LWpolyline works properly.

