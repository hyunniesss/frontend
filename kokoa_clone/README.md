# lecture summary

browser is made by text
for example, [koreatimes.co.kr](https://www.koreatimes.co.kr/?edition=south*korea)

folder/file name should be all lower case

## HTML
* Hyper Text Markdown Language
* for content

* html file have ".html" extension file name
* browser understand html and css file. so, open it from browser
* html doesn't tell error on your page
* open tag, write something, close tag
* example,
  * h1~h6 meaning header,
  * ul with li meaning unordered list and list,
  * ol with li meaning ordered list and list,
  * a means anchor, going to another website, use with attribute `href`
  * img is self-closing tag, use with attribute `src`, no content
* html start with "<!DOCTYPE html>" means this document type is html
* all tags have own attributes
* id attribute is unique key

* html semantic tag from div id, makes reading html files easier
    * semantic tag can replace div, header tag means `<div id="header">`
    * main tag means `<div id="main">`

* [html tag MDN](https://developer.mozilla.org/ko/docs/Web/HTML/Reference/Elements)

## CSS
* **C**ascading **S**tyle **S**heets
* should be used <b style="color: red;">with HTML</b>
* makes browser's design
* in html file, `<style></style>` inside `<head>` : inline css
* separate from html file, `<link ref="*.css" rel="stylesheet">` inside `<head>` : external css
* point the element, make design
    ```
    tagname {
        propertyname: value;
    }
    ```
* from top to bottom ordered style
* all tags are block type(nothing next to element) or inline type(something next to element)
* `display: inline` has no height and width
* `margin`: 경계 바깥의 공간(space outer of border)
    * `margin-top` and `margin-bottom` don't work at inline element
    ```
    margin: all
    margin: topbottom leftright
    margin: top leftright bottom
    margin: top right bottom left
    ```
* [collapsing margins](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_box_model/Mastering_margin_collapsing)
    * 자식 엘리먼트의 경계가 부모 엘리먼트의 경계와 만날 떄 발생, 두 엘리먼트의 margin이 합쳐지면서 부모한테 먹힘
* `padding`: 경계 안쪽의 공간(spane inner of border)
* `border`: inline, block element 전부 적용되는 엘리먼트 경계선 디자인
    ```
    border: size style color
    ```
    * `border-radius`: 경계 꼭지점의 둥글기
* `#id`: tag에 id값을 추가함으로써 각 tag를 unique하게 만들어 css에서 단 하나의 값으로 지정
* `.class`: tag에 class값을 추가해서 같은 classname을 가진 엘리먼트들에 같은 css를 적용
    * class는 공백을 기준으로 여러개를 동시 적용할 수 있음 `<div class=classname1 classname2 ...>`
* `display: inline-block` 
    * can make inline element with block attributes like width, height, etc.
    * **doesn't support responsive design**
* `flexbox`: inline-block 의 단점 보안
    * talk to the parent, not to the children elements
    ```
    parent { 
        display: flex; // parent is in control of their children
        justify-content: // position of children, calcuate automatically, works horizontally(수평, main axis, 주축)
        align-items: // vertically(수직, cross axis, 교차축)
    }
    ```


## JavaScript

* brain of website
* if event occured by user, it works by javascript

## VSCode extension

* VSCode is just text editor like 메모장
* Community Material Theme
* Material Icon Theme
