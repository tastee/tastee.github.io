# Tastee Parameters

In your documentation, you may want to use variable in order to switch environment or to simplify expression such as the [CSS Selectors](./what-is-css-selector.md).

For that manner, Tastee proposes to create property files (`.properties`) which content is listed as `key = value`.

For exemple :
```
Tastee.web.site = https://tastee.github.io
Tastee.menu = .button-collapse > i:nth-child(1)
```

With theses parameters, in each Tastee script using it, `Tastee.web.site` will be replaced by `'https://tastee.github.io'`. 

In order to use the property file in your script, you'll need to specify which file you want to eat using `//savor custom-parameter.properties`