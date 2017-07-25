---
layout: post
title: Pandoc Experience
tags: [INLS161, pandoc, experience, text, conversion, markdown, html, docx, odt, pdf, rtf]
fullview: true
comments: true
---

**Description**

My code converts any (markdown) file to html, docx, odt, pdf, and rtf files. It takes the input file name and removes anything past the "." and renames the file using the new format of text.

**Methods**

I haven't had any prior experience with Pandoc or scripting in general before this class, so most of my code is based on outside resources. 

Converting a file to the different file types was pretty straight-forward since I used information from [here](http://pandoc.org/demos.html) and [here](https://inls161.johndmart.in/refsheets/pandoc-ref/).

Creating variables was more difficult. We went over how to create new variables in class, but I had multiple issues renaming my files. For instance, my file name was "dickinson.md," but the only way I could figure out how to rename my file resulted in "dickinson.md.'new file format'" so I had to browse Google to learn how to only use characters before the '.' symbol. I ended up using this [link](https://unix.stackexchange.com/questions/137775/how-to-extract-part-of-a-filename-before-or-before-extension), but had confusion over how to refer to my original variable. I don't quite understand why I refer to my variable without the '$' symbol, but I'm just glad that my code works -- at least I think it does.


**Product**
* [Repository](https://github.com/melissafu/melissafu-convert-documents)
* [Script](https://github.com/melissafu/melissafu-convert-documents/blob/master/melissafu-convert-docs.sh)
  * *I left some questions commented in my code*
* [Source File](https://github.com/melissafu/melissafu-convert-documents/blob/master/dickinson.md)
  * [html](https://github.com/melissafu/melissafu-convert-documents/blob/master/dickinson.html)
  * [docx](https://github.com/melissafu/melissafu-convert-documents/blob/master/dickinson.docx)
  * [odt](https://github.com/melissafu/melissafu-convert-documents/blob/master/dickinson.odt)
  * [pdf](https://github.com/melissafu/melissafu-convert-documents/blob/master/dickinson.pdf)
  * [rtf](https://github.com/melissafu/melissafu-convert-documents/blob/master/dickinson.rtf) -- the instructions said to have 5 conversions
