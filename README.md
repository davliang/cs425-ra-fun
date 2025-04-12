# CS425 Ricart-Agarwala Algorithm Simulator GUI

## Getting Started

To run the tkinter version:

```bash
uv run main.py
```

To run the PyQT6 version (recommended):

```bash
uv run main_qt.py
```

---

Get `uv` here: <https://github.com/astral-sh/uv>

## Troubleshooting

### `AttributeError: module '_tkinter' has no attribute '__file__'`

See:

- <https://github.com/matplotlib/matplotlib/issues/23074/>
- <https://github.com/astral-sh/python-build-standalone/issues/129>
- <https://github.com/astral-sh/uv/issues/6893>
- <https://github.com/matplotlib/matplotlib/commit/1c02efb55247860b1dc92aa0c5cd5c69b8b8e59d>.

---

At the moment, the only solution is to use a system installed version of Python with the correct tkinter bindings.

If you have an existing system Python install, you can find it with:

```
uv python list
```

and then select it with:

```bash
uv venv --python {version}

#Example
uv venv --python 3.9.22
```

Documentation for these commands can be found at <https://docs.astral.sh/uv/concepts/python-versions/#finding-a-python-executable>.

---

On MacOS, if you have brew installed, you can try running these command to install a compatible version of Python.

```
brew install python@3.9

brew install python-tk@3.9
```
