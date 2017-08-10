### 新增标签
1. `<header>`: 用于网页首部
2. `<footer>`: 用于网页底部
3. `<article>`: 用于文章
4. `<section>`: 用于章节
5. `<aside>`: 用于边栏
6. `<nav>`: 用于导航条

### 微元素
```html
<time datetime="2017-08-07T14:28">文章发表于2017年8月7号下午14点28分</time>
<hgroup>
  <h1>我是主标题</h1>
  <h2>我是副标题</h2>
</hgroup>
<address>Asia, the Earth, the Galaxy</address>
<figure>
    <img src="../imgs/boy/timg%20(15).jpg" alt="">
</figure>
<figcaption>My Avatar</figcaption>
```

### 表单元素
#### input
增加类型：image, hidden, email, url, tel, number, range, time, date, week, month,datetime-local, datetime, color, search, file
增加属性：maxlength, readonly, disabled, required, placeholder, autofocus, autocomplete, accesskey

#### select
增加属性 multiple 多选

#### datalist
参考 select，类似

#### form
新增：fieldset
```html
<fieldset>
  <legend>基本信息</legend>
  <section>
    <p>
      <span>用户名：</span>
      <input type="text" name="username" maxlength="5" accesskey="q" autocomplete="off">
    </p>
    <p>
      
      <input type="radio" name="gender" >男
      <input type="radio" name="gender">女
      <input type="radio" name="gender" checked>你猜
    </p>
    <p>
      <span>密码：</span>
      <input type="text" name="password" required>
    </p>
  </section>
</fieldset>
```

#### 媒体标签
`<video>`, `<audio>`
