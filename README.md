# Modifications
* I  modified the ULP for my needs. I ran into the problem that you cannot convert lines and arcs into polygons with this ULP though it is possible to use them in EAGLE.
* The modifications are in two parts, first the arcs are created now in wires rather than arcs. This enables easier debugging of polygons that are created using arcs.
* I added a check box for using lines and arcs for polygon creation. When the box is checked lines and arcs are combined to create polygons.

## Instructions

#### Creating the DXF
* Design your DXF file using for example AutoCad
* Use only arcs and lines that run continuously
* If the order in the DXF for the lines and arcs are mismatched, then the output will not be desired
* Usually creating a single polyline and exploding it helps to get them in the right order
* If this does not work:
	* Uncheck the "Lines and Arcs to Polygon" check box
	* Run the program
	* Copy the output script to a text editor
	* Manually reorder the lines and arcs so that the last point on the first line or arc matches the first point of the second
	* After all the points are in order delete the first point from all entries except the first one
	* Delete the semicolons from all entries except the last
	* Rename "Wire" to "Polygon"
	* Run the script normally

#### Other notes
* At this time the mod only supports one continuous line and arc combination at a conversion
* A demo file is in the repo

