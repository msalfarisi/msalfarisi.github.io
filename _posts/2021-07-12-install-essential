---
title: 'Installation of essentials (Xubuntu 20.04 LTS)'
date: 2021-07-12
permalink: /posts/2021/07/install-essential/
tags:
  - ubuntu
  - diy
  - science
  - en
---

This article is to document the installation of some essential softwares in Xubuntu 20.04, mainly for my reference in the future. This page will be updated time-by-time, if needed. I hope this can be useful.

### Basic installation

To install gcc compiler and other essentials.

```shell
$ sudo apt-get update
$ sudo apt-get install build-essential
```

### Installing from .deb

Other than the software repositories, .deb is also commonly used. The installation can be done from the terminal, after moving to the folder that contains the file, as follows:

```shell
$ sudo dpkg -i package_file.deb
```

### Installing from .sh

Another common installer comes in .sh format. To install this, we need to first move to the folder containing the file. Then execute:

```shell
$ chmod +x
$ bash install.sh
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

### gnuplot

Gnuplot has been a nice tool to form graphs for me. It can be installed by a simple command as follows:

```shell
$ sudo apt-get install gnuplot
```
