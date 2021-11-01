# flex

- [阮一峰 flex](https://www.ruanyifeng.com/blog/2015/07/flex-grammar.html)

```css
/*
    容器属性 
*/
/* 启用 flex布局 */
display: flex | inline-flex;
/* 默认:row。设置主轴方向。 */
flex-direction: row | column | row-reverse | column-reverse;
/* 默认:nowrap。如果一条轴线排不下，如何换行。wrap-reverse:首先会wrap，之后形成的多行以行为单位进行reverse */
flex-wrap: nowrap | wrap | wrap-reverse;
/* 默认:row nowrap。flex-direction和flex-wrap的简写，值与顺序无关 */
flex-flow: <flex-direction> || <flex-wrap>;
/* 默认:flex-start。 主轴对其方式。space-around:项目之间的间隔比项目与边框之间的间隔大一倍*/
justify-content: flex-start | flex-end | center | space-between | space-around;
/* 默认:stretch。辅轴（交叉轴）对其方式。stretch: 拉伸至整个容器。baseline: 项目的第一行文字基线 */
align-items: stretch | flex-start | flex-end | center | baseline;
/* 默认:stretch。多根轴线的对其方式，一个无效 */
align-content: stretch | flex-start | flex-end | center | space-between |
  space-around;

/*
    项目属性
*/
/* 默认:0。定义项目排列顺序，数值越小越靠前 */
order: <integer>;
/* 默认:0。定义项目放大比例，0表示，即使有剩余空间也不放大 */
flex-grow: <number>;
/* 默认:1。定义项目缩小比例 */
flex-shrink: <number>;
/* 默认:auto。定义了在分配多余空间时，项目占据的主轴空间，浏览器根据这个属性计算主轴是否有多余空间。auto: 项目的本来大小；length: 如300px*/
flex-basis: auto | <length>;
/* 默认:0 1 auto。flex-grow、flex-shrink、flex-basis的简写。推荐使用简写。none(0 0 auto)、auto(1 1 auto) */
flex: none | auto | <flex-grow> <flex-shrink> ? || <flex-basis>;
/* 默认:auto,表示继承父元素align-item | stretch。允许单个项目有与其他项目不一样的对齐方式，可覆盖align-items。 */
align-self: auto | stretch | flex-start | flex-end | center | baseline;
```
