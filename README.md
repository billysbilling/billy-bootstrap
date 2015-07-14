billy-bootstrap
===============

A Bower component containing a Billyfied [Bootstrap](http://getbootstrap.com/)
theme.

The colors, fonts etc. match our general design.


## Installation

Add `billy-bootstrap` to your `bower.json` file. Example:

```javascript
{
    "dependencies": {
        "billy-bootstrap": "billysbilling/billy-bootstrap#~1.0.0"
    }
}
```

Install bower dependencies:

```
bower install
```

Add an import statement to your sass file:

```sass
@import "vendor/billy-bootstrap/billy-bootstrap";
```

The [bootstrap project](https://github.com/twbs/bootstrap) is a dependency of
billy-bootstrap. So you can `require` `bootstrap.js` in your JavaScript like
this:

TODO: How to do it with broccoli?


## Design recipes

### Application layout with fixed navigation bar

Copy `images/billy-face.svg` or `images/billy-face.png` into your
project.

```html
<div class="navbar navbar-default navbar-fixed-top">
    <div class="navbar-header">
        <a href="/" class="navbar-brand">
            <img src="/path/to/billy-face.svg"/>
            billy's example application
        </a>
    </div>

    <ul class="nav navbar-nav">
        <li><a href="/a">Page A</a></li>
        <li><a href="/b">Page B</a></li>
    </ul>
</div>

<div class="container-fluid">
    <!-- Content goes here -->
</div>
```

You can replace `<img src="/path/to/billy-face.png"/>` with
`<img src="/path/to/billy-face.svg"/>`, or even use the
[ember-svg](https://github.com/billysbilling/ember-svg) helper, as in
`{{svg "billy-face"}}`.

It looks coolest if you keep the application name in all lowercase to match our
logo (in this case "billy's example application").


### Integration sites

See [billy-minuba-webapp)[https://github.com/billysbilling/billy-minuba-webapp] for an example. Check under `app/templates/application.hbs` and `app/templates/login.hbs`.
