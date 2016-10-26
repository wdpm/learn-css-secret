# text-effects

## letterpress
![letterpress](./letterpress.png)
``` html
<style>
    p {
        max-width: 300px;
        padding: .5em;
    }

    .letterpresss {
        font-size: 200%;
        background: hsl(210, 13%, 30%);
        color: hsl(210, 13%, 80%);
        text-shadow: 0 -1px 1px black;
    }
</style>
<p class="letterpresss">The only way to get rid of outdated is keeping learning.</p>
```

## stroked-text
- text-shadow

![stroked-text-by-text-shadow](./stroked-text-by-text-shadow.png)
``` html
<style>
    h1 {
        background: deeppink;
        padding: .5em;
    }

    .stroked-text {
        font-size: 350%;
        color: white;
        text-shadow: 1px -1px black, 1px 1px black, -1px 1px black, -1px -1px black;
    }
</style>
<h1 class="stroked-text">CSS</h1>
```

- svg

![stroked-text-by-svg](./stroked-text-by-svg.png)
``` html
<style>
    h1 {
        font: 350%/1 Rockwell, serif;
        background: deeppink;
        color: white;
        padding: .5em;
    }

    h1 text {
        fill: currentColor;
    }

    h1 svg {
        overflow: visible
    }

    h1 use {
        stroke: black;
        stroke-width: 6;
        stroke-linejoin: round;
    }
</style>
<h1>
    <svg width="2em" height="1.2em">
        <use xlink:href="#css"></use>
        <text id="css" y="1em">CSS</text>
    </svg>
</h1>
```

## glow
![glow](./glow.png)
``` html
<style>
    a {
        display: block;
        width:180px;
        line-height:90px;
        background: #203;
        color: white;
        transition: 2s;
        text-transform: capitalize;
        text-align: center;
        font-size: 300%;
    }
    a:hover {
        color:transparent;
        text-shadow: 0 0 .1em white, 0 0 .3em white;
    }
</style>
<a>glow</a>
```
Or use filter:
``` html
<style>
    a {
        display: inline-block;
        padding: .7em 1em;
        background: #203;
        color: white;
        transition: 1s;
    }

    a:hover {
        filter: blur(.05em);
    }
</style>
<a>glow</a>
```

## extruded
![extruded](./extruded.png)
``` html
<style>
    h1 {
        width:120px;
        line-height:50px;
        color: white;
        text-align: center;
        font-size: 200%;
        font-family: "Bitstream Vera Sans",sans-serif;
        background: hsl(0, 50%, 45%);
        text-shadow:
        1px 1px black,
        2px 2px black,
        3px 3px black,
        4px 4px black,
        5px 5px black,
        6px 6px black,
        7px 7px black,
        8px 8px black;
    }
</style>
<h1>retro</h1>
```
> [text-retro.scss](./text-retro.scss)

