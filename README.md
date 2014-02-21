front-end-skills
================

前端开发奇淫技巧-个人前端技巧收藏夹

###性能优化###

UL有 10000 个LI子元素，如何将这 10000 个LI颠倒顺序? [http://v2ex.com/t/100982]

CSS:
```css
    ul {transform: rotate(180deg)} 
    li {transform: rotate(180deg)}
```  
Javascript:

```javascript
    [].slice.call(nodeList).reverse(); //循环一次组成字符串插回 ul 节点
```
