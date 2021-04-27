---
title: "Installation of some essentials"
permalink: /tutorial/install-essential/
---

Here are the installation of some essential softwares in Xubuntu 20.04. I hope this can be useful.

### Basic installation

To install gcc compiler and other essentials.

```shell
$ sudo apt-get update
$ sudo apt-get install build-essential
```

### LaTeX

LaTeX has been a very useful tool for me to write papers and reports. Here are the installation steps. LaTeX is usually available directly from the Debian (I used Xubuntu) software repositories and can by installed simply. However, there are variants of the installation packages. I personally would recommend the following for scientists:

```shell
$ sudo apt-get install texlive-latex-extra
$ sudo apt-get install texlive-publishers
$ sudo apt-get install texlive-science
```

The first will give a good starter pack for the environment. The second will give the standard packages for writing papers with some publishers. The third will give some useful packages for scientific writing. As a text editor, I personally like texmaker. It can be installed easily with the following command:

```shell
$ sudo apt-get install texmaker
```
