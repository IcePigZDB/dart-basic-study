---
layout:     post
title:      "测试MarkDown页内跳转统一用法 "
subtitle:   "VsCode中的跳转和Typora（博客）的不能统一就很麻烦。"
date:       2020-04-19 23:59:59
author:     "IcePig"
header-img: "img/in-post/2020-04-19-blog-design-and-implement/summer-flower.jpg"
catalog: true
tags:
    - MarkDown
typora-root-url: ..
---




# Anchor 1

```html
Anchor1：<a id="anchor1">Anchor1</a>  
Jump1：<a href="#anchor1">Link to Anchor1</a>
```

Anchor1：<a id="anchor1">Anchor1</a>  

# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
Jump1：<a href="#anchor1">Link to Anchor1</a>

# Anchor 2
```html
Anchor2：<a name= "anchor2">Anchor2</a>
Jump2：<a href="#anchor2">Link to Anchor2</a>
```

Anchor2：<a name= "anchor2">Anchor2</a>

# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
Jump2：<a href="#anchor2">Link to Anchor2</a>

# Anchor 3
```html
Anchor3：<span id="anchor3">Anchor3</span> 
Jump3：<a href="#anchor3">Link to Anchor3</a>
```

Anchor3：<span id="anchor3">Anchor3</span>  

# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
Jump3：<a href="#anchor3">Link to Anchor3</a>

# Anchor 4
```html
Anchor4：<span name= "anchor4">Anchor4</span>
Jump4：<a href="#anchor4">Link to Anchor4</a>
```

Anchor4：<span name= "anchor4">Anchor4</span>

# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
Jump4：<a href="#anchor4">Link to Anchor4</a>

# Anchor 5
```html
Anchor5：<a id="anchor5">Anchor5</a>
Jump5：[Link to Anchor5](#anchor5)
```

Ancho5r：<a id="anchor5">Anchor5</a>

# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
Jump5：[Link to Anchor5](#anchor5)

# Anchor 6
```html
Anchor6：<a name="anchor6">Anchor6</a>
Jump6：[Link to Anchor6](#anchor6)
```

Anchor6：<a name="anchor6">Anchor6</a>

# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
Jump6：[Link to Anchor6](#anchor6)

# Anchor7
```html
Anchor7： Header :# Anchor7
Jump7：[Link to Anchor7](#Anchor7)
```

# 1

# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
# 1
Anchor7： Header :# Anchor7
Jump7：[Link to Anchor7](#Anchor7)



| Anchor | info             | Typora | VsCode | GFM  |
| :----- | ---------------- | ------ | ------ | ---- |
| 1      | <a ,id ,<href    | ✗      | ✓      | ✓    |
| 2      | <a ,name ,<href  | ✓      | ✗      | ✓    |
| 3      | <span,id,<href   | ✗      | ✓      | ✓    |
| 4      | <span,name,<href | ✓      | ✗      | ✓    |
| 5      | <a,id,[](#       | ✗      | ✓      | ✓    |
| 6      | <a,name,[](#     | ✓      | ✗      | ✓    |
| 7      | # header [](#    | ✓      | ✓      | ✓    |