# CSS-tips

Selectors
<ul>
<li>tagname for tags, # for id, . for class</li>
<li>.selector1, .selector2 => two selectors sharing same css</li>
<li>.selector1.selector2 => element having both selectors</li>
<li>.ancestor .child => applied on child of ancestor</li>
<li>selector1,selector2 => two selectors sharing same css</li>
</ul>

Adding style

```
<head>
<link rel="stylesheet" href="style.css" />
</head>
```

Heirarchy of tags

Id>Class>Element

Note: if two tags are of same heirarchy are present, the latter one is implemented
Note: Inline css overrides everything else
