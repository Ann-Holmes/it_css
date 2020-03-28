# 查找到的有用资源

- [CSS水平居中+垂直居中+水平/垂直居中的方法总结](https://blog.csdn.net/weixin_37580235/article/details/82317240#%C2%A0%E5%9D%97%E7%BA%A7%E5%85%83%E7%B4%A0)

- [在CSS中定义超链接样式](https://www.cnblogs.com/52php/p/5657597.html)

# 保留文本中的空格

只需要在CSS样式中添加: 

```css
.bottom {
    white-space: pre;
}
```

# `header` 标签

- `header` 是一个块级标签
- `header` 的[全局属性](https://www.runoob.com/tags/ref-standardattributes.html)
- `header` 的[事件属性](https://www.runoob.com/tags/ref-eventattributes.html)

# [`input`标签](https://www.w3school.com.cn/tags/tag_input.asp)

目前会用到的属性: 

`pattern`, `placeholder`, `type`, `value`. 

`id`：作为标签的唯一标识。
`name`：作为可与服务器交互数据的[HTML元素](https://www.baidu.com/s?wd=HTML元素&tn=SE_PcZhidaonwhc_ngpagmjz&rsv_dl=gh_pc_zhidao)的[服务器端](https://www.baidu.com/s?wd=服务器端&tn=SE_PcZhidaonwhc_ngpagmjz&rsv_dl=gh_pc_zhidao)的标示。

`input` 块级元素, 因此所有对`div`标签有效的CSS属性, 对于`input` 都有效. 

### [设置input标签的placeholder属性的字体和颜色](https://www.cnblogs.com/hcxwd/p/9232936.html)



| 属性                                                         | 值                                                           | 描述                                                         |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| [accept](https://www.w3school.com.cn/tags/att_input_accept.asp) | *mime_type*                                                  | 规定通过文件上传来提交的文件的类型。                         |
| [align](https://www.w3school.com.cn/tags/att_input_align.asp) | left, right, top, middle, bottom                             | 不赞成使用。规定图像输入的对齐方式。                         |
| [alt](https://www.w3school.com.cn/tags/att_input_alt.asp)    | text                                                         | 定义图像输入的替代文本。                                     |
| [autocomplete](https://www.w3school.com.cn/tags/att_input_autocomplete.asp) | on, off                                                      | 规定是否使用输入字段的自动完成功能。                         |
| [autofocus](https://www.w3school.com.cn/tags/att_input_autofocus.asp) | autofocus                                                    | 规定输入字段在页面加载时是否获得焦点。（不适用于 type="hidden"） |
| [checked](https://www.w3school.com.cn/tags/att_input_checked.asp) | checked                                                      | 规定此 input 元素首次加载时应当被选中。                      |
| [disabled](https://www.w3school.com.cn/tags/att_input_disabled.asp) | disabled                                                     | 当 input 元素加载时禁用此元素。                              |
| [form](https://www.w3school.com.cn/tags/att_input_form.asp)  | *formname*                                                   | 规定输入字段所属的一个或多个表单。                           |
| [formaction](https://www.w3school.com.cn/tags/att_input_formaction.asp) | *URL*                                                        | 覆盖表单的 action 属性。（适用于 type="submit" 和 type="image"） |
| [formenctype](https://www.w3school.com.cn/tags/att_input_formenctype.asp) | 见注释                                                       | 覆盖表单的 enctype 属性。（适用于 type="submit" 和 type="image"） |
| [formmethod](https://www.w3school.com.cn/tags/att_input_formmethod.asp) | get, post                                                    | 覆盖表单的 method 属性。（适用于 type="submit" 和 type="image"） |
| [formnovalidate](https://www.w3school.com.cn/tags/att_input_formnovalidate.asp) | formnovalidate                                               | 覆盖表单的 novalidate 属性。如果使用该属性，则提交表单时不进行验证。 |
| [formtarget](https://www.w3school.com.cn/tags/att_input_formtarget.asp) | _blank, _self, _parent, _top*framename*                      | 覆盖表单的 target 属性。（适用于 type="submit" 和 type="image"） |
| [height](https://www.w3school.com.cn/tags/att_input_height.asp) | *pixels %*                                                   | 定义 input 字段的高度。（适用于 type="image"）               |
| [list](https://www.w3school.com.cn/tags/att_input_list.asp)  | *datalist-id*                                                | 引用包含输入字段的预定义选项的 datalist 。                   |
| [max](https://www.w3school.com.cn/tags/att_input_max.asp)    | *number, date*                                               | 规定输入字段的最大值。请与 "min" 属性配合使用，来创建合法值的范围。 |
| [maxlength](https://www.w3school.com.cn/tags/att_input_maxlength.asp) | number                                                       | 规定输入字段中的字符的最大长度。                             |
| [min](https://www.w3school.com.cn/tags/att_input_min.asp)    | *number, date*                                               | 规定输入字段的最小值。请与 "max" 属性配合使用，来创建合法值的范围。 |
| [multiple](https://www.w3school.com.cn/tags/att_input_multiple.asp) | multiple                                                     | 如果使用该属性，则允许一个以上的值。                         |
| [name](https://www.w3school.com.cn/tags/att_input_name.asp)  | field_name                                                   | 定义 input 元素的名称。                                      |
| [pattern](https://www.w3school.com.cn/tags/att_input_pattern.asp) | *regexp_pattern*                                             | 规定输入字段的值的模式或格式。例如 pattern="[0-9]" 表示输入值必须是 0 与 9 之间的数字。 |
| [placeholder](https://www.w3school.com.cn/tags/att_input_placeholder.asp) | *text*                                                       | 规定帮助用户填写输入字段的提示。                             |
| [readonly](https://www.w3school.com.cn/tags/att_input_readonly.asp) | readonly                                                     | 规定输入字段为只读。                                         |
| [required](https://www.w3school.com.cn/tags/att_input_required.asp) | required                                                     | 指示输入字段的值是必需的。                                   |
| [size](https://www.w3school.com.cn/tags/att_input_size.asp)  | number_of_char                                               | 定义输入字段的宽度。                                         |
| [src](https://www.w3school.com.cn/tags/att_input_src.asp)    | URL                                                          | 定义以提交按钮形式显示的图像的 URL。                         |
| [step](https://www.w3school.com.cn/tags/att_input_step.asp)  | *number*                                                     | 规定输入字的的合法数字间隔。                                 |
| [type](https://www.w3school.com.cn/tags/att_input_type.asp)  | button, checkbox, file, hidden,  image, password, radio, reset, submit, text | 规定 input 元素的类型。                                      |
| [value](https://www.w3school.com.cn/tags/att_input_value.asp) | *value*                                                      | 规定 input 元素的值。                                        |
| [width](https://www.w3school.com.cn/tags/att_input_width.asp) | *pixels %*                                                   | 定义 input 字段的宽度。（适用于 type="image                  |

# [`form`标签](https://www.w3school.com.cn/tags/tag_form.asp)

## 定义和用法

- `<form>`签用于为用户输入创建 HTML 表单。
- 表单能够包含 [input 元素](https://www.w3school.com.cn/tags/tag_input.asp)，比如文本字段、复选框、单选框、提交按钮等等。
- 表单还可以包含 [menus](https://www.w3school.com.cn/tags/tag_menu.asp)、[textarea](https://www.w3school.com.cn/tags/tag_textarea.asp)、[fieldset](https://www.w3school.com.cn/tags/tag_fieldset.asp)、[legend](https://www.w3school.com.cn/tags/tag_legend.asp) 和 [label 元素](https://www.w3school.com.cn/tags/tag_label.asp)。
- 表单用于向服务器传输数据。

## [`method` 属性](https://www.w3school.com.cn/tags/att_form_method.asp)

- method 属性规定如何发送表单数据（表单数据发送到 action 属性所规定的页面）。
- 表单数据可以作为 URL 变量（method="get"）或者 HTTP post （method="post"）的方式来发送。

### `method` 详解

浏览器使用 method 属性设置的方法将表单中的数据传送给服务器进行处理。共有两种方法：POST 方法和 GET 方法。

如果采用 POST 方法，浏览器将会按照下面两步来发送数据。

- 首先，浏览器将与 action 属性中指定的表单处理服务器建立联系，一旦建立连接之后，浏览器就会按分段传输的方法将数据发送给服务器。

- 在服务器端，一旦 POST 样式的应用程序开始执行时，就应该从一个标志位置读取参数，而一旦读到参数，在应用程序能够使用这些表单值以前，必须对这些参数进行解码。用户特定的服务器会明确指定应用程序应该如何接受这些参数。

另一种情况是采用 GET 方法，这时浏览器会与表单处理服务器建立连接，然后直接在一个传输步骤中发送所有的表单数据：浏览器会将数据直接附在表单的 action URL 之后。这两者之间用问号进行分隔。

一般浏览器通过上述任何一种方法都可以传输表单信息，而有些服务器只接受其中一种方法提供的数据。可以在 `<form>` 标签的 method （方法）属性中指明表单处理服务器要用方法来处理数据，使 POST 还是 GET。

### POST 还是 GET？

如果表单处理服务器既支持 POST 方法又支持 GET 方法，那么你该选择哪种方法呢？下面是有关这方面的一些规律：

- 如果希望**获得最佳表单传输性能**，可以采用 GET 方法发送只有少数简短字段的小表单。
- 一些服务器操作系统在处理可以立即传递给应用程序的命令行参数时，会限制其数目和长度，在这种情况下，对那些有许多字段或是很长的文本域的表单来说，就应该采用 POST 方法来发送。
- 如果你在编写服务器端的表单处理应用程序方面经验不足，应该选择 GET 方法。如果采用 POST 方法，就要在读取和解码方法做些额外的工作，也许这并不很难，但是也许你不太愿意去处理这些问题。
- 如果**安全性是个问题**，那么我们建议选用 POST 方法。GET 方法将表单参数直接放在应用程序的 URL 中，这样网络窥探者可以很轻松地捕获它们，还可以从服务器的日志文件中进行摘录。如果参数中包含了信用卡帐号这样的敏感信息，就会在不知不觉中危及用户的安全。而 POST 应用程序就没有安全方面的漏洞，在将参数作为单独的事务传输给服务器进行处理时，至少还可以采用加密的方法。
- 如果想在表单之外调用服务器端的应用程序，而且包括向其传递参数的过程，就要采用 GET 方法，因为该方法允许把表单这样的参数包括进来作为 URL 的一部分。而另一方面，使用 POST 样式的应用程序却希望在 URL 后还能有一个来自浏览器额外的传输过程，其中传输的内容不能作为传统 `<a> `标签的内容。

| 值          | 描述                       |
| :---------- | :------------------------- |
| _blank      | 在新窗口中打开。           |
| _self       | 默认。在相同的框架中打开。 |
| _parent     | 在父框架集中打开。         |
| _top        | 在整个窗口中打开。         |
| *framename* | 在指定的框架中打开。       |

