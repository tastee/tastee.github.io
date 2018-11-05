# What is a CSS selector ?

CSS selectors are pattern used to retrieve one or more elements within your HTML page.

Examples of CSS Selectors can be found [here](http://htmldog.com/references/css/selectors/)

## Why are they useful using Tastee ?

For the purpose of Testing HTML page, Tastee scripts need to specify on which button to click or which text to verify.

There are few techniques to retrieve dynamically en element in an HTML page like XPath or CSS Selectors.  
CSS Selectors have been chosen for Tastee since they are more commonly used and can also be given by most of the browser (read bellow)

## I don't want to learn CCS Selector, what should I do ?

You don't have to learn CSS Selectors (even if it can be useful).

Most of the Web Browser can give you the CSS Selector by right clicking on the HTML Element, Then "inspect". This will open a tool with the HTML code. On the selected HTML Element in the "Elements" tab, right click, once again and select "Copy -> Copy Slector". Then you can easily paste the copied CSS Selector in your Tastee scripts.

## Copied CSS selector are nasty, How to make Tastee Script more readable ?

Sometimes, HTML is complicated and your browser generates a wierd CSS Selector which can be big and not readable. Then you have 3 solutions :

* Either you know the developer team and ask them to add Ids and or better CSS classes
* Either you know a bit of CSS Selectors to simplify it by yourself
* Either you use [Taste Parameters](./tastee-parameters.md) : create a readable parameter which value is your CSS Selector `Connexion.button = #main > div.w3-responsive > table > tbody > tr:nth-child(16) > td:nth-child(2)`
