Issue centring hypherlink text on Widnows
=========================================

This is a wxglade project that demonstrates an issue centring hyperlink text on Windows platform.

On Mac the native hyperlink text can be centred, so just allocating an appropriate sizer slot, 
and allowing the widget to centre does the right thing.
The widget is expanded to take the entire size of the spacer.

On Windows only left or right alignment is possible, so it doesn't look the same as Mac.

There are 2 work-arounds I can think of.

1. have sizers within sizers.  e.g. the outer sizer splits the space into equal areas, and the inner sizer splits into 3 with spacers either side of the text
2. use wxSHAPED style so that the hyperlink width doesn't expand to the entire sizer area, and the widget can be aligned within the sizer with the layout options.
