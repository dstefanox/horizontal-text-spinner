[![Build Status](https://travis-ci.org/dstefanox/horizontal-text-spinner.svg?branch=master)](https://travis-ci.org/dstefanox/horizontal-text-spinner)

# horizontal-text-spinner

An element which shows text which slides-in from the left or the right and gets out of the area by slidding-out to the left or to the right.

## Demo

To get better idea about this element, check [live demo](http://dstefanox.github.io/horizontal-text-spinner/components/horizontal-text-spinner)


## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install horizontal-text-spinner --save
```

## Usage

1. Import  Element:

    ```html
    <link rel="import" href="bower_components/horizontal-text-spinner/horizontal-text-spinner.html">
    ```

2. Place it on the page:

    ```html
    <horizontal-text-spinner id="spinner" content="Initial text">
    </horizontal-text-spinner>
    ```

3. Spin some new text into component from left/right:

    ```js
    var el = document.getElementById("spinner");
    el.spinLeft("Spinning left!")
    el.spinRight("Spinning right!")
    ```

## Customization

Element uses absolute positioning of internal elements, so it is important understand how to style it.
By default, element has fixed height of 36 pixels, which corresponds to line height (this allows text to be centered verticaly within element).
To keep text verticaly centered within element, keep line height and element height same values.

The following custom properties are available for styling:

Custom property | Description | Default
----------------|-------------|----------
`--horizontal-text-spinner-font-size` | Size of the font used to show text within element | `24px`
`--horizontal-text-spinner-line-height` | Text line height. Keep it same value as element height to make text vertically centered | `36px`
`--horizontal-text-spinner-height` | Height of the element | `36px`
`--horizontal-text-spinner-color` | Text color | `black`
`--horizontal-text-spinner-background-color` | Background color of the element | `{}`


## License

[MIT License](http://opensource.org/licenses/MIT)
