# fluid-fixed

![fluid-fixed](./fluid-fixed.png)
``` html
<style>
    /**
     * Fluid background, fixed content
     */

    body {
        margin: 0;
        font: 100%/1.5 sans-serif;
    }

    header, section, footer {
        padding: 1em calc(50% - 350px);
    }

    header {
        background: orange;
        color: white;
    }

    section + section {
        background: #eee;
    }

    footer {
        background: #333;
        color: white;
    }
</style>
<body>
<header>
    <h1>Fluid background, <br>fixed content</h1>
</header>
<section>
    <h1>Heading</h1>
    <p>Bacon ipsum dolor amet voluptate et shoulder, ipsum flank tongue exercitation commodo sed beef ribs drumstick in
        venison laborum. Laboris ut enim id drumstick, et aute esse. Consequat ad kielbasa anim pork loin turkey qui
        cupidatat drumstick doner labore. Nulla sirloin jerky do sed magna meatloaf. Ribeye ea ut elit leberkas laboris
        sausage corned beef drumstick cillum non.</p>
</section>
<section>
    <h1>Another heading</h1>
    <p>Nostrud landjaeger cillum beef cow tail cupidatat non mollit voluptate jowl. Enim sunt in, flank hamburger
        proident qui. Id aute excepteur chuck magna tempor ipsum pork chop t-bone. Frankfurter meatball pork loin beef
        et leberkas pork. Pig ball tip pancetta in.</p>
    <p>Ribeye in veniam ipsum flank. Elit incididunt t-bone proident meatball. Porchetta exercitation prosciutto sausage
        chuck ut eu brisket shank pastrami turkey sunt laboris tenderloin anim. Landjaeger do venison laboris kevin.</p>
</section>
<footer>
    <p>2015 XXXXXX (j/k, feel free to use wherever)</p>
    <p>Consectetur et t-bone pork loin. Tri-tip cupim in, spare ribs velit exercitation in. Tempor cillum fugiat, nisi
        leberkas reprehenderit anim laboris proident cow. Eu fatback kevin sint, ad shoulder in venison picanha. Sausage
        drumstick capicola, culpa boudin pork belly minim aute ipsum biltong picanha venison nulla adipisicing.</p>
</footer>
</body>
```