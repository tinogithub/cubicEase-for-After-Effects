# cubicEase-for-After-Effects
This is a function to use in After Effects expressions and have the advantage of cubic-bezier values.
Look on https://cubic-bezier.com to build your favourite curve and calculate the cubic-bezier values.

Thanks to Friedrich Schultheiss who published a cubic bezier function in Javascript that I use here. I just tweaked it a little to work in After Effects.
Link: https://gist.github.com/symdesign/713ed58de32349cfeeb517b7352121df

The function works like the common ease-function. It just comes with a new parameter, the cubic bezier values:
cubicEase(time, startTime , endTime, valueMin, valueMax, [cubic-bezier-values]);

An example on a path trim:
cubicEase(time, 0 , 2, 0, 100, [1, 0, 0.9, 0]);
