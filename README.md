# \<guide-color-gradient\>

Show a simple color gradient in your style guide

## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:`<paper-badge>` is a circular text badge that is displayed on the top right
corner of an element, representing a status or a notification. It will badge
the anchor element specified in the `for` attribute, or, if that doesn't exist,
centered to the parent node containing it.
Badges can also contain an icon by adding the `icon` attribute and setting
it to the id of the desired icon. Please note that you should still set the
`label` attribute in order to keep the element accessible. Also note that you will need to import
the `iron-iconset` that includes the icons you want to use. See [iron-icon](../iron-icon)
for more information on how to import and use icon sets.
Example:
    <div style="display:inline-block">
      <span>Inbox</span>
      <paper-badge label="3"></paper-badge>
    </div>
    <div>
      <paper-button id="btn">Status</paper-button>
      <paper-badge icon="favorite" for="btn" label="favorite icon"></paper-badge>
    </div>
    <div>
      <paper-icon-button id="account-box" icon="account-box" alt="account-box"></paper-icon-button>
      <paper-badge icon="social:mood" for="account-box" label="mood icon"></paper-badge>
    </div>
### Styling
The following custom properties and mixins are available for styling:
Custom property | Description | Default
----------------|-------------|----------
`--paper-badge-background` | The background color of the badge | `--accent-color`
`--paper-badge-opacity` | The opacity of the badge | `1.0`
`--paper-badge-text-color` | The color of the badge text | `white`
`--paper-badge-width` | The width of the badge circle | `20px`
`--paper-badge-height` | The height of the badge circle | `20px`
`--paper-badge-margin-left` | Optional spacing added to the left of the badge. | `0px`
`--paper-badge-margin-bottom` | Optional spacing added to the bottom of the badge. | `0px`
`--paper-badge` | Mixin applied to the badge | `{}`
@group Paper Elements
@element paper-badge

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.
