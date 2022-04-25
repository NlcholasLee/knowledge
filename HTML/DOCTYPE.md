# DOCTYPE
```DCOTYPE```是```document type```的简写。在```Web```设计中用来说明使用的```HTML```是什么版本。

```<!DOCTYPE html>```声明必须是```HTML```文档中的第一行，位于```<html>```标签之前。它存在的意义是阻止浏览器在渲染文档时进入混杂模式（Quirks Mode）。也就是说```<!DOCTYPE html>``这一文档类型可以确保浏览器尽可能地使用遵循规范的模式来渲染，而不是使用某些不符合规范的渲染模式。

## 混杂模式和标准模式
过去，```web```页面主要运行的两类浏览器：一个是网景的```Navigator```和微软的```IE```。后来W3C制定了Web规范之后，为了保证现有的页面可用，各大浏览器不能立马改用新规范。

于是，浏览器的厂商引入了两种模式来区别对待符合新标准的网站和旧标准的遗留网站：混杂模式（Quirks Mode）和标准模式（Standards Mode）。在过渡阶段还存在一种接近标准模式（Almost Standards Mode）。

- 混在模式，也称为怪异模式，会兼容```Navigator 4```和```IE 5```的非标准行为
- 近标准模式，会兼容少数的混杂行为，可以理解为过渡模式。
- 标准模式，只会兼容符合标准描述的行为。

## 查看页面渲染模式
```document.doctype```可以返回声明的文档类型。