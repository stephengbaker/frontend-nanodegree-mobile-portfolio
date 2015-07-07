Instructions for running application:
The application can be used as a portfolio site to display projects that you have worked on by updating the information in Index.html with your own contact info and replacing the project site examples with your own true examples.

Detail of performance enhancements made:
In order to get page speed score of index.html above 90, I did the following changes:
1. Inlined the style.css to the index.html
2. Added a media attribute so the print.css would not block rendering
3. Used window.onload so that google page speed api would not block rendering
4. Made all scripts asyncronous

In order to get pizza.html to operate under 60fps, I reduced the number of moving pizzas generated from 200 to 20.

In order to get pizza.html to resize pizzas in under 5ms, I moved variable declaration calculations outside of the for loop so that calculations would only have to be made once.
