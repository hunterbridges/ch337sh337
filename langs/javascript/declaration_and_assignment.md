Variables in JavaScript are not strongly typed. A variable can hold any type
of value and values are always aware of their own types.

Variables are **declared** using the ```var``` keyword.

    var foo;

Variables are **assigned** using the [assignment operator](#assignment_operators)
```=```

    foo = 1;

Variables can be **initialized** by declaring and assigning in the same statement.
Variables that are not initialized have the value of ```undefined```.

    var foo = 1;

Assigning a variable that has not been declared will implicitly declare it in
**global scope**. This is valid JavaScript, but can lead to unexpected behavior.

    function setbar() {
        bar = 2;
    }

    setbar();

    console.log(bar);
    // Logs 2

**Reading** a variable that has **not been declared** will throw an [exception](#exceptions).
