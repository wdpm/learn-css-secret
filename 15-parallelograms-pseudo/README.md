# parallelograms-pseudo

![parallelograms-pseudo](./parallelograms-pseudo.png)
``` html
<style>
    .button {
        position: relative;
        display: inline-block;
        padding: .5em 1em;
        margin: 1em;
        background: transparent;
        color: white;
        text-transform: uppercase;
        font: bold 200%/1 sans-serif;
    }

    .button::before {
        content: ''; /* To generate the box */
        position: absolute;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
        z-index: -1;
        background: #58a;
        transform: skew(-45deg);
    }
</style>

<div class="button">click me</div>
```
