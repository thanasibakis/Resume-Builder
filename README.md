# Resume Builder

This project is a data-driven approach to creating my resume.

1. All resume entries (education, experience, etc.) are stored in a spreadsheet, without any formatting or styling information. A boolean *Include* column allows me to specify which entries I would like included in the document to be generated.
2. The R Markdown file reads the spreadsheet and does minor processing (ordering by date, merging dates into a phrase, etc.).
3. With the help of the [vitae](https://github.com/mitchelloharawild/vitae) package, a LaTeX template is populated with the resume entries, and a PDF is knitted.

## Usage

From an R prompt:

```r
rmarkdown::render("Resume.Rmd")
```

Alternatively, you can open `Resume.Rmd` in RStudio and click the *Knit* button.
