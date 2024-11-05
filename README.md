# CV

This repo contains my CV and the code used to build it. This is a work in progress, forked from Han Zhang's.

## Main Files

* `CV_AlexFink.pdf`: The final product.
* `CV_AlexFink.rmd`: The R Markdown file used to create the PDF.
* `awesome-cv.cls`:This LaTeX template is in charge of the overall style of your CV. [vitae](https://github.com/mitchelloharawild/vitae) supports several templates and I liked this one the most. I made small tweaks to the personal info section (font size, color, & spacing) based on the original template. If you prefer the original, delete this file. 
* `apa-cv.csl`: APA 7th style from the [Zotero Style Repository](https://www.zotero.org/styles?q=id%3Aapa-cv). This file defines your citation style. In my field (Psychology), APA style is the standard. Change it to other citation styles if needed.
  `Note: I edited the `apa-cv.csl` file to support "in press" articles and to add a citation number before each reference. To display an article as "in press", in Zotero you want to leave the published date empty, add "in press" in the "Extra" field, and export it as a `.bib` file. You will find that the reference has a `note` field with the value `in press`. This will replace the year field in the generated citation. If you do not want this feature, remove the .csl file and download the original one from the Zotero Style Repository.`
* `.bib` files: I have 3 `.bib` files that separately store info for publisheded papers, in prep manuscripts, and conference presentations. You can create those `.bib` files from your reference manager (e.g., Zotero) or from scratch. It's important that you create separate `.bib` files for separate sections of your CV. 
* `lua\strong.lua`: This makes your last name in the biblographies displayed in bold font. Change it to your own last name as needed. 

Make sure to install `vitae` and `tinytex` if you haven't done so:

```
install.packages("tinytex")
tinytex::install_tinytex()

install.packages("vitae")
```
