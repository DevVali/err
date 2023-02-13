# Err library

Err is a NekoScript library for throwing errors.

## Installation

> Please [read this](https://github.com/YuzuTheNeko/nekoscript/blob/dev/examples/libraries.md) before starting.

In your libraries folder, run:

```sh-session
git clone https://github.com/DevVali/err.git
```

## Example usage

Require the library:

```
@ Require the lib
neko err = load_file("err");

@ Init the lib in our workspace
neko err_init = err->init;
```

We throw a new error with `err->new()` function:

```
@ Require the lib
neko err = load_file("err");

@ Init the lib in our workspace
neko err_init = err->init;

if ("banana" == "banana") {
    err->new("Bananas are bananas!", true); 
};
```

First parameter is the error message (text). Second parameter is used to specify whether return the full log (bool). You can disable this feature by specifying `false`.

## The error object

Errors are stored in an object. The object looks like:

```
object!{
  name: "Error",
  message: "String wanted.",
  show_log: true
};
```

## Help

If you don't understand something in the documentation, you are welcome to ask for help in the [issues tab](https://github.com/DevVali/err/issues).
