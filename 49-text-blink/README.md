# text-blink

``` html
<style>
    @keyframes blink {
        50% {
            color: transparent;
        }
    }

    .highlight {
        animation: 1s blink 3 steps(1);
    }
</style>
<body>
<h1 class="highlight">Text Blink</h1>
</body>
```