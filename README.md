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

### Order doesn't matter

Cells don't need to be in any specific order. Marimo takes the order of operation into account, so any cell referencing a variable will always run after the declaration of the variable.

![Example](https://github.com/a13n20/Marimo-Intro/blob/17fe6f6e87dc98be2a50d708c5c1e516f177e816/order.gif)

### Global variable naming

Due to Marimo's reactivity, global variables **must all have unique names.** The kernel will not allow you to re-declare a variable. You can only permanently modify an existing variable by changing the original declaration value or assigning it to a new renamed variable.

![Example](https://github.com/a13n20/Marimo-Intro/blob/17fe6f6e87dc98be2a50d708c5c1e516f177e816/variable_nameing.gif)

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
