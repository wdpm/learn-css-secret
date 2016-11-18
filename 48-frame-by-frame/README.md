# frame-by-frame
- use **steps()** instead of cubic-bezier() timing-function

![frame-by-frame](./frame-by-frame.png)
``` html
<style>
    @keyframes loader {
        to {
            background-position: -800px 0;
        }
    }

    .loader {
        width: 100px;
        height: 100px;
        text-indent: 999px;
        overflow: hidden; /* Hide text */
        background: url('48-frame-by-frame/loader.png') 0 0;
        animation: loader 1s infinite steps(8);
    }

</style>
<body>
<div class="loader">Loading...</div>
</body>
```