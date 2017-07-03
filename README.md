# CSS-Selector-Cheatsheet
A cheatsheet for CSS Selectors.
Just something small and useful that I made to aid in the CSS maze of confusedness.

Not a complete list, will update every once in a while.

Unless differently specified, classes, ids and elements are interchangeable.

1. ```*``` selects all elements.

2. ```element``` selects the DOM element called ‘element’.

3. ```#id``` selects an id called ‘id’.

4. ```.class``` selects a class called ‘class’.


## The basics

Let's start simple.

5. ```element, .class``` selects all elements called ‘element’ and a class called ‘class’.

6. ```parent child``` selects all elements called ‘child’ inside an element called ‘parent’.

7. ```parent *``` selects all elements inside an element called 'parent'.

8. ```parent.child``` selects a class called ‘child’ inside an element called ‘parent’.


## Atributes

Attributes are pieces of data that can be added to any DOM element, there are no restrictions to the amount or naming of these elements.

9. ```.class[title]``` selects a class called 'class' containing an attribute called 'title'.

10. ```element[title="book"]``` selects all elements called 'element' containing an attribute called 'title' that has 'book' as its value.

11. ```a[href*="wiki"]``` selects all link elements containing an href that has 'wiki' somewhere in that href.

12. ```a[href^="https"]``` selects all link elements containing an href that starts with 'https'.

13. ```a[href$=".png"]``` selects all link elements containing an href that ends with '.png'.


## User actions

There are various ways to handle styling based on user interaction with the object.

14. ```.checkbox:checked``` selects a class called 'checkbox' that has been checked, this will only work on radio buttons or checkboxes.

15. ```.button:hover``` selects a class called 'button' whenever the user hovers over this element on the page.

16. ```.button:click``` simmilar to the previous one, this selector selects a class whenever it is clicked.


## Filters

17. ```div:not(#container)``` selects all elements called 'div' that do not have 'container' as it's id.

18. ```ul li:first-child``` selects the first 'li' element inside all 'ul' elements.

19. ```ul li:last-child``` selects the last 'li' element inside all 'ul' elements.

20. ```ul li:nth-child(3)``` selects the third 'li' element inside the parent 'ul' element.

21. ```ul li:nth-last-child(3)``` the same as number 18 but instead of counting from the start, this selector takes the third 'li' element from the end.

22. ```ul:first-of-type``` selects the first 'ul' element on the page.

24. ```ul:last-of-type``` selects the last 'ul' element on the page.

25. ```ul:nth-of-type(3)``` this selector takes the third 'ul' element on the page. The difference between number 20 and this one is that the 'ul' element that we are selecting now does not have to be a child of any other element.

26. ```ul::nth-last-of-type(3)``` combine numbers 21 and 25 and you get this selector. 
