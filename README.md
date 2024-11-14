Python highlighting in LaTeX
============================

A simple Python highlighting style to be used with LaTeX.

The package is loaded by the following line:

```tex
\usepackage{pythonhighlight}
```

It is then possible to include a Python snippet directly in the code using:

```tex
\begin{python}
def f(x):
    return x
\end{python}
```

It is also possible to include inline Python code in LaTeX with ``\pyth``:

```tex
The special method \pyth{__init__}...
```

This also works with other delimiters, for instance:
```tex
We use the dictionary \pyth|d = {"a": 1, "b": 2}|.
```

Last but not least, you can load an external Python file with:
```tex
\inputpythonfile{python_file.py}[23][50]
```
to display the contents of the file ``python_file`` from line 23 to line 50,
or with
```tex
\inputpythonfile{python_file.py}
```
to input the whole Python file.
