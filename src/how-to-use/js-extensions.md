# Extend instructions using Javascript

Tastee is based on Javascript (source written in Typescript can be found on [Github](https://github.com/tastee)).

## Selenium API

[Selenium Webdriver](https://www.seleniumhq.org/projects/webdriver/) is used to control the browser and execute Tastee lines which are translated into Javascript code.

Therefore, within your instruction, you can use native javascript and part of the Selenium JS API to customize Tastee's behaviour and extends your scripts.

Selenium JS API is exposed directly with :

* `driver` which is build directly from the Selenium API regarding the browser name 
* `By` equivalent to `selenium.By`
* `Key` equivalent to `selenium.Key`
* `until` equivalent to `selenium.until`
* `Actions` equivalent to `selenium.ActionSequence`
* or directly `selenium`

More on Selenium JS API is avalaible [here](https://seleniumhq.github.io/selenium/docs/api/javascript/index.html)

Here is an example extracted from the common BSL instruction :

```
Check that $name is equal to $value:
    - var element = driver.findElement(By.css($name));
    - element.getText().then(function(text) {
        assert.equal(text, $value, 'the '+ $name + ' element contains '+text);
    });
```

If you think your instructions could be shared with the other Tastee users, please don't hesitate to create a new [pull request](https://github.com/tastee/tastee-examples/pulls) in [tastee-example](https://github.com/tastee/tastee-examples).

## Debugging

Tastee-ui is build on top of [Electron](https://electronjs.org/) and therefore executed with Chromium. We made the choice to allow anyone to access Chrome Developpers tools within Tastee-ui by using `F12` or `CTRL + MAJ + I`.  

So any element you use to use to debug your Javascript Application in Chrome is available, you can then use `console.log`, for example, if you wish so.
