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
height:100px;
width: 100px;
padding: 10px;
margin; 50pq;
border: solid O black;
backgrournd color: red;
}
```
