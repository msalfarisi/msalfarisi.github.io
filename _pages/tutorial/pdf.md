---
title: "Manipulation of .pdf files"
permalink: /tutorial/pdf/
---

Some useful command for manipulating .pdf files.

### Compress

There are plenty of online pdf compressor. But for safety, it is better to perform it in our own PC. Here, I use Ghostscript. It is usually already included in the linux package, just to make sure, you can try installing:

```shell
$ sudo apt install ghostscript
```

And then run the following to compress your pdf file:

```shell
$ gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/prepress -dNOPAUSE -dQUIET -dBATCH -sOutputFile=compressed_PDF_file.pdf input_PDF_file.pdf
```

### Passwording

Sometimes, password has to be made for pdf files. Here, I use pdftk. For installation:

```shell
$ sudo apt-get install pdftk
```

Then use the following command to add a password to the existing input.pdf file and output it as ouput.pdf:

```shell 
$ pdftk <input>.pdf output <output>.pdf userpw <password>
```
