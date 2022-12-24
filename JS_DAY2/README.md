### JS30-Day2-CSS + JS Clock
## 整理 CSS 屬性重點
1. transform-origin: 設定物件變形的起始點
    共有三個參數，分別是控制 x 軸(左到右)，y 軸(上到下)，z 軸的起始位置
    ```css
    transform-origin(0, 0); 
    ```
    * 註：是從物件的左上角開始

2. transform: 設定物件的變形種類
    常用包括translate(位移)、scale(縮放)、rotate(旋轉)、skew(傾斜)等，還有結合 scale、skew、translate 的 matrix(scale X, scale Y, skew X, skew Y, move X, move Y)
    
3. transition-timing-function: 設定物件不同變形期間的變形速度
    ```css
    transition-timing-function: cubic-bezier(.29, 1.01, 1, -0.68);
    ```

### Document.querySelector syntax

```css
    element = document.querySelector(selectors);
```

### Transition 
* transition-property:指定要轉換的CSS屬性
* transition-duration:轉換需要的時間，預設0，單位為s或ms
* transition-delay:延遲多久轉換，預設0，單位為s或ms
* transition-timing-function:轉換時的速度曲線，預設ease
==================================================================

### setInterval() 方法
* syntax
```javascript=
setInterval(function(){ alert("Hello tzu"); }, 1000); 
```
* 每1秒（1000 毫秒）弹出 "Hello tzu" 的意思

* syntax
* setInterval(code, milliseconds);
* setInterval(function, milliseconds, param1, param2, ...)
==================================================================