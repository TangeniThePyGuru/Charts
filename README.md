<p align="center"><a href="https://erik.cat/projects/Charts"><img height="250" src="http://i.imgur.com/zylVNhI.png"></a></p>

<p align="center">
<a href="https://styleci.io/repos/69124179"><img src="https://styleci.io/repos/69124179/shield?branch=master&style=flat" alt="StyleCI Status"></a>
<a href="https://styleci.io/repos/69124179"><img src="https://img.shields.io/badge/Built_for-Laravel-orange.svg" alt="Build For Laravel"></a>
<a href="https://packagist.org/packages/consoletvs/charts"><img src="https://poser.pugx.org/consoletvs/charts/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/consoletvs/charts"><img src="https://poser.pugx.org/consoletvs/charts/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/consoletvs/charts"><img src="https://poser.pugx.org/consoletvs/charts/license.svg" alt="License"></a>
</p>

## What is Charts?

Charts is a multi-library chart package to create interactive charts using laravel. It Gives you access to
tons of different charts. Over +100 different charts and +13 different chart libraries to choose from. With this package
you can forget writing all the javascript manually and focus on your laravel project, while keeping an insane customizable chart coded in PHP. And last but not least, we support different types of charts, mathematical charts, multi-charts, they can even be
created using your eloquent models! And hey... We do support realtime stuff as well ;)

## Sample Chart

This chart is a multi bar chart using the material library.

![Charts Logo](https://i.gyazo.com/2f50ac060f699cc323741403174cec66.png)

```php
$chart = Charts::multi('bar', 'material')
            // Setup the chart settings
            ->title("My Cool Chart")
            // A dimension of 0 means it will take 100% of the space
            ->dimensions(0, 400) // Width x Height
            // This defines a preset of colors already done:)
            ->template("material")
            // You could always set them manually
            // ->colors(['#2196F3', '#F44336', '#FFC107'])
            // Setup the diferent datasets (this is a multi chart)
            ->dataset('Element 1', [5,20,100])
            ->dataset('Element 2', [15,30,80])
            ->dataset('Element 3', [25,10,40])
            // Setup what the values mean
            ->labels(['One', 'Two', 'Three']);
```

## Important News

Charts is not in a good state now. Managin new features is a pain and maintain such a long library is painfull. As I'm currently under some free time, I decided to give it a spin, creating the next release of charts as a total rework of the library, from the ground up. The next version will support fewer libraries (at least at the start) and fewer features (no realtime, etc) at the beggining, but will give everyone 100% customization under ANY supported library. That means, yes, you'll finally be able to do what you want and make your charts look like you want. It will be also in a more laravel-releated code style, coding it with classes (more like you code mail / notifications).

Due to this information, I won't accept any new PR and all issues will be formally closed once the new version is live.

**TL;DR;**: The library will be refactores, from the group up, issues and PR closed until the new one is released. This is a major breaking change.

## Comming Soon

<p align="center">
    <img src="https://image.prntscr.com/image/YCJjBypAQpu86PL-UiY_qA.png">
</p>

Simplistic charts, perfect to fit in places where no extra information is needed. Only chartjs will be supported this time!

Remember, no axis, no labels, no tooltips!

## Support me on patreon

You can support me on patreon if you liked, enjoyed or use any of my libraries on github, this really keeps me up for fixing new problems and adding new features.

<p align="center">
<a href="https://www.patreon.com/ErikCampobadal"><img src="https://i.imgur.com/ZTLPSt5.png"></a>
</p>

## Documentation

<p align="center">
<a href="https://erik.cat/projects/Charts/docs/5"><img src="http://i.imgur.com/47WnADd.png"></a>
</p>

## Supporters

The official list of supporters

-   [TimS - Developer from Finland](https://twitter.com/tdawgpharaoh)

## License

```
MIT License

Copyright (c) 2016 Erik Campobadal

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

```
