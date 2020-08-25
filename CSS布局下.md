flex 布局是一维布局，横着排或者竖着排
grid 布局两个方向都可以 ! [grid 布局](2.png)
先成为 container
.container{
display:grid | inline-grid;
}
.container{
grid-template-columns:40px 50px auto 50px 40px;
grid-template-rows:25% 100px auto;
}
第一个 40px 是第一列的宽度，以此类推
25%是横轴的宽度

.container{
grid-template-columns：1fr 1fr 1fr；
} free space
.container{
grid-template-columns：1fr 50px 1fr 1fr；
}

分区：grid-template-areas
item-a{
grid-area：header；
}
item-b{
grid-area：main；
}
item-c{
grid-area：sidebar；
}
item-d{
grid-area：footer；
}
。container{
display：grid；
gird-template-columns：50px 50px 50px 50px；
grid-template-rows：auto；
grid-template-areas：
“header header header header”
“main main sidebar”
“footer footer footer footer”；
}

grid-gap：grid 间隙
