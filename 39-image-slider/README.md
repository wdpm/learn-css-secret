# image-slider

![image-slider](./image-slider.png)
``` html
<style>
    .image-slider {
        position: relative;
        display: inline-block;
    }

    .image-slider > div {
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        width: 50%;
        overflow: hidden;
    }

    .image-slider img {
        display: block;
        user-select: none;
    }

    .image-slider input {
        position: absolute;
        left: 0;
        bottom: 10px;
        margin: 0;
        filter: contrast(.5);
        mix-blend-mode: luminosity;

        width: 50%;
        transform: scale(2);/* 50% * 2 = 1,for fitts' law */
        transform-origin: left bottom;
    }
</style>

<div class="image-slider">
    <img src="39-image-slider/my_icon_grey.jpg" alt="Before"/>
    <img src="39-image-slider/my_icon.jpg" alt="After"/>
</div>

<script>
    function $$(selector, context) {
        context = context || document;
        var elements = context.querySelectorAll(selector);
        return Array.prototype.slice.call(elements);
    }

    $$('.image-slider').forEach(function (slider) {
        var div = document.createElement('div');
        var img = slider.querySelector('img');
        slider.insertBefore(div, img);
        div.appendChild(img);

        var range = document.createElement('input');
        range.type = 'range';
        range.oninput = function () {
            div.style.width = this.value + '%';
        };
        slider.appendChild(range);
    });
</script>
```
