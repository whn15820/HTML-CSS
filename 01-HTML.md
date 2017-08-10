## HTML
全称：`HyperText Markup Language`

文本文档不具备任何的样式。我们通用加上标签的形式，让原有的内容呈现出我们想要的语义。

在html中提供了很多的标签对，可以给文本只能加不同的语义。

## 编辑器
VSCODE 世界第一！

## 基本框架
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
</head>
<body>
  
</body>
</html>
```

## HTML 标签
作用：为没有样式的 HTML 增加语义

分类：容器级，文本级

### title 标签
```html
<title>Foobar</title>
```
定义标签的名称。

### h1, ... 标签
```html
<h1>Foo</h1>
<h2>Bar</h2>
<!-- ... -->
<h6>Baz</h6>
```

### 链接标签
```html
<a href="{{ dest }}" target="{{ target }}" title="{{ title }}"> Content Here </a>
```
1. `dest` 指明跳转目标，可以是相对路径，也可以是业内的元素 ID
2. `title` 指明标题，鼠标悬停展示
3. `target` 指明目标，可以在页面的 `<iframe>` 或者是 `_blank`

### 图片
```html
<img src="{{ url }}" alt="fallback text" title="hover text">
```

### 列表
#### 无序列表
```html
<ul>
  <li>foo</li>
  <li>bar</li>
</ul>
```
效果：
<ul>
  <li>foo</li>
  <li>bar</li>
</ul>

#### 有序列表
```html
<ol>
  <li>foo</li>
  <li>bar</li>
</ol>
```
效果：
<ol>
  <li>foo</li>
  <li>bar</li>
</ol>

#### 定义列表
```html
<dl>
  <dt>RPM系</dt>
  <dd>RedHat</dd>
  <dd>Fedora</dd>
  <dd>CentOS</dd>
  <dt>Deb系</dt>
  <dd>Debian</dd>
  <dd>Ubuntu</dd>
  <dt>其他派系</dt>
  <dd>Arch Linux</dd>
  <dd>Gentoo</dd>
</dl>
```
效果：
<dl>
  <dt>RPM系</dt>
  <dd>RedHat</dd>
  <dd>Fedora</dd>
  <dd>CentOS</dd>
  <dt>Deb系</dt>
  <dd>Debian</dd>
  <dd>Ubuntu</dd>
  <dt>其他派系</dt>
  <dd>Arch Linux</dd>
  <dd>Gentoo</dd>
</dl>

### DIV 和 SPAN
div 是用于分割的容器级标签

span 是访问本图片等小元素的行内标签

### 表单元素
#### 输入元素
```html
<input type="text|password|radio|checkbox" value="value" name="name">
```
需要注意的是，如果是多个input标签表达同一个组的语义时，name 需要相同

#### 选择元素
```html
<select>
  <option value="a">Linux</option>
  <option value="b">Drawin</option>
  <option value="c">BSD</option>
  <option value="d">NT</option>
</select>
```

#### 多行文本
```html
<textarea>
import std.io;
int main() {
  printf("Fuckyou, world!\n");
}
</textarea>
```

#### 按钮
```html
<input type="button|submit|reset" value="value" name="name">
```

#### 标签
```html
<label for="name">FOOBAR</label>
<input type="text" value="value" name="name">
```
