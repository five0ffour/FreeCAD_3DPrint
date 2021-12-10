# 3D Printing Projects - Example 9
  
## Approach
Used Part Design to create an involute gear but couldn't get the involute gear to work as it seems to assume bevel gears.   
Next I googled and found a square tooth gear macro on github that someone created using arrays. It looks like it can do the job if I do my math correctly.  It never worked out  
Ulimtately I researcehd how to manually compute gears, pitch and modules.  That gave me enough insight to reason out the manual approach    
- Create the three reference circles  
- Create bisecting guidelines that sliced 22.5 degrees around the center vertex (360/16 teeth) gives you the center of each tooth  
- Create a 10mm horizontal line perpendicular to that vertex  
- Drop two parallel lines to that vertex from each side of the tooth to the inner reference line  
- Trim out the execess lines once the tooth is fixed
- Lather, rinse, repeaat 15 more times working around the axis    

## First principles skills I picked up  
Involute gear   
Macros  
Arrays  

## Overall impression  
A tough one in FreeCAD. The involute gear feature doesn't seem to support square teeth. I needed to do it manually.

## Alternate approaches
Found a script included in the FreeCAD install for radial copies. I suspect there is a way to automate these boxes with arrays.

## File References
This notes file: README-ex09.md  
FreeCAD project file: Cardin360-ex09.FCStd  
Requirements book view: Cardin360-ex09.png  
FreeCAD project rendered output: Result-ex09.png  
  
## Built With
FreeCAD 0.19 - FreeCAD (https://www.freecad.org/downloads.php)   
  
## Author
Michael Galarneau - Five0ffour  
Last update: December 10, 2021  
    
## Output   
![EX-09](Result-ex09.png)  