# thesisdowndss

This project was inspired by the [bookdown](http://github.com/rstudio/bookdown) and [thesisdown](https://github.com/ismayc/thesisdown) packages.

Currently, the PDF and gitbook versions are fully-functional. (The word and epub versions are developmental, have no templates behind them, and are essentially calls to the appropriate functions in bookdown. There is no plan to further develop these, in fact, files related to these will be removed in the near future.)

The current outputs for the two functional versions are here:
- [PDF](https://github.com/ismayc/thesisdown_book/blob/gh-pages/thesis.pdf) (Generating LaTeX file is available [here](https://github.com/ismayc/thesisdown_book/blob/gh-pages/thesis.tex) with other files at in the [book directory](https://github.com/ismayc/thesisdown_book/tree/gh-pages).)
- [gitbook](http://ismayc.github.io/thesisdown_book)

Under the hood, the Duke StastSci LaTeX template is used to ensure that documents conform precisely to submission standards. At the same time, composition and formatting can be done using lightweight [markdown](http://rmarkdown.rstudio.com/authoring_basics.html) syntax, and **R** code and its output can be seamlessly included using [rmarkdown](http://rmarkdown.rstudio.com).

Using **thesisdowndss** has some prerequisites which are described below. To compile PDF documents using **R**, you are going to need to have LaTeX installed.  It can be downloaded for Windows at <http://http://miktex.org/download> and for Mac at <http://tug.org/mactex/mactex-download.html>.  Follow the instructions to install the necessary packages after downloading the (somewhat large) installer files.  You may need to install a few extra LaTeX packages on your first attempt to knit as well.

### Using thesisdowndss from Mine's GitHub

To use **thesisdowndss** from within RStudio:

1) Install the latest [RStudio](http://www.rstudio.com/products/rstudio/download/).

2) Install the **bookdown** and **thesisdown** packages: 

```S
install.packages("devtools")
install.packages("bookdown")
devtools::install_github("mine-cetinkaya-rundel/thesisdowndss")
```

3) Use the **New R Markdown** dialog to select **Thesis**:

![New R Markdown](thesis_rmd.png)

Note that this will currently only **Knit** if you name the directory `index` as shown above.
