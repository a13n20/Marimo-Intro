# Marimo Intro

## How to Install

```console
pip install marimo
```
If you have Python3 then use pip3

## What is Marimo?

Marimo is a reactive, open-source Python notebook. It's very similar to Jupyter Lab, but there are some key differences in both the way it functions and the interface of the kernel.

### Reactive

Reactive refers to the kernel's ability to run all related cells automatically when a shared variable is modified.

![Example](https://github.com/a13n20/Marimo-Intro/blob/17fe6f6e87dc98be2a50d708c5c1e516f177e816/reactive.gif)

### Order doesn't matter

Cells don't need to be in any specific order. Marimo takes the order of operation into account, so any cell referencing a variable will always run after the declaration of the variable.

![Example](https://github.com/a13n20/Marimo-Intro/blob/17fe6f6e87dc98be2a50d708c5c1e516f177e816/order.gif)

### Global variable naming

Due to Marimo's reactivity, global variables **must all have unique names.** The kernel will not allow you to re-declare a variable. You can only permanently modify an existing variable by changing the original declaration value or assigning it to a new renamed variable.

![Example](https://github.com/a13n20/Marimo-Intro/blob/17fe6f6e87dc98be2a50d708c5c1e516f177e816/variable_nameing.gif)

### Explore Variables

Marimo has an "Explore Variables" tab, where you can easily reference all the variables that have been previously declared. Along with the variable name, it shows the type and value. There are also links to all the cells where the variable is used and to the cell where the variable is declared.

[Example](https://github.com/a13n20/Marimo-Intro/blob/17fe6f6e87dc98be2a50d708c5c1e516f177e816/variables.png)

### Explore Dependencies

There's an "Explore Dependencies" tab that shows which cells rely on each other. You can view these in a Mini Map, where you click on the cell and it points to any related cells, a vertical tree, and a horizontal tree.

[Example](https://github.com/a13n20/Marimo-Intro/blob/17fe6f6e87dc98be2a50d708c5c1e516f177e816/Minimap.png)
[Example](https://github.com/a13n20/Marimo-Intro/blob/17fe6f6e87dc98be2a50d708c5c1e516f177e816/VerticalTree.png)
[Example](https://github.com/a13n20/Marimo-Intro/blob/17fe6f6e87dc98be2a50d708c5c1e516f177e816/HorizontalTree.png)
