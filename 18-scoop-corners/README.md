# scoop-corners

![scoop-corners](./scoop-corners.png)
``` html
<style>
    p {
        height: 100px;
        width: 200px;
        background: #58a;
        background:
            radial-gradient(circle at top left, transparent 15px, #58a 0) top left,
            radial-gradient(circle at top right, transparent 15px, #58a 0) top right,
            radial-gradient(circle at bottom right, transparent 15px, #58a 0) bottom right,
            radial-gradient(circle at bottom left, transparent 15px, #58a 0) bottom left;
        background-size: 51% 51%;/* 50% will cause white line bug on chrome*/
        background-repeat: no-repeat;
        padding: .5em;
    }
</style>

<p>Some text.</p>
```