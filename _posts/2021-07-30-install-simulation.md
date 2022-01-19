---
title: 'Installation of useful simulation tools (Xubuntu 20.04 LTS)'
date: 2021-07-30
permalink: /posts/2021/07/install-simulation/
tags:
  - simulation
  - diy
  - science
  - en
---

This post is to document the installation steps of my important simulation tools, mainly as a reference for myself in the future.

### KiCad

KiCad has been very helpful for me to design electrical circuits. The installation can be performed by adding its PPA address through the terminal as follows:

```shell
sudo add-apt-repository --yes ppa:kicad/kicad-6.0-releases
sudo apt update
sudo apt install --install-recommends kicad
sudo apt install kicad-demos
```

The last line is optional to add some demo projects. The above steps will install the full version of KiCad including many packages. It reduces the hassle to install default libraries and symbols, however, require some disk space (and installation time).

### FreeCAD

FreeCAD is a useful tool to make a 3D design. It is usually available directly from the Debian (I used Xubuntu 20.04) software repositories and can by installed by:

```shell
sudo apt-get install freecad
```

### SALOME

I use SALOME to form mesh from the 3D design for simulations. The installation can be performed by downloading suitable installer from their [official homepage](https://www.salome-platform.org/downloads/current-version/download-page). For instance, I used the Universal Linux Binary (SALOME 9.7.0) installer for my Xubuntu 20.04 environment. Installation was performed by extracting the downloaded package and the program can be run as follows:

```shell
tar xfz SALOME-9.7.0-MPI.tar.gz
cd SALOME-9.7.0-MPI
./salome
```

### Elmer

Elmer is a quite powerful multipurpose simulation tool for solids. The installation can be performed by adding its repository as follows:

```shell
sudo add-apt-repository ppa:elmer-csc-ubuntu/elmer-csc-ppa
sudo apt-get update
sudo apt-get install elmerfem-csc
```

If you need a graphical user interface, it can be installed through the following command similarly, having the repository added:

```shell
sudo apt-get install elmerfem-csc-eg
```

### OpenFOAM

For fluids, OpenFOAM can be used instead. The installation process can be performed by adding its repository as follows:

```shell
sudo sh -c "wget -O - https://dl.openfoam.org/gpg.key | apt-key add -"
sudo add-apt-repository http://dl.openfoam.org/ubuntu
sudo apt-get update
sudo apt-get install openfoam8
```

### ParaView

ParaView is a useful tool to visualize and interpret your simulation results. It is usually available directly from the Debian (I used Xubuntu 20.04) software repositories and can by installed by:

```shell
sudo apt-get install paraview
```
