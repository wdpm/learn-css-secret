# text-typing

![text-typing](./text-typing.png)
``` html
<style>
    body {
        font-family: monospace, sans-serif;
    }

    @keyframes typing {
        from {
            width: 0
        }
    }

    @keyframes caret {
        50% {
            border-color: currentColor; /*avoid can't blink in old browser*/
        }
    }

    h1 {
        width: 15ch; /* text-width, ch for monospace */
        overflow: hidden;
        white-space: nowrap;
        border-right: .05em solid;
        border-right: .05em solid transparent; /* rollback style*/
        animation: typing 6s steps(15),
        caret 1s steps(1) infinite;
    }
</style>
<body>
<h1>CSS is awesome!</h1>
<script>
    function $$(selector, context) {
        context = context || document;
        var elements = context.querySelectorAll(selector);
        return Array.prototype.slice.call(elements);
    }

    $$('h1').forEach(function (h1) {
        var len = h1.textContent.length,
                s = h1.style;
        s.width = len + 'ch';
        s.animationTimingFunction = "steps(" + len + "),steps(1)";
    });
</script>
</body>

```