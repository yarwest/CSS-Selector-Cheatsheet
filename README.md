# CSS-Selector-Cheatsheet
A cheatsheet for CSS Selectors.
Just something small and useful that I made to aid in the CSS maze of confusedness.

Unless differently specified, classes, ids and elements are interchangeable.

```*``` selects all elements

```element``` selects the DOM element called ‘element’

```#id``` selects an id called ‘id’

```.class``` selects a class called ‘class’


## The basics

Let's start simple.

```element, .class``` selects all elements called ‘element’ and a class called ‘class’

```parent child``` selects all elements called ‘child’ inside an element called ‘parent’

```parent *``` selects all elements inside an element called 'parent'

```parent.child``` selects a class called ‘child’ inside an element called ‘parent’


## Atributes

Attributes are pieces of data that can be added to any DOM element, there are no restrictions to the amount or naming of these elements.

```.class[title]``` selects a class called 'class' containing an attribute called 'title'

```element[title="book"]``` selects all elements called 'element' containing an attribute called 'title' that has 'book' as its value

```a[href*="wiki"]``` selects all link elements containing an href that has 'wiki' somewhere in that href

```a[href^="https"]``` selects all link elements containing an href that starts with 'https'

```a[href$=".png"]``` selects all link elements containing an href that ends with '.png'


## User actions

```.checkbox:checked``` selects a class called 'checkbox' that has been checked, this will only work on radio buttons or checkboxes

```.button:hover``` selects a class called 'button' whenever the user hovers over this element on the page

```.button:click``` simmilar to the previous one, this selector selects a class whenever it is clicked


## Filters

