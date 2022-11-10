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
