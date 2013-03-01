simpleGrid
==========

A simple, responsive grid for rapid prototyping in the browser

* Seemless plun-n-play into pre-existing projects
* No dependencies, other than Sass
* Less than 1kb
* Infinite nesting and stacking


<h2>Base Classes</h2>
<div class="data">
<table>
  <thead>
    <tr>
      <th>Property</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
  <tr class="odd">
    <th><code>row</code></th>
    <td>Groups units on one horizontal row.</td>
  </tr>
  <tr class="even">
    <th><code>unit</code></th>
    <td>Base class which divides a line into columns. The sum of all children of a row should be equal to one. (Beware of the [sub-pixel rounding](http://palantir.net/blog/responsive-design-s-dirty-little-secret)). 
  </tr>
  <tr class="odd">
    <th><code>sizeXofY</code></th>
    <td>Extends <code>unit</code>. Indicates the fractional width of the unit.</td>
  </tr>
</tbody>
</table>
</div>

###Note:
* Use optional grid-classes for OOCSS styling, or Sass @extend for cleaner markup
* A unit can contain another row or it can contain other objects directly.  
* Grids control width, content controls height. 
* Apply styles to grid objects, never to grid itself.

##Examples:

###1/3, 1/3, 1/3

```
<div class="row">
  <div class="unit size1of3">
    <h3>1/3</h3>
    <p>Lorem ipsum dolor sit amet...</p>
  </div>
  <div class="unit size1of3">
    <h3>1/3</h3>
    <p>Lorem ipsum dolor sit amet...</p>
  </div>
  <div class="unit size1of3">
    <h3>1/3</h3>    
    <p>Lorem ipsum dolor sit amet...</p>
  </div>
</div>

```

###1/3, 2/3

```
<div class="row">
  <div class="unit size1of3">
    <h3>1/3</h3>
    <p>Lorem ipsum dolor sit amet...</p>
  </div>
  <div class="unit size2of3">
    <h3>2/3</h3>
    <p>Lorem ipsum dolor sit amet...</p>
  </div>
</div>

```
