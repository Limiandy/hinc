## hinc.css 一个极简的 css 框架

### 开始使用

Git 仓库下载至项目目录，然后在项目中引入

### 规范、公区类、属性

|   类名(class)   |         说明         |
|:--------------:|:-------------------:|
|   pull-right   |        右浮动        |
|   pull-left    |        左浮动        |
|    clearfix    |       清除浮动        |
|  center-block  |  设置一个居中的块元素   |
|   text-left    |     文字水平左对齐     |
|   text-right   |     文字水平右对齐     |
|  text-center   |    文字水平居中显示    |
|   align-top    |      垂直顶部对齐      |
|  align-middle  |      垂直居中对齐      |
|  align-bottom  |      垂直底部对齐      |
| text-ellipsis  |   文字超出显示省略号    |
| text-uppercase |  英文单词全部大写显示   |
|  text-middle   | 使用伪元素使内容垂直居中 |

### 页面元素

#### 按钮

基础类名 btn
样式风格 例如：default、primary 设定背景色与字体颜色，包含各伪类状态
按钮组 btns

更详细的使用，请参考 css 文件

#### 容器

**\.container** 生成一个最大宽度为1170像素的居中的容器

#### 圆形图片容器

**\.avatar** 生成一个圆形的图片框

#### 布局

<fieldset>
<legend>简单的栅格系统</legend>
<p>我们将容器进行了 12 等分，预设了 4*12 种 CSS 排列类，需要注意的是，目前栅格系统仅在页面宽度小于768像素时表现不同</p>
<div>
      <p>栅格布局规则：</p>
      <hr>
      <table>
        <tbody>
          <tr>
            <td>1.</td>
            <td>采用 <em>row</em> 来定义行，如：<em>&lt;div class="row"&gt;&lt;/div&gt;</em> </td>
          </tr>
          <tr>
            <td>2.</td>
            <td>
              采用类似 <em>col-*</em> 这样的预设类来定义一组列（column），且放在行（row）内。其中：
              <div>
                <ul>
                  <li>变量<em>*</em> 代表的是该列所占用的12等分数（如6/12），可选值为 1 - 12</li>
                  <li>如果多个列的“等分数值”总和等于12，则刚好满行排列。如果大于12，多余的列将自动另起一行。</li>
                </ul>
              </div>
            </td>
          </tr>
          <tr>
            <td>3.</td>
            <td>可对列追加类似 <em>layui-col-md-offset3</em> 这样的预设类来定义列的间距和偏移。</td>
          </tr>
          <tr>
            <td>4.</td>
            <td>最后，在列（column）元素中放入你自己的任意元素填充内容，完成布局！</td>
          </tr>
        </tbody>
      </table>
</fieldset>
<br>
<fieldset>
<legend>flex 布局</legend>
<table>
<thead>
<tr>
<td>类名（class）</td>
<td>说明</td>
</tr>
</thead>
<tbody>
<tr>
<td>media</td>
<td>指定容器为flex</td>
</tr>
<tr>
<td>media-body</td>
<td>设置flex 为 1</td>
</tr>
<tr>
<td>media-left</td>
<td>padding-right: 10px</td>
</tr>
<tr>
<td>media-right</td>
<td>padding-left: 10px</td>
</tr>
<tr>
<td>media-heading</td>
<td>margin-top: 0; margin-bottom: 5px;</td>
</tr>
<tr>
<td>media-content</td>
<td>font-size: 13px</td>
</tr>
</tbody>
</table>
</fieldset>

### 表单

|类名|说明|
|:--:|:--:|
|form-control|表单控制器（按钮）|
|form-label|label样式设定|
|form-group|组容器|
|form-inline|设置元素为内联属性|
|checkbox|复选框样式|
|help-block|添加表单说明样式|

### 表格

|类名|说明|
|:--:|:--:|
|table|设定表样基础样式|
|bordered|设定表格边框样式|
|striped|设定表格风格|
|hover|hover样式|
|table-overflow| overflow-x: auto|

### 盒模型

|类名|说明|
|:--:|:--:|
|boxes|盒容器基本样式|
|box|容器内，盒子样式|
|box-header|header盒子样式|
|box-body|body盒子样式|
|box-footer|footer盒子样式|

#### 盒子边框样式颜色
|类名|说明|
|:--:|:--:|
|default|#ddd|
|primary|#348fe2|
|info|#49b6d6|
|success|#84b547|
|danger|#ff5b57|
|warning|#f59c1a|
|inverted|#2d353c|
|transparent|#transparent|

#### 盒子风格

|类名|说明|
|:--:|:--:|
|raised|设置边框颜色、阴影|
|secondary|无外部边框，设定内部盒元素边框|

### 颜色

#### 背景色

<ul>
    <li style="background-color: #348fe2;">
        <p>#348fe2</p>
        <p>类名：bg-primary</p>
    </li>
    <li style="background-color: #49b6d6;">
        <p>#49b6d6</p>
        <p>类名：bg-info</p>
    </li>
    <li style="background-color: #84b547;">
        <p>#84b547</p>
        <p>类名：bg-success</p>
    </li>
    <li style="background-color: #ff5b57;">
        <p>#ff5b57</p>
        <p>类名：bg-danger</p>
    </li>
    <li style="background-color: #f59c1a;">
        <p>#f59c1a</p>
        <p>类名：bg-warning</p>
    </li>
    <li style="background-color: #2d353c;">
        <p style="color: #fff;">#2d353c</p>
        <p style="color: #fff;">类名：bg-inverted</p>
    </li>
</ul>

#### 字体颜色

<ul>
<li style="color: #555;">
<p>#555</p>
<p>类名：text-muted</p>
</li>
<li style="background-color: #000; color: #fff;">
<p>#fff</p>
<p>类名：text-white</p>
</li>
<li>其余与背景色对应，只是类名前缀更换为 text </li>
</ul>


## hinc-helper.css 是对 hinc.css 的扩充，里面扩充了工具式的css类名

如:

字体的粗细 f-w-*

字体的大小 f-s-*

字体的对齐方式

padding p-* p-r-* ...

marging m-* m-r-* ...

border b-* ...

border-radius r-* ...

overflow overflow-hidden ...

背景色与字体颜色的扩充
