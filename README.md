# A DAY TO REACT SLIDES

## Installation

First gloabbly install [reveal-md](https://github.com/webpro/reveal-md) which is markdown files to [reveal.js](https://github.com/hakimel/reveal.js) builder.

```shell
npm install -g reveal-md
```

Then use command below to install plugins.

```shell
bower install
```

Then use the command below to launch the desired slideshow in a browser.

```shell
$ reveal-md session1.md
```

In development you can use `--watch` command for auto refresh.

```shell
$ reveal-md session1.md --watch
```


For further instructions you can visit reveal-md [documentation](https://github.com/webpro/reveal-md).

## reveal-md.json example

```json
{
  "template": "assets/template.html",
  "theme": "assets/style/black.css",
  "css": "assets/style/slide-theme.css",
  "highlightTheme": "gruvbox-dark",
  "separator": "\n---\n",
  "verticalSeparator": "\n----\n"
}

```

## reveal.json example

```json
{
  "controls": true,
  "controlsTutorial": true,
  "controlsLayout": "bottom-right",
  "controlsBackArrows": "faded",
  "progress": true,
  "slideNumber": false,
  "history": true,
  "keyboard": true,
  "overview": true,
  "center": true,
  "touch": true,
  "loop": false,
  "rtl": false,
  "shuffle": false,
  "fragments": true,
  "fragmentInURL": false,
  "embedded": false,
  "help": true,
  "showNotes": false,
  "autoPlayMedia": null,
  "autoSlide": 0,
  "autoSlideStoppable": true,
  "autoSlideMethod": "Reveal.navigateNext",
  "defaultTiming": 120,
  "mouseWheel": false,
  "hideAddressBar": true,
  "previewLinks": false,
  "viewDistance": 3,
  "parallaxBackgroundHorizontal": null,
  "parallaxBackgroundVertical": null,
  "display": "block",
  "transition": "slide"
}

```

## Custom Slide Attributes

    <!-- .slide: data-background="#be1d2c" -->

    # Slide Background Color

    ---

    <!-- .slide: data-background-image="https://facebook.github.io/create-react-app/img/logo-og.png" data-background-size="100px" data-background-repeat="repeat" -->

    ## Slide Image Background

    ---

    # Inline Styling <!-- .element: style="text-align: left" -->

    ---

    ### Fragments

        Highlight Red <!-- .element: class="fragment highlight-red" -->

        Highlight Blue <!-- .element: class="fragment highlight-blue" -->

        Highlight Green <!-- .element: class="fragment highlight-green" -->

        - Growing List Item <!-- .element: class="fragment grow" -->
        - Shrinking List Item <!-- .element: class="fragment shrink" -->
        - Fading Out List Item <!-- .element: class="fragment fade-out" -->
        - Fading In List Item <!-- .element: class="fragment fade-in" -->

    ---

    # You can give a class to element <!-- .element: class="a-class" -->
    # You can give an id to element <!-- .element: id="importantElement" -->


## Markdown Example

See [Github Mastering Markdown](https://guides.github.com/features/mastering-markdown/) guide for advanced usage.

    # First Slide Title

    * List item 1
    * List item 2

    ---

    ## Second Slide

    > Best quote ever.

    Note: speaker notes FTW!

    ---

    ## Third slide with code example

    ```js
    // Basic console prompt
    console.log('Hello World');
    ```

    ---

    ## Fourth slide with image

    Welcome to VNGRS

    ![VNGRS Dev](https://vngrs.com/assets/images/vngrs-dev-544x311.png)

## YAML Front matter

    ---
    title: Foobar
    separator: <!--s-->
    verticalSeparator: <!--v-->
    theme: solarized
    revealOptions:
        transition: 'fade'
    ---
    Foo

    Note: test note

    <!--s-->

    # Bar

    <!--v-->
