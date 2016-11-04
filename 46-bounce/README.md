# bounce

``` html
<style>
    @keyframes bounce {
        60%, 80%, to {
            transform: translateY(400px);
            animation-timing-function: ease;
        }
        70% {
            transform: translateY(300px);
        }
        90% {
            transform: translateY(360px);
        }
    }

    .ball {
        animation: bounce 3s cubic-bezier(.1, .25, 1, .25);
    }
</style>
```