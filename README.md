LESS HTML Plugin
===

Parse LESS on HTML files containing `<style type=text/less>` tags.

Example:

```html
<!doctype html>
<title>LESS HTML Plugin test</title>
<body>
<style type=text/less>
  body {
    color: darken(red, 50%;
    p {
      color: white;
    }
  }
</style>
<p>It works!</p>
```

You now should get a warning about the missing parenthesis on line 6.

**Note:** the attribute `type=text/less` is necessary to correctly parse the
tag contents.

## Installation

    npm install -g less-plugin-html

## Usage

    lessc --html file.html


