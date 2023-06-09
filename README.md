# CSS-tips

Selectors
<ul>
<li>tagname for tags, # for id, . for class</li>
<li>.selector1, .selector2 => two selectors sharing same css</li>
<li>.selector1.selector2 => element having both selectors</li>
<li>.ancestor .child => applied on child of ancestor</li>
<li>selector1,selector2 => two selectors sharing same css</li>
</ul>

Adding style</br>

```
<head>
<link rel="stylesheet" href="style.css" />
</head>
```

Heirarchy of tags</br>

Id>Class>Element</br>

Note: if two tags are of same heirarchy are present, the latter one is implemented</br>
Note: Inline css overrides everything else</br>

**If an element has no styling, it inherits it's parent's Style**</br>

Padding & Border with box model</br>

```
.box {
height:100px;                         //actual element
width: 100px;
padding: 10px;                        //space between element & it's border
margin; 50px;                         //space between element & another element
border: solid 1Opx black;
backgrournd color: red;
}
```

<h3>units</h3>
% is % of parent</br>
em is multiple of element's font size</br>
em is multiple of root font size</br>

<h3>positioning</h3>

<ol>
<li>Static is default for all elements  => static says to follow natural order i.e one after other</li>

<li>Relative
<ul>
<li>Relative keeps the original space of element in document flow as is & never changes that</li>
<li>Now it allows us to change position relative to the original position it would have</li>
</ul>
</li>

<li>Absolute
<ul>
<li>Absolute takes the element out of document flow & acts like it doesn't exist there or take any place</li>
<li>Now if we position it, it goes on to take the position according to that parent that has either relative, absolute, fixed or sticky</li>
<li>This is done when you want to insert an element in a pre-existing page without disturbing any of the orginal positioning</li>
</ul>
</li>

<li>Fixed
<ul>
<li>Fixed element takes position according to the HTML element, ignoring everything else</li>
<li>Fixed element's position is invisible to other elements, i.e other elements would exist as if sticky was never present there</li>
<li>Fixed element is not affected by scrolling, we would still be able to see it after scrolling down</li>
</ul>
</li>

<li>Sticky
<ul>
<li>Sticky acts like relative or absolute normally, but when it reaches the top value(for eg.) it converts to fixed & sticks there in place</li>
<li>position: sticky; top 10px (when scrolling down it reaches 10px from tops, now it will stick)</li>
<li>position sticky is only sticky inside it's parent element, if parent element itself goes up then it will also go up along with it at it's end</li>
</ul>
</li>

```
list-header {
position: -webkit-sticky;
position: -moz-sticky;
position: -ms-sticky;
position: -o-sticky;
//above kits for support issue
  
position:  sticky;
top: 0px;
```

</ol>


