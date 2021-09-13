# Description

Please follow this guide if you'd like to create your own [1C:Enterprise](https://www.1ci.com/developers/) **component** codebase that implements [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) codebase of a **component** or if you'd like to contribute to an existing [1C:Enterprise](https://www.1ci.com/developers/) **component** codebase.

# Skripio JS concepts

The following key concepts that are guaranteed to be supported in [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) codebase of every **skripio** component.

- Each **component** is guaranteed to be supplied as a single [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) bundle that contains all assets and dependencies in one `HTML` file.
- Each **component** is supplied with a set of **global init functions** that MUST be called to instantiate a component object.
- Each **component** is guaranteed to have one global `execSkripioMethod` function that executes given method of a given component with given method arguments.
- `execSkripioMethod` function is guaranteed to accept 3 arguments:
  - `component` - name of the component object.
  - `method` - method name of the component object to execute.
  - `args` - **String** that contains serialized **Array** of `method` **Arguments**. Arguments in array MUST follow order defined in requested method.
- Each **component** method will return result or response in 2 ways:
  - `sync` responses - returned as regular responses to JS function calls.
  - `async` responses - returned by generating **click** event on a `HTML` **div** element.

# Quick steps

- Add all contents of component bundle to html page on 1C form.
- Instantiate a component with given name.
- Use `execSkripioMethod` to call component methods.
- TODO: