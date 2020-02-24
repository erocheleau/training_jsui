# TRAINING COVEO/SEARCH-UI

[View the site here](https://erocheleau.github.io/training_jsui/)

## Introduction - Examples and training for the coveo/search-ui

This repository contains examples for specific use cases for the coveo search-ui. Each page is just a basic HTML page
that imports the different JavaScript released version of the search-ui and the CSS. All of the custom code is in the 
pages themselves and mostly commented with a short explanation of what it does or why it is present. Read the sub-sections
below for the different module details.

In order to use each page, have the Chrome dev tools open and load each page (or reload). Most of the pages contain 
breakpoints or debugger statements for you to explore and comments associated with the sections.

## 1. [How to use the Chrome debugger with the Coveo/search-ui framework (JSUI)](https://erocheleau.github.io/training_jsui/1debugger.html)

In this example you can see how to find elements in the HTML page and their attached Coveo modules.

You can see an example of how to use the `debugger;` JavaScript instruction to stop the execution of your code where you
want in order to explore variable values or find bugs in your scripts. 

And also how to use the step functionnalities of the Chrome debugger to go through your scripts one line at a time.

You will also encounter an error and learn how to spot the code that created this error and how to find the cause.

## 2. [Interacting with the search-ui through events in JavaScript](https://erocheleau.github.io/training_jsui/2events.html)

In this module, you will find different examples on how to attach a listener to events sent by the search-ui. Either through
native JavaScript or with the _dom_ helper packaged with the search-ui.

The different event listeners have explanations of how to access the event parameters received with each event.

There is also an example of what **not** to do to attach yourself to events.

## 3. [How to use the Chrome network tab](https://erocheleau.github.io/training_jsui/3networktab.html)

This page is mostly a placeholder in order for you to explore the Chrome network tab as part of the Chrome debugging tools.

You should be able to: 
- Easily explore the requests of a query, and what kind of data is sent with it.

- Easily explore the structure of a response from the Coveo platform when you do a search.

- Learn some tricks and interesting parts of the response when using the query debug mode.

## 4. [Coveo Analytics](https://erocheleau.github.io/training_jsui/4analytics.html)

You can explore here the structure of an analytics event sent when you do a search, a click, etc. on a Coveo search page.

(The other pages did not have an Analytics component in the page so you never saw those requests before now.)

Explore by triggering different actions and check the Chrome Network tab for the different requests sent.

## 5. [Search token generation](https://raw.githubusercontent.com/erocheleau/training_jsui/master/5searchtoken.html)

In this page you will find an example of how to generate a Search token starting with an API key that can impersonate.

This is a short example included because it is something that is often asked and a core element of how to interact with 
the Coveo platform. However, most of the code included should be executed server side as an API key with impersonate can 
be used to generate a search token with whichever identity. 

So you should generate the search token server side and then serve the page client side with the token already present.


# Other examples:

## [rest_callout_example.html](https://erocheleau.github.io/training_jsui/rest_callout_example.html)

This is a demonstration of how you can call an external REST API for each new result displayed in the Coveo search page
and add some information to the result template. This adds some pictures of dogs **after** the initial rendering of the 
results. In a real life scenario, we could have a loading gif during the call to then be replaced by the resulting information.
