![Skripio logo](/logo/logo-128.svg)
# What is skripio?
**Skripio** is a set of UI **components** designed and built for [1C:Enterprise](https://www.1ci.com/developers/) platform. 

These components allow [1C:Enterprise](https://www.1ci.com/developers/) developers to implement UI elements in [1C:Enterprise](https://www.1ci.com/developers/) forms that are not available as a part of the default platform toolkit.  

**Skripio components** are intended to help [1C:Enterprise](https://www.1ci.com/developers/) developers enrich user experience of their application through implementing native web technologies and open source libraries.

**Skripio components** are fully functional bundles that can be easily added into [1C:Enterprise](https://www.1ci.com/developers/) project with zero [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) code.

# Why skripio?

On _September 20th 2018_ **1C** [announced](https://wonderland.v8.1c.ru/blog/perevod-klientskikh-prilozheniy-dlya-windows-na-ispolzovanie-webkit-optimizatsiya-otobrazheniya-html/) webkit support as platform HTML generating engine. 

This platform feature technically allows [1C:Enterprise](https://www.1ci.com/developers/) developers to create custom UI element with help of modern technologies such as: `HTML5`, `CSS3`, `JavaScript ES6`.

However, such component development in most of the cases will require `HTML`, `CSS` or [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) coding to be done by developer which drastically extends development time frames.

Here are a few 1C - webkit limitations that require coding outside of [1C:Enterprise](https://www.1ci.com/developers/) platform environment:

- **Primitive types in function calls**. When calling a JS function or method from [1C:Enterprise](https://www.1ci.com/developers/) only primitive types can ba passed. Passing a collection of any kind results in `undefined` value upon argument receiving.
- **No JS prototype chain support**. If there is an object instantiated of a class that inherits another class then object's methods are located in it's parent object. In such case those methods are not accessible out of [1C:Enterprise](https://www.1ci.com/developers/) environment.
- **No async code support**. It is impossible to pass a [1C:Enterprise](https://www.1ci.com/developers/) method or procedure as a callback to [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) function. If [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) function or method requires a callback passed to it as an argument, that function can not be used directly out of [1C:Enterprise](https://www.1ci.com/developers/) environment. Going forward, no native [asynchronous JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Introducing) code is accessible out of [1C:Enterprise](https://www.1ci.com/developers/) platform, such as [Promises](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Using_promises) and [async/await functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function). A [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) wrapper is required to organize that type of interaction.
- **No asset tree support**. It is impossible to reference any assets located in a folder on server like in a conventional project. Therefore we either have to compile all our assets in one bundle or reference them with http links.

The aforementioned list of limitation have facilitated skripio components to emerge.

# Getting started with skripio

Step-by-step guide to implement skripio component in a [1C:Enterprise](https://www.1ci.com/developers/) project:  
TODO:

# Contribute

[Contribute 1C](https://github.com/fmecgroup/skripio-intro/blob/master/CONTRIBUTE1C.MD) - Guide to contribute to [1C:Enterprise](https://www.1ci.com/developers/) codebase.  
[Contribute JS](https://github.com/fmecgroup/skripio-intro/blob/master/CONTRIBUTEJS.MD) - Guide to contribute to [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) codebase.
