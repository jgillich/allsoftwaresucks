jQuery is well known for solving all problems related to web development. Just
by including it, your site becomes compatible with browsers like Netscape,
MOSAIC and its inferior successor Internet Explorer. We also provide you with
jQuery mobile, a framework to turn your web site into an app that works great on
mobile devices like the Nintendo 3DS. Because all jQuery mobile sites look and
feel exactly the same, browsers only have to render them once, making them
blazingly fast. And there's jQuery UI, although we are still exploring what it
could be used for.

Today, we introduce the next generation of the jQuery platform: The jQuery
Browser. It is a web browser written using the jQuery programming language. How
does it differ from existing web browsers, like the MOSAIC we all use and love?
The jQuery browser is not just another browser, it features a completely
redesigned web platform. We believe that many web sites are being held back by
legacy technologies like Java and CSS.

## A better way to style sites

Many web sites use CSS. It's from the 90s, therefore I don't need to tell you
its design is inherently flawed. That is why we are introducing jQuery Style
Sheets ($SS), a language to define the looks of your site in a very concise
way:

```js
$SS('body', function(body) {
  $SS(body).style('background-color', 'black');

  $SS(body).find('a', function(a) {
    $SS(a).style('color', 'jQuery');
  });
});
```

As you can see, we've also added the `jQuery` color.

## A new browser environment

We've completely redesigned the jQuery language environment. The global root
object formerly known as `window` has been renamed to `$`, all jQuery functions
are now directly accessible from the root. To avoid collisions with legacy code,
all functions have been prefixed with `$`, where you previously wrote `$.each`,
you can now simply write `$each`. But there's more! Although jQuery already
solves all problems and always has been, we added many modules to make sure
jQuery continues to solve all problems in the future, these include:

* $getCoffe: An extended version of the existing $makeCoffee, it now
  automatically transfers coffee to your desk so you can keep coding.
* $wat: Whenever you have no idea what you're doing, call this to automatically
  post a question on Stack Overflow. We've been shipping this to our users from
  India for years, but now we're making it available to everyone.
* $solveProblem: The core of jQuery, now part of our public API. You pass a
  problem description, and jQuery solves it for you. Note that this is only for
  advanced users that are able to express their problems (otherwise, see $wat).

## A disruptive user interface

Now that we've talked about the internals of our new jQuery Browser platform,
lets look at the user interface. We compared all browsers and how they developed
over time. While the first browsers only had a very minimal interface, the
current browser generations have a lot of toolbars and extensions that distract
from what actually matters: the jQuery-powered content. So here is the result
of years of research by jQuery UI engineers:

![jQuery Browser](/images/jquery-surf.png)

Impressive, right? But save your applause for later, I first need to tell you
about the revolutionary way to control the browser: your keyboard! There are two
modes, input mode and control mode. In input mode, you navigate web pages and
enter form values. In control mode, you have the full power of jQuery at your
fingertips. Bookmarking a web site becomes as easy as hammering ESC 2-5 times
and then typing:

```js
:$bookmark($.location.url);
```

You may clap now.
