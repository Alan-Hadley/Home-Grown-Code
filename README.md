I have written an image stacking program called CombineZ which is now very old and out of date.
I have also written a general purpose program for processing objects like images, strings, mathematical expressions, simulations etc. These programs rely on several PD libraries, some of which are quite old. So I would like to recode their functionality using the QT libraries and my own code.
I am first developing a general purpose Expression Parser, which takes a string as input, converts it into a tree consisting of nodes and connections and then simplifies the parts with mathematical operators that it understands. Needless to say if you input "2+2" you can get 4 as a double or a string as the simplified result.
The Parser is a single class in C++. It supports the standard maths operators, a host of operators that the user, programmer,  can define, several types of functions, three types of brackets, punctuation, variables, expression signatures and capturing parts of expressions.
For maximum flexability it uses static callback functions that you register with it. So far I have started on a differential calculus class, another that implements the standard cmaths library functions, a function that can recognize and solve a quadratic in a variable of your choice and some trial operators such as << shift left.