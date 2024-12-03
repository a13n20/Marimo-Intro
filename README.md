# Marimo Intro

## How to Install

```console
pip install marimo
```
If you have Python3 then use pip3

## What is Marimo?

Marimo is a reactive, open-source Python notebook. It's almost exactly like Jupyter Lab, but there are some key differences.

### Reactive

Reactive refers to the kernel's ability to run all related cells automatically when a shared variable is modified.

![Example](https://github.com/a13n20/Marimo-Intro/blob/17fe6f6e87dc98be2a50d708c5c1e516f177e816/reactive.gif)

### Order doesn't matter

Cells don't need to be in any specific order. Marimo takes the order of operation into account, so any cell referencing a variable will always run after the declaration of the variable.

![Example](https://github.com/a13n20/Marimo-
Intro/blob/17fe6f6e87dc98be2a50d708c5c1e516f177e816/order.gif)
