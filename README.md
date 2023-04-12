# LoadBlurr
## This is a JavaScript code that creates a simple loading animation by blurring the background of a webpage while displaying a percentage of the loading progress.

> The code starts by selecting two elements from the HTML document using the querySelector() method. The first element is a paragraph element with a class of loading-text that displays the percentage of the loading progress. The second element is a background element with a class of bg that will be blurred as the loading progresses.

> Then, two variables are defined: load and int. load starts at 0 and will be incremented by 1 each time the blurring() function is called. int is used to store the return value of setInterval(), a built-in JavaScript function that repeatedly calls a function or executes a code snippet, with a fixed time delay between each call. In this case, blurring() will be called every 30 milliseconds until clearInterval(int) is executed.

> The blurring() function is defined next. It increments the load variable, and checks if load is greater than 99. If load is greater than 99, clearInterval(int) is called to stop the execution of blurring(). Otherwise, the percentage value of load is displayed in the innerText property of the loadText element, and the opacity of loadText is changed according to the value of load using the scale() function. The scale() function maps a range of numbers (in this case, the range of load values from 0 to 100) to another range of numbers (in this case, the opacity values from 1 to 0). The blur() function is used to blur the background image of the webpage, and its intensity is also determined by the value of load, using the scale() function.

> Finally, the scale() function is defined, which takes five arguments: num (the number to be scaled), in_min and in_max (the minimum and maximum values of the original range), out_min and out_max (the minimum and maximum values of the target range). It returns the scaled value of num. This function is used to convert the range of load values into opacity and blur values that can be applied to the loadText and bg elements.

### In summary, this code creates a simple loading animation that updates the percentage value and the blur intensity of the background image as the loading progresses.
