# RprojectDemo

This demonstration shows how to organize a research project using R and Rmarkdown in such a way that:

* Analyses are reproducible
* Reports, talks, and papers all use the same R code
* Papers are compiled to HTML and PDF/Word at the same time; your paper is a website!
* Websites can include interactive figures, while PDF/Word contains static ones

## How to prepare

You might need to install some things first. You'll need some R packages.

* knitr
* papaja (for the PDF output )
* rmdformats (for HTML templates)
* pubprint (for easy statistics formatting)

You can install these packages by running the following command in R:

    install.packages(c('knitr','papaja','rmdformats','pubprint'))

### Windows

Software to download and install:

* MiKTeX, for compiling to PDFs (https://miktex.org)
* R (https://cran.r-project.org)
* RStudio (https://www.rstudio.com/products/rstudio/download3/)
* Zotero, for exporting bibtex files for bibliographies (https://www.zotero.org/download/)

If you would like to download bibtex reference files from the web, you'll also need:

* GNU wget for Windows, for downloading files in a script (http://gnuwin32.sourceforge.net/packages/wget.htm)
* GNU LibIconv for Windows, for converting file types (http://gnuwin32.sourceforge.net/packages/libiconv.htm)

If you do not want to download bibtex reference files, just comment the relevent files in the `buildme.bat` file with `REM` at the beginning of the line.

Additional tasks:

Add the R binary directory to the path.


### OSX

Software to download and install:

* MacTeX, for compiling to PDFs (https://www.tug.org/mactex/)
* R (https://cran.r-project.org)
* RStudio (https://www.rstudio.com/products/rstudio/download3/)
* Zotero, for exporting bibtex files for bibliographies (https://www.zotero.org/download/)

### Linux

Install using your favorite package manager, if available.

* LaTeX
* R 
* RStudio 
* Zotero, for exporting bibtex files for bibliographies (https://www.zotero.org/download/)

## How to compile

* Download the whole repository
* Edit the text in `papers/Rpaper1/text/sections/` if you like. The paper structure is in `structure.Rmd`; each section is a file in this directory.
* Set the Rstudio build script to `buildme` (or `buildme.bat` in Windows)
* Also, check out the website template in the `website` directory. With GitHub, you can easily create and host your own webpages, including the HTML version of your paper! You'll have to turn on GitHub pages, though.

