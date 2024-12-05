# Marimo Intro

## How to Install

```console
pip install marimo
```
If you have Python3 then use pip3

## What is Marimo?

Marimo is a reactive, open-source Python notebook. It's very similar to Jupyter Lab, but there are some key differences.

### Reactive

Reactive refers to the kernel's ability to run all related cells automatically when a shared variable is modified.

![Example](https://github.com/a13n20/Marimo-Intro/blob/17fe6f6e87dc98be2a50d708c5c1e516f177e816/reactive.gif)

Reactive also means that UI elements update automatically when using them.

You can create a slider, and it will update the output as you slide it without needing to manually run the cell.

```console
slider = mo.ui.slider(1, 22)
```
```console
mo.md(
    f"""
    {slider}
    {"##" + "🎵" * slider.value}
    """
)
```
The slider has to be defined in a separate cell from the one it's used in because of the risk of circular dependencies in UI elements. Both the slider's value and the slider's creation depend on the kernel, so the kernel can't decide the proper order of execution.

### Order doesn't matter

Cells don't need to be in any specific order. Marimo takes the order of operation into account, so any cell referencing a variable will always run after the declaration of the variable.

![Example](https://github.com/a13n20/Marimo-Intro/blob/98197ca0c553c255c03ca5a0d9145ef2f824ce8b/order.gif)

### Global variable naming

Due to Marimo's reactivity, global variables **must all have unique names.** The kernel will not allow you to re-declare a variable. You can only permanently modify an existing variable by changing the original declaration value or assigning it to a new renamed variable.

![Example](https://github.com/a13n20/Marimo-Intro/blob/57db6ad2c0b72f087493378cbbc7ed1bb3d8d0f2/variable_nameing.gif)

## Converting

You can actually convert Jupyter Lab files to Marimo files using:

```console
marimo convert file.ipynb > file.py
```
## Starting a project

To make a new or edit an existing .py file, use:

```console
marimo edit file.py
```

## Tutorial

Marimo includes a built in tutorial project that you can access by using:

```console
Marimo tutorial intro
```
