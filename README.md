# Spark-line

A simple webcomponent **wrapper** to inline spark line svg's. The svg drawing engine  is [fnando/sparkline](https://github.com/fnando/sparkline) and this is a wrapper to help dynamically render AND style spark lines in framework components and nested webcomponents.

![](/resources/spark-line-webcomponent-demo.gif)

### fnando/sparkline Pitfalls

The nando/sparkline pitfalls are the following:
1. Fixed svg `width` styling (not dyanmic/responsive)
2. Fixed svg `height` styling (not dyanmic/responsive)
3. Data manipulation (not dynamic/responsive)

This wrapper helps alleviate those pain points is a simple way.

## Attributes

A definitive list of all attributes on this component.

### data

Use the `data` attribute to assign data to the chart.

#### Example

```html
<spark-line data="[1,2,3,4,5,6,7,8,9,10]"></spark-line>
```

**OR (Recommended)** you can set the JavaScript property, not attribute, to
set the data after the component has been instantiated or to update the data.

```javascript
let sprkLineRef = document.querySelector('spark-line');
sprkLineRef.setData([1,2,3,4,5,6,7,8,9,10]);
```

### line-width

Use the `line-width` attribute to set the `stroke` (in pixels) of the svg.
**The default `line-width` value is `2`.**

#### Example

```html
<spark-line data="[1,2,3,4,5,6,7,8,9,10]" line-width="4"></spark-line>
```

### height

Use the `height` attribute to set the height (in pixels) of the svg. 
**By default the chart will take the size of the container.**

#### Example

```html
<spark-line data="[10]" height="200"></spark-line>
```

### width

Use the `width` attribute to set the height (in pixels) of the svg.
**By default the chart will take the size of the container.**

#### Example

```html
<spark-line data="[10]" height="200" width="200"></spark-line>
```

## License

(The MIT License)

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.