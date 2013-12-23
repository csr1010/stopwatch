stopwatch
=========

stop watch with controls like start, hold,split,stop,reset etc


the stop watch application is developed using
     javascirpt,bootstrap-for CSS, and HTML5
	 HTML5->webworkers,cache.
Buttons:

start -> starts the timer always from 0

hold -> Holds the timer ,will continue only when clicked on the continue button.,if clicked on play button it will start again from begining i.e 0

continue-> will continue the paused time

reset ->will clear the time to 0,and clear the content in the table

stop ->will stop the timer and add the result to the table on right with default task name, and logs the stopped time

split ->splits the time at the point and logs the split timings in a table along with taskname and individual split event
         by default task name is taskname and individual split event is 1,2,3 ....i.e row no:
		 
used module pattern approach  to acheive the same

works fine in ie 10, chrome ,safari , firefox

responsive design to fit fine in desktop/tablet.


concept:

every i millisecond i calculate the gettime(),which gives me millisecs from 1970,jan 1st,

I ll save that as start time and subtract the current millisecs from start,

I ll then calculate the time spent based on the millisecs

when i keep on hold,
          i ll calculate the millsecs at the point of hold, whne user click on continues, I ll calculate the  difference between New gettime() and Hold time(previosuly saved when user clicks on hold)
		  
		  now i should eliminate this difference every time,
		  
		  => nowgetTime() - starttime -difference will set our pointer back to hold point.
		  

Please get me back,if by any chance its not working or any bug found, so that i can correct it send u back soon.


