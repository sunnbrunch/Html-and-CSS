# Html-and-CSS
Html

1.Intro

<!DOCTYPE html>
<html>
     <head> meta-data for the page </head>
     <body></body>
</html>

Attributes 属性 e.g. <html lang=“en-US”> lang为属性

<p></p>
<h1></h1>…<h6></h6>

2.List

<body>
     <h1> heading1 </h1>
          <ol>
               <li> list item </li>
               <li> list item </li>
               <li> list item </li>
          </ol>
</body>

heading1

- list item
- list item
- list item

Identation 缩紧 is useful to show hierarchy 层级.

<ol></ol>: ordered list

<ul></ul>: unordered list

3.Tables

<table border=1>
     <tr>
          <td>1</td>
          <td>2</td>
     </tr>
     <tr>
          <td>3</td>
          <td>4</td>
     </tr>
</table>

12
34

<tr> table row 行
<td> table data

Attribute: border=1
style=“width:100%"

4.media - hyperlinks / images

<body>
     <h2>heading2</h2>
     <a href=“http://lrnapp.com”>
          lrn website
     </a>
</body>

<body>
     <h2>heading2</h2>
     <img src=“http://dog.jpg” style=“width:100”/>
</body>

heading2
lrn website

heading2
dog img with width 100

<a></a> anhcor tag 链接
Attribute:
href (assigned a url value)

Attribute:
src: url of image
width:
height:

5.Forms

<form>
     <p>Name</p>
     <input type=“text” name=“name” value=“your name” />
     <p>Comments:</p>
     <textarea name=“comments” rows=“5” cols=“20”>Your comments</textarea>
     <p>You are:</p>
     <select>dropdown menu
          <option>cool</option>
          <option>very cool</option>
     </select>
</form>

Name:
输入框 Your name
Comment:
文本框 Your comments
You are:

[ ] cool

[ ] very cool

input type: text/password/checkbox/radio/submit

value=“your name”
placeholder=“initial value 初始值"

6.Layout - div/span     the structure of your webpage

<div style=“color:red”; id=“footer">
     <span>wow,cool</span>
</div>

<div style=“width:50px; heigth:50px; background-color:blue;”></div>

<p>
     <span style=“color:red”>I am</span>
     hip.
</p>

wow,cool

蓝色方形

I am hip.

<div> break web page into distinct sections
<span> tag allows us to choose small parts of existent HTML, usually text and style it
＊try to avoid using <span> tags

CSS

1.Intro

index.html
<head>
    <link rel=“stylesheet” type=“text/css” href=“style.css”/>
</head>
<body>
    <h1>heading1<h1>
</body>

style.css
h1 {
    color:red;
}

heading1

selector:h1
properties:color:red;

2.Selectors

h1,h2 {
    color:#8c459a;
}

* {
    color:#8c459a;
}

.classname {
    color:#8c459a;
}

a:action {
    color:#8c459a;
}

#idName {
    color:#8c459a;
}

* select - all of the HTML elements

.classname - class selector

a:action - psuedo-class伪类 链接颜色变化

#idName - id attribute applied to a single element

color: #8c459a;
color: red;
color: rgb(201,44,44);

3.Properties - used to assign styles to the HTML elements

h1 {
    font: 15px Chalkduster;
}

font: 21px Arial;
background-color: Green;
height: 30px;
width: 50px;

4.Spacing - the box model

margin-border-padding-content

margin-left,right,top,bottom
border: thickness,type,color
            1px,solid,red; 实线
            1px,dashed,red; 虚线
border-radius: 4px; 圆角半径
padding:space between the content and the border
             left,top,right,bottom

5.Positioning - containers

display: block; 锁定 纵排三个长方形
             inline-block; 横排三个正方形
             inline; 三条竖线
             none; 不显示
float: right;
         left;
position: static; 静态的（default）
               absolute; 绝对的
               relative;
               fixed;
