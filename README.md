

# Create Link

Source code of [Create Link](https://chrome.google.com/webstore/detail/create-link/gcmghdmnkfdbncmnmlkkglmnnhagajbm).

# Filters

This feature is basically for developers.

You can define a Filter for each format which is applied to the text generated by Create Link.
Filters are defined with JavaScript code which takes generated text and returns text.

|Name|Format|Filter|
|----|------|------|
|HTML|<a href="%url%">%title%</a>|return s + ' ' + (new Date().toJSON().substring(0, 10))|

The configuration above gives you following text.

```html
<a href="http://example.com/">Example Domain</a> 2017-03-14
```

# Development

## Build

webpack is used for building application code. Run

```sh
make webpack
```
to watch the changes and generate js files.

## Test

```sh
make test
```

