front-end-skills
================

前端开发奇淫技巧-个人前端技巧收藏夹

================

###性能优化###
--
>**UL有 10000 个LI子元素，如何将这 10000 个LI颠倒顺序?** 摘自[V2EX](http://v2ex.com/t/100982)
```css
    /* Css方式: */
    ul {transform: rotate(180deg)} 
    li {transform: rotate(180deg)}
```
```javascript
    //Javascript方式:
    [].slice.call(nodeList).reverse(); //循环一次组成字符串插回 ul 节点
```

###CSS效果###
--
>**利用css3动画增强页面效果**
```html
    <div class="css_3">
        <img src="1.jpg />
    </div>
```
```css
    .css_3 img {transition: all .8s ease 0s;}
    .css_3:hover img {transform: scale(1.1);} /* hover时 img放大 可以有很多效果,如改变透明度等等 */
```
