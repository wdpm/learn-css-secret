# multiple-borders

- box-shadow

![](./03-multiple-borders(box-shadow).png)
``` html
<style>
    .box {
        margin: 20px;
        width: 100px;
        height: 50px;
        background: yellowgreen;
        box-shadow: 0 0 0 10px #655,
                    0 0 0 15px deeppink,
                    0 2px 5px 15px rgba(0, 0, 0, .6);
    }
</style>

<div class="box"></div>
```

- outline

![](./multiple-borders(outline).png)
``` html
<style>
    .box {
        width: 200px;
        height: 100px;
        background: #655;
        outline: 2px dotted white;
        outline-offset: -10px;/* use negative offset*/
    }
</style>

<div class="box"></div>
```
