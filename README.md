![SVG Pattern Element](projectHeader.png "SVG Pattern Element")
Scalable Vector Graphic (SVGs) can be used for web development and data visualization. It is mainly used to create vector based images. SVG draws lines at different coordinates on the screen to create the image. A powerful SVG element is pattern! The many uses and features of the pattern element are described below.

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

### Feature 2
Most of the time a pattern is filling a shape. To
accomplish is in the SVG element with give the shape a style property fill
that is referencing the pattern defined above.

![SVG Pattern Element Feature 2](feature-2.png "Feature 2 Test")

    <svg
        viewBox="0 0 300 200">
        <defs>
            <pattern id="myPattern"
                     x="10" y="10" width="20" height="20"
                     patternUnits="userSpaceOnUse">
                     <!--start pattern-->
                     <circle cx="10" cy="10" r="7" style="stroke: none;
                     fill: #307476"/>
                    <!-- end pattern -->
            </pattern>
        </defs>
        <circle cx="60" cy="60" r="60" style="stroke: #DA502A; stroke-width: 3px; fill:url(#myPattern);" />
    </svg>

### Feature 3
The is not only used to fill circular shapes, but
other basic shapes as well such as a line, polygons, rectangles, and polylines.

![SVG Pattern Element Feature 3](feature-3.png "Feature 3 Test")
----
#### Attributes


#### Uses
The SVG Pattern element can used for data visualization software, particularly
graphs and diagrams. For instance, the Github daily commit tracker on a users profile
uses the SVG pattern element.

SVG allows you build up complex, layered patterns.

Furthermore there is software that generates SVG patterns that you can
download for free such as Hero Pattern and SVG Patterns Gallery.

## Browser Support
The SVG pattern element has basic support from most browsers.
- Chrome
- Edge
- Firefox
- IE
- Opera
- Safari
- WebView Android
- Chrome Android
- Edge Mobile
- Firefox Android
- Opera Android
- Safari iOS

However valuable pattern element attributes such `patternUnits`, `patternContentUnits`, and `patternTransform` are only supported by Safari.

## Documentation
- https://developer.mozilla.org/en-US/docs/Web/SVG/Element/pattern

## Other Resources
- http://vanseodesign.com/web-design/svg-basics/
- https://www.sitepoint.com/6-incredible-svg-pattern-generators/
