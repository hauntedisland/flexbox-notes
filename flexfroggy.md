## flex布局学习

> [Flexbox Froggy - A game for learning CSS flexbox](https://flexboxfroggy.com/)

### flex basic attributes

- `flex direction`：改变主轴(flex items放置的)方向
	- `row`: Items are placed the same as the text direction.横
	- `row-reverse`: Items are placed opposite to the text direction.横反
	- `column`: Items are placed top to bottom.竖
	- `column-reverse`: Items are placed bottom to top.竖反
- `flex-wrap`：决定flex items是否出现在同一行上
	- `nowrap`: Every item is fit to a single line.同一行
	- `wrap`: Items wrap around to additional lines.不出现在同一行
	- ==`wrap-reverse`: Items wrap around to additional lines in reverse.==
	> [cssreference.io](https://cssreference.io/flexbox/#flex-wrap)![[Pasted image 20241204144106.png|700]]
- `flex-flow`=`flex-wrap`+`flex-direction`
	- `flex-direction参数` `flex-wrap参数`

### main axis

- `justify-content`: 在主轴上改变flex item的位置
	- `flex-start`: Items align to the left side of the container.最左
	- `flex-end`: Items align to the right side of the container.最右
	- `center`: Items align at the center of the container.居中
	- `space-between`: Items display with equal spacing between them.剩余空间在flex items之间，相对于整个flex container
	- `space-around`: Items display with equal spacing around them.剩余空间在flex items周围包裹

### cross axis
- `align-self`：对单个flex items进行纵向操作，内容与`align-items`一样
- `align-items`：在纵轴上对齐flex items
	- `flex-start`: Items align to the top of the container.最上
	- `flex-end`: Items align to the bottom of the container.最下
	- `center`: Items align at the vertical center of the container.居中
	- `baseline`: Items display at the baseline of the container.
	- `stretch`: Items are stretched to fit the container.占满空间
- `align-content`：当纵轴还有剩余空间时，让全部flex items对齐。只有多行时生效。 
	- `flex-start`: Lines are packed at the top of the container.
	- `flex-end`: Lines are packed at the bottom of the container.
	- `center`: Lines are packed at the vertical center of the container.
	- `space-between`: Lines display with equal spacing between them.
	- `space-around`: Lines display with equal spacing around them.
	- `stretch`: Lines are stretched to fit the container.

- `order`：对单个flex items设置值，从而将全部flex items按照值顺序排序![[Pasted image 20241204141843.png|350]]