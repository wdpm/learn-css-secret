# vertical-centering

![vertical-centering](./vertical-centering.png)
## base on absolute position
``` css
main {
    position: absolute;
    top: 50%;
    left: 50%;
    margin-top: -3em; /* 6/2 = 3 */
    margin-left: -9em; /* 18/2 = 9 */
    width: 18em;
    height: 6em;
}
```
Or use ``calc()`` function:
``` css
main {
    position: absolute;
    top: calc(50% - 3em);
    left: calc(50% - 9em);
    width: 18em;
    height: 6em;
}
```
Disadvantage:
- require element's width and height are both fixed value.

 Or use ``transform`` feature:
``` css
main {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
```
Disadvantage:
- sometimes we can't use absolute position
- element will be clipped if it's height is larger than viewport's.
- cause element seem to look like fuzzy if it's putted in 0.5px when in some browsers.
(use ``transform-style: preserve-3d`` to fix)

## base on vh
``` html
<style>
    main {
        width: 18em;
        padding: 1em 1.5em;
        margin: 50vh auto 0;
        transform: translateY(-50%);
        box-sizing: border-box;
        background: #655;
        color: white;
        text-align: center;
    }

    h1 {
        margin: 0 0 .2em;
        font-size: 150%;
    }

    p {
        margin: 0;
    }

    body {
        background: #fb3;
        font: 100%/1.5 sans-serif;
    }
</style>
<main>
    <h1>Am I centered yet?</h1>
    <p>Center me, please!</p>
</main>
```
>Link: [one line to implement full screen area](https://medium.com/@ckor/make-full-screen-sections-with-1-line-of-css-b82227c75cbd)
> ``` css
> .section { height: 100vh; }
> ```

## base on flexbox
``` html
<style>
    body {
        display: flex;
        min-height: 100vh;

        background: #fb3;
        font: 100%/1.5 sans-serif;
    }

    main {
        padding: 1em 2em;
        margin: auto;
        box-sizing: border-box;
        background: #655;
        color: white;
        text-align: center;
    }

    h1 {
        margin-bottom: .2em;
        font-size: 150%;
    }
</style>
<body>
<main>
    <h1>Am I centered yet?</h1>
    <p>Center me, please!</p>
</main>
</body>
```