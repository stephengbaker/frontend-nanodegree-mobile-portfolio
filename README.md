#Udacity Project 4 Readme

##Instructions for running application using Github pages:

1. To run application, first ensure the files are in a gh-pages repository.
2. Go to http://stephengbaker.github.io/frontend-nanodegree-mobile-portfolio/

More details can be found here: https://pages.github.com/

##Detail of performance enhancements made:

###Index.html:

In order to get page speed score of index.html above 90, I did the following changes:
1. Inlined the style.css to the index.html
2. Added a media attribute so the print.css would not block rendering
3. Used window.onload so that google page speed api would not block rendering
4. Made scripts asyncronous

###Pizza.html 60fps:

In order to get pizza.html to operate under 60fps, I reduced the number of moving pizzas from 200 to a number automatically determined by the size of the viewport. I also moved some calculations outside of for loops and replaced querySelector's with getElementById's to improve performance.

###Pizza.html resize<5ms:

In order to get pizza.html to resize pizzas in under 5ms, I moved variable declaration calculations outside of the for loop so that calculations would only have to be made once.

##Resources Used:

*https://www.developers.google.com/speed

*http://www.w3schools.com/jsref/event_onload.asp

*Udacity Project 4 office hours

*https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/round

*http://www.stoimen.com/blog/2012/01/24/javascript-performance-for-vs-while/

*http://www.kirupa.com/html5/loops_in_javascript.htm

*https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementById

*https://help.github.com/articles/markdown-basics/
