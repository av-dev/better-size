# BetterSize

Плагин для установки одинаковой высоты блоков(по максимальной). Demo: https://codepen.io/JoyZi/pen/zdKQYw

### Settings

Option | Type | Default 
------ | ---- | ------- 
elements | string | $(this).find(">div") 
childClass | string | "content"
afterChange | function | null

### Methods

Method | 
------ | ---- 
elements | string | $(this).find(">div") 
childClass | string | "content"
afterChange | function | null

### [Demo](https://codepen.io/JoyZi/pen/zdKQYw)

### Инициализация после подключения самого плагина

```javascript
$( document ).ready( function () {
     $(".current_items").betterSize({
        elements: ".item",
        childClass: "child",
        afterChange: function (el, height) {
            console.log(el, height);
        }
    });
});
```
