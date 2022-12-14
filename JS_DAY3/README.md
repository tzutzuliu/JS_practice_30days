### JavaScript 型態、變數與運算子
## 整理重點
* JS若想把一個代表數字的字串剖析為數字，可以使用Number()函式
* 但JavaScript 還有 parseInt()、parseFloat()函式可以做字串剖析，不過它們無法處理 '0o'、'0b'之類的剖析
* parseInt() 方法是用於將字串轉為整數
* parseFloat() 方法用於將一個字串轉為浮點數

### 字串說明
* JavaScript 表示字串，可以使用 '', 或 "",(包括文字)，兩者在JavaScript中具有相同作用，都是產生基本型態字串，可視情況互換
* 多數JavaScript開發者的習慣，是使用單引號來建立字串，若要在字串中包括單引號，可以使用雙引號來撰寫字串
* 否則就必須使用 反斜線'或 反斜線" 來進行轉譯
* 字串使用typeof的話，會傳回'string'
* JavaScript中沒有字元型態，撰寫程式碼時，以單引號或雙引號來包刮單一Unicode字元，也是字串型態
* typeof 'A' => 'string' 
* typeof "B" => 'string'
