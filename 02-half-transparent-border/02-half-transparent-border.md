# half-transparent-border

![half-transparent-border](./02-half-transparent-border.png)

``` html
<style>
    .wrapper{
        padding: 10px;
        background: #000;
        width: 120px;
    }
    .box {
        width: 100px;
        height: 100px;
        border: 10px solid hsla(0, 0%, 100%, .5);
        background: white;
        background-clip: padding-box;
    }
</style>
<div class="wrapper">
    <div class="box">Some text</div>
</div>
```