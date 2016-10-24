# diamond-images

![diamond-images](./diamond-images.png)

``` html
<style>
    .picture {
        margin: 80px;
        width: 200px;
        height: 200px;
        transform: rotate(45deg);
        overflow: hidden;
    }

    .picture > img {
        width: 200px;
        height: 200px;
        max-width: 100%;
        z-index: -1;
        transform: rotate(-45deg) scale(1.42);/* sqrt(2)*/
    }
</style>

<div class="picture">
    <img src="16/icon.jpeg" alt="..."/>
</div>
```