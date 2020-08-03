# Chapter 1 - Node Overview

## 1.1 The Document Object Model (aka the DOM) is a hierarchy/tree of JavaScript node objects
When you write an HTML document you encapsulate HTML content inside of other HTML content. By doing this you setup a hierarchy that can be expressed as a [tree](http://dvcs.w3.org/hg/domcore/raw-file/tip/Overview.html#trees). Often this hierarchy or encapsulation system is indicated visually by indenting markup in an HTML document. The browser when loading the HTML document interrupts and [parses this hierarchy to create a tree of node objects](http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/#Parsing_general) that simulates how the markup is encapsulated.

```<!DOCTYPE html>
<html lang="en">
<head>
<title>HTML</title>
</head>
<body>
<!-- Add your content here-->
</body>
</html>
```
The above HTML code when parsed by a browser creates a document that contains nodes structrured in a tree format (i.e. DOM). Below I reveal the tree struture from the above HTML document using Opera's Dragonfly DOM inspector.

![image](http://www.domenlightenment.com/images/c1sec1.png)

On the left you see the HTML document in its tree form. And on the right you see the corresponding JavaScript object that represents the selected element on the left. For example, the selected <body> element highlighted in blue, is an element node and an instance of the HTMLBodyElement interface.

What you should take away here is that html documents get parsed by a browser and converted into a tree structure of node objects representing a live document. The purpose of the DOM is to provide a programatic interface for scripting (removing, adding, replacing, eventing, modifiying) this live document using JavaScript.

### Notes
> The DOM originally was an application programming interface for XML documents that has been extended for use in HTML documents.

------

# 第一章 - 节点概览

## 1.1 文档对象模式 (简称 DOM) 是一个层次/树结构的JavaScript节点对象

When you write an HTML document you encapsulate HTML content inside of other HTML content. By doing this you setup a hierarchy that can be expressed as a [tree](http://dvcs.w3.org/hg/domcore/raw-file/tip/Overview.html#trees). Often this hierarchy or encapsulation system is indicated visually by indenting markup in an HTML document. The browser when loading the HTML document interrupts and [parses this hierarchy to create a tree of node objects](http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/#Parsing_general) that simulates how the markup is encapsulated.

<!-- 当编写HTML文档时， 将HTML内容封装在其他HTML内容内 -->