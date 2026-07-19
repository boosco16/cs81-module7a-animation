## What part of the code was the most confusing and why?

The index % frames.length line took me a while to fully grasp. I understood % gives you a remainder, but I didn't immediately see
why that was useful. But after recognizing that the frames length is 5, I understood that the "%" was responsible of limiting the 
loop. Without this, the code would break as the loop will run infinitely. 

## How does the animation help visualize asynchronous behvior? 

setInterval keeps firing every 500ms by default in the background without effecting the rest of the page. It made the idea of "this runs later, not right now" actually visible instead of something I had to memorize. clearInterval() stopping it was also userful to see, since without it the loop would just run forever, meaning setInterval doesn't stop until you tell it to. 


## What did you change or improve, and what effect did it have? 

I added in a live cycle counter in a new div, as well as changed the background color once the loading has fully finished. 
The counter made the loop feel less infinite and lets you visualize the maxCycles counter. The background color after 
the counter has finished gives it a definitive signal when completed. 
