![SVG Pattern Element](projectHeader.png "SVG Pattern Element")
Scalable Vector Graphic (SVGs) can be used for web development and data visualization. It is mainly used to create vector based images. SVG draws lines at different coordinates on the screen to create the image. A powerful SVG element is pattern!

### Feature 1
The pattern element defines a graphics object which can be redrawn at repeated x and y coordinate intervals ("tiled") to cover an area.

![SVG Pattern Element Feature 1](feature-1.png "Feature 1 Test")

<svg xmlns="http://www.w3.org/2000/svg"
     version="1.1"
     viewBox="0 0 300 200" >

  <title>Example pattern01</title>
  <desc>Fill an ellipse using a pattern paint server.</desc>

  <defs>
    <pattern id="TrianglePattern"
         patternUnits="userSpaceOnUse"
             x="0" y="0" width="50" height="50"
             viewBox="0 0 10 10" >
      <path d="M 0 0 L 7 0 L 3.5 7 z"
          fill="#fdcb6e"
          stroke="#e84393" />
    </pattern>
  </defs>

  <!-- The ellipse is filled using a triangle pattern paint server -->
  <ellipse fill="url(#TrianglePattern)"
       stroke="black"
       stroke-width="2"
           cx="150" cy="100" rx="125" ry="75" />
</svg>


----
##### Attributes


#### Uses
The SVG Pattern element can used for data visualization software, partcularly
graphs and diagrams. For instance, the Github daily commit tracker on a users profile
uses the SVG pattern element.

## Other Resources
- https://developer.mozilla.org/en-US/docs/Web/SVG/Element/pattern
- https://www.sitepoint.com/6-incredible-svg-pattern-generators/
