# hit-area

![hit-area](./hit-area.png)
``` html
<style>
    button {
        position: relative;
        padding: .3em .5em;
        background: #58a;
        border-radius: 50%;
        border: 1px solid rgba(0, 0, 0, .3);
        box-shadow: 0 .1em .2em -.05em rgba(0, 0, 0, .5);
        color: white;
        font: bold 150%/1 sans-serif;
        cursor: pointer;
    }

    button::before {
        content: '';
        position: absolute;
        top: -10px;/* 10px larger than the host element */
        right: -10px;
        bottom: -10px;
        left: -10px;
    }
</style>
<button>+</button>
```
