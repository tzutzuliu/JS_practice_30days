# JS30-DAY1_JavaScript

## 養成好習慣
* 將 JavaScript 程式碼集中寫在 .js 檔案中是好習慣是"best practice"
* 【建議】
>> 1.可以將 JS 程式碼和 HTML 分開，才不會雜在一起很難閱讀和查找。
   2.不同邏輯的 JavaScript 程式碼，建議可以分開不同的檔案編寫和儲存，方便維護和管理。
   3.瀏覽器在下載 JS 檔案後，會自動暫存 (cache) 一份在客戶端電腦中，之後就不需要再重複下載一次，加快之後的網頁載入速度。

## 工具
* 線上練習JS >>JSFiddle 

## Important note 
### addEventListener()
* 為了讓整個網頁監聽鍵盤按下的事件，使用了 window 綁定 keydown 事件
```javascript=
window.addEventListener('keydown', function(){});
```
* addEventListener 方法可以用來綁定元素的事件處理函數，第一個參數eventType 是事件名稱，第二個參數listener 是事件處理函數。 

========================================================================
* syntax
```javascript=
document.addEventListener(event, function, useCapture)
```
* event
  * 可以是所有HTML DOM事件
  * EX: onclick、oncontextmenu、onmousedown、onmousemove、onmouseover、 onmouseup..

* function 
  * 指定事件一定要觸發時執行的函數。

* useCapture
  * 可以是 true / false


## Element object attribute & method
### Element object
*  DOM Element Object .id =>element的id
*  DOM Element Object .nodeName=>element的nodename
*  DOM Element Object .innerHTML (寫法如下)

* syntax
```javascript=
document.getElementById("demo").innerHTML = "I'm Tzutzu";
```
```javascript=
let html = document.getElementById("myP").innerHTML;
```
*  DOM Element Object .textContent=>element.textcontent

* syntax
```javascript=
element.textContent = "I'm Tzutzu";
```
```javascript=
let text = element.textContent;
```
========================================================================


## JavaScript DOM Node Properties (DOM 節點物件的屬性)
### Node.nodeType 屬性
* nodeType 屬性可以取得該節點的類型，像是 elements (元素節點), text (文字節點) 或 comments (註解節點)。
* DOM 還有這些常數,就是 (Node type constants)，幫助判斷節點類型。

  * Node.ELEMENT_NODE
  =>表示 HTML 元素 (Element) 節點

  * Node.TEXT_NODE
  =>表示文字 (Text) 或屬性 (Attr) 節點

  * Node.COMMENT_NODE
  =>表示註解節點 (Comment)

  * Node.DOCUMENT_NODE
  =>表示根節點 (Document)

  * Node.DOCUMENT_TYPE_NODE
  =>表示 DocumentType 節點，像是<!DOCTYPE html>的文件概念意思

  * Node.DOCUMENT_FRAGMENT_NODE
  => 表示 DocumentFragment 節點

========================================================================

* NodeList 物件是節點的集合，可藉由 Node.childNodes 屬性或 document.querySelectorAll() 等方法取得。 
* NodeList 雖然有著與陣列相似的特性，但不是陣列，所以也不會有陣列相關的 method 可以使用 (如 map、filter 等)。
