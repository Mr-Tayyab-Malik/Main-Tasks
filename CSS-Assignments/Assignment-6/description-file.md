# CSS Combinators:
- *Combinators* are used to define relationships between two or more selectors.
- They help us target HTML elements based on their relationship with other elements.
- And it is also known as the upgrated version of **Selectors**
### In CSS we are having 4 main Combinators:
1. Descendant Combinator ( )
2. Child Combinator (>)
3. Adjacent Sibling Combinator (+)
4. General Sibling Combinator (~)
## 1- Descendant Combinator: 
- It selects all elements that exist inside a parent element,
 including children, grandchildren, and deeply nested elements.
- In the *Descendant Combinator,* all matching elements inside the specified parent element will be targeted,
 no matter how deeply they are nested.
- Symbol **(Space)**
### Example of HTML & CSS 
```HTML
  <div>
    <p>Paragraph 1</p>

    <section>
        <p>Paragraph 2</p>
    </section>
</div>
```
```CSS
div p {
    color: red;
}
```
## 2- Child Combinator:
- It selects only the direct child elements of a specified parent element.
- It does not target grandchildren or deeply nested elements.
- Symbol **(>)**
### Example of HTML & CSS 
```HTML
<div>
    <p>Paragraph 1</p>

    <section>
        <p>Paragraph 2</p>
    </section>
</div>
```
```CSS
div > p {
    color: red;
}
```
#### Here only Para-1 will be targeted.
## 3- Adjacent Sibling Combinator:
- It selects the element that comes immediately after a specified element.
- Both elements must have the same parent element.
- It targets only the immediately following sibling, not all following siblings.
- Symbol **(+)**
### Example of HTML & CSS 
```HTML
<div>
    <h1>Heading</h1>
    <p>Paragraph 1</p>
    <p>Paragraph 2</p>
</div>
```
```CSS
h1 + p {
    color: red;
}
```
#### Here also only Para-1 will be targeted.
## 4- General Sibling Combinator:
- It selects all specified sibling elements that come after a particular element.
- It selects all specified sibling elements that come after a particular element.
- It selects all matching following siblings, not just the immediately next sibling.
- Symbol **(~)**
### Example of HTML & CSS 
```HTML
<div>
    <h1>Heading</h1>
    <p>Paragraph 1</p>
    <h2>Sub Heading</h2>
    <p>Paragraph 2</p>
    <p>Paragraph 3</p>
</div>
```
```CSS
h1 ~ p {
    color: red;
}
```
#### Here Para-1,Para-2 & Para-3 will be targeted.
## Difference B/W Adjacent & General Sibling Combinators:
### Adjacent Sibling Combinator(+):
- Selects only the immediately next sibling.
### General Sibling Combinator(~):
- Selects all matching following siblings.