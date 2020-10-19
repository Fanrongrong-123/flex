## flex布局

.container是父元素，items是子元素

1、让一个元素变成容器

    .container{
        display:flex;
    }

## flex container 样式

    .container{
        flex direction:row | row-reverse | column | column-reverse(改变主轴流动方向：从左往右、从右往左、从上到下、从下到上)
    }

    .container{
        flex-wrap:nowrap | wrap | wrap-reverse(改变折行：默认值、换行、反向换行)
    }

    .container{
        justify-content:flex-start | flex-end | center |space-between | space-around | space-evenly(主轴对其方式：左对齐、右对齐、居中对齐、空间在中间、每个元素左右两边距离相等、空间平均包围)
    }

    .container{
        align-items:streth | flex-start | flex-end | center(次轴对齐：高度相等 | 底部在上面 | 底部在下面 | 中心对齐）
    }
    align-self定制align-items
    例：align-self:flex-end

    .container{
        align-content:flex-start | flex-end(多行内容分布)
    }


## flex item 样式

    .item{
        order:100(默认值为零，数值越大位置越靠后，可以为负数位置在默认值之前)
    }

    .item{
        flex-grow:1(默认值为零，控制如何变宽)
        flex-shrink:0(默认值为一，控制如何变窄)
        flex-basis:xx px(默认是auto，控制基准宽度与width差别不大)
    }

    flex:flex-grow flex shrink flex-basis的缩写：例flex:1 100 100px

    

