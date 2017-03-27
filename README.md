# Pharo FastTable improvements

FastTables was integrated into Pharo 5.0 to solve two main problems that old lists’ implementations were facing, first the performance issue, old list’s data source was limited to a couple of hundreds of rows only and second the lack of extensibility since old lists don’t handle complex element morphs very well.

Since their integration, FT and their sub classes have known several improvements allowing them to render multi cells tables, expandable trees and draggable lists but the development is still in its early stage and there are still a lot of work ahead. 

The goals of this proposal are to highlight the needed improvements and extensions to build a better FT family widgets that could fulfill much bigger variety of applications. Those changes will be delivered as incremental way based on their severity and importance.
A detailed roadmap with several milestones that need to be reached during the GSOC period will be delivered.

## Here are some of defined goals/improvements:

*	Finish the missing tests in the Morphic-Widgets-FastTable package.
*	Support cell selection in the FTTableMorph:
The mouse/keyboard event handler needs to propagate the selected cell index.
*“The selection needs to be made cell-aware”
*	Support row editing and reflect the changes to the data source 
Probably define multiple binding methods between the widget and the data source (One way from source, two way, one way from the widget)
*	Support for variable-height/width rows/columns
*	Add a subclass to FT and build a one that’s much suited to replace old lists model used in SPEC widgets.

> Check out the issues for a complete review/discussion over each point 


