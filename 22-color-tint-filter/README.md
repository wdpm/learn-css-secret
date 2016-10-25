# color-tint-filter
> Not full supported

![fate-zero-normal](./fate-zero-normal.png)
![fate-zero-filter](./fate-zero-filter.png)
``` html
<style>
    img {
        width: 384px;
        height: 320px;
        transition: filter 5s;
        filter: sepia(1) saturate(4) hue-rotate(295deg);
    }

    img:hover,
    img:focus {
        filter: none;
    }
</style>

<img src="22-color-tint-filter/fate-zero.jpg"/>
```