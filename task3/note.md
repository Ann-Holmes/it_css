# CSS 定位

## CSS 定位属性允许对元素进行定位

### CSS 定位和浮动

- 一切皆为框

    div、h1 或 p 元素常常被称为块级元素。这意味着这些元素显示为*一块内容*，即“块框”。与之相反，span 和 strong 等元素称为“行内元素”，这是因为它们的内容显示在行中，即“行内框”。

    可以使用 [display 属性](https://www.w3school.com.cn/cssref/pr_class_display.asp)改变生成的框的类型。

### CSS 定位机制

- 普通流
- 浮动
- 绝对定位





# CSS中的单位

| 单位 | 描述                                                         |
| :--- | :----------------------------------------------------------- |
| %    | 百分比                                                       |
| in   | 英寸                                                         |
| cm   | 厘米                                                         |
| mm   | 毫米                                                         |
| em   | 1em 等于当前的字体尺寸。2em 等于当前字体尺寸的两倍。例如，如果某元素的字体大小是 12px，那么 2em 是24px。在 CSS 中，em 是非常有用的单位，因为它可以自动适应用户所使用的字体。 |
| ex   | 一个 ex 是一个字体的 x-height。 (x-height 通常是字体尺寸的一半。) |
| pt   | 磅 (1 pt 等于 1/72 英寸)                                     |
| pc   | 12 点活字 (1 pc 等于 12 点)                                  |
| px   | 像素 (计算机屏幕上的一个点)                                  |

# 弹性设计

> 关键: **Web页面中所有元素都使用“em”单位值**
>
> 掌握 "font-size", "px" 和 "em" 之间的关系

任意浏览器的默认字体高都是16px, 所有未经调整的浏览器都符合:  1em=16px。

为了简化font-size的换算, 需要在css中的body选择器中声明: font-size=62.5%, 这就使em值变为 16px*62.5%=10px

### 写CSS的注意事项: 

1. body选择器中声明Font-size=62.5%；

2. 将你的原来的px数值除以10，然后换上em作为单位；

3. 由于每一级元素的em实际大小都继承自父元素的px, 因此要重新计算那些被放大的字体的em数值。避免字体大小的重复声明。

    如: 1.4em x 1.4em = 2. 96em 

### rem 特点

rem：是一个相对单位，相对根元素字体大小的单位，再直白点就是相对于html元素字体大小的单位。

优点：这样在计算子元素有关的尺寸时，只要根据html元素字体大小计算就好。不再像使用em时，要重新计算那些被放大的字体的em数值. 

# PS/GIMP 切图的作用

1. 导出当前图片的HTML布局
2. 获取某一个组件



## GIMP 切图

GIMP切图只能按照Guides 创建HTML布局和切图. PS似乎功能更多, 但是在Ubuntu下用PS比较麻烦, 暂时不予考虑. 

