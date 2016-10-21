# extended-bg-position

![extended-bg-position](./extended-bg-position.png)

### 1.background-position
``` html
<style>
    .box {
        width: 200px;
        height: 100px;
        background: url("./avatar.svg") no-repeat bottom right #619dc2; /*bottom right: backing out*/
        background-position: right 20px bottom 10px;
        padding: 10px;
    }
</style>

<body>
<div class="box"></div>
</body>
```

### 2.background-origin: content-box
``` css
padding: 10px;
background: url("./avatar.svg") no-repeat #619dc2 bottom right; /* or 100% 100% */
background-origin: content-box;
```

### 3.calc()
``` css
background-position: calc(100% - 20px) calc(100% - 10px);
```

