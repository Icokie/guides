---
title: Python
---

## What is Python?

<a>Python</a> is a general purpose programming language which is dynamically typed, interpreted, and known for its easy readability with great design principles.

To know more about Python, you might want to check <a href='https://www.python.org/doc/essays/blurb/' target='_blank' rel='nofollow'>this</a> and <a href='https://docs.python.org/3/faq/general.html' target='_blank' rel='nofollow'>this</a>.

## Python 2 or Python 3

*   The two versions are similar, with knowledge of one switching to writing code for the other is easy.
*   <a href='https://wiki.python.org/moin/Python2orPython3' target='_blank' rel='nofollow'>Python 2 or Python 3</a>
    *   The 2.x branch will see no new major releases after that. 3.x is under active development <a href='https://docs.python.org/3/using/index.html' target='_blank' rel='nofollow'>...] This means that all recent standard library improvements, for example, are only available by default in Python 3.x.
    *   Python ecosystem has amassed a significant amount of quality software over the years. The downside of breaking backwards compatibility in 3.x is that some of that software (especially in-house software in companies) still doesn't work on 3.x yet.

## Installation

Most *nix based operating systems come with Python installed (usually Python 2). Replacing the system Python is not recommended and may cause problems. However, different versions of Python can be safely installed along side the system Python. See [Python Setup and Usage</a>

Windows doesn't come with Python, the installer and instructions can be found <a href='https://docs.python.org/3/using/windows.html' target='_blank' rel='nofollow'>here</a>

## Python Interpreter

The Python interpreter is what is used to run Python scripts.

If it is available and in Unix shell’s search path makes it possible to start it by typing the command `python` followed by the script name will invoke the interpreter and run the script.

`hello_campers.py`

    if __name__ == '__main__'
        print('Hello campers!')

From terminal:

    $ python hello_campers.py
    Hello campers!

"When multiple versions of Python are installed, calling them by version is possible depending on the install configuration. In the Cloud9 ide custom environment, they can be invoked like:

    $ python --version
    Python 2.7.6
    $ python3 --version
    Python 3.4.3
    $ python3.5 --version
    Python 3.5.1

## Python Interpreter Interactive Mode

Interactive mode can be started by invoking the Python interpreter with the `-i` flag or without any arguments.

Interactive mode has a prompt where Python commands can be entered and run:

    $ python3.5
    Python 3.5.1 (default, Dec 18 2015, 00:00:00)
    <a href='https://docs.python.org/3/' target='_blank' rel='nofollow'>GCC 4.8.4] on linux
    Type "help", "copyright", "credits" or "license" for more information.
    >>> print("Hello campers!")
    Hello campers!
    >>> 1 + 2
    3
    >>> exit()
    $

## The Zen of Python

Some of the principles that influenced the design of Python are included as an easter egg and can be read by using the command inside Python interpreter interactive mode:

    >>> import this
    The Zen of Python, by Tim Peters

    Beautiful is better than ugly.
    Explicit is better than implicit.
    Simple is better than complex.
    Complex is better than complicated.
    Flat is better than nested.
    Sparse is better than dense.
    Readability counts.
    Special cases aren't special enough to break the rules.
    Although practicality beats purity.
    Errors should never pass silently.
    Unless explicitly silenced.
    In the face of ambiguity, refuse the temptation to guess.
    There should be one-- and preferably only one --obvious way to do it.
    Although that way may not be obvious at first unless you're Dutch.
    Now is better than never.
    Although never is often better than *right* now.
    If the implementation is hard to explain, it's a bad idea.
    If the implementation is easy to explain, it may be a good idea.
    Namespaces are one honking great idea -- let's do more of those!

## Documentation

Python is well [documented</a>. These docs include tutorials, guides, references and meta information for language.

Another important reference is the Python Enhancement Proposals (<a href='https://www.python.org/dev/peps/' target='_blank' rel='nofollow'>PEPs</a>). Included in the PEPs is a style guide for writing Python code, <a href='https://www.python.org/dev/peps/pep-0008/' target='_blank' rel='nofollow'>`PEP 8`</a>.

## Debugging

Inline `print` statements can be used for simple debugging:

> **... often the quickest way to debug a program is to add a few print statements to the source: the fast edit-test-debug cycle makes this simple approach very effective.**
> 
> --<a href='https://www.python.org/doc/essays/blurb/' target='_blank' rel='nofollow'>Executive Summary</a>

Python also includes more powerful tools for debugging, such as:

*   logging module, <a href='https://docs.python.org/3/library/logging.html' target='_blank' rel='nofollow'>_logging_</a>
*   debugging module, <a href='https://docs.python.org/3/library/pdb.html' target='_blank' rel='nofollow'>_pdb_</a>

Just note that these exist for now.

## Hello World!

Going back to the docs, we can read about the <a href='https://docs.python.org/3/library/functions.html#print' target='_blank' rel='nofollow'>`print`</a> function, a <a href='https://docs.python.org/3/library/functions.html' target='_blank' rel='nofollow'>_built-in function_</a> of the <a href='https://docs.python.org/3/library/index.html' target='_blank' rel='nofollow'>Python Standard Library</a>.

    print(*objects, sep=' ', end='\n', file=sys.stdout, flush=False)

The built-in functions are listed in alphabetical order. The name is followed by a parenthesized list of formal parameters with optional default values. Under that is a short description of the function and its parameters are given and occasionally an example.

The <a href='https://docs.python.org/3/library/functions.html#print' target='_blank' rel='nofollow'>`print`</a> function in Python 3 replaces the <a href='https://docs.python.org/2/reference/simple_stmts.html#print' target='_blank' rel='nofollow'>`print`</a> statement in Python 2.

    >>> print("Hello world!")
    Hello world!

A function is called when the name of the function is followed by `()`. For the Hello world! example, the print function is called with a string as an argument for the first parameter. For the rest of the parameters the defaults are used.

The argument that we called the `print` function with is a `str` object or _string_, one of Python's <a href='https://docs.python.org/3/library/stdtypes.html#text-sequence-type-str' target='_blank' rel='nofollow'>_built-in types_</a>.

The `objects` parameter is prefixed with a `*` which indicates that the function will take an arbitrary number of arguments for that parameter.