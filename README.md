# ICCAT papers for SCRS workshop

This Quarto format will help you create documents for the ICCAT publications.  
To learn more about ICCAT publications, see [ICCAT's infomation](https://www.iccat.int/Documents/SCRS/Other/Guide_ColVol_ENG.pdf). 
For more about Quarto and how to use format extensions, see <https://quarto.org/docs/journals/>.

## Creating a New Article

You can use this as a template to create an article for the ICCAT. To do this, use the following command:

```quarto use template ob7-ird/journals-iccat```

This will install the extension and create an example qmd file and bibiography that you can use as a starting place for your article.


## Installation For Existing Document

You may also use this format with an existing Quarto project or document. From the quarto project or document directory, run the following command to install this format:

```quarto add ob7-ird/journals-iccat```

## Usage 

To use the format, you can use the format names `iccat-pdf`. For example:

```quarto render article.qmd --to iccat-pdf```

or in your document yaml

```yaml
format:
  pdf: default
  iccat-pdf:
    keep-tex: true    
```


## Example

Here is the source code for a minimal sample document: [template.qmd](template.qmd).

<!-- pdftools::pdf_convert('template.pdf', pages = 1)  -->
![[template.qmd](template.qmd)](template_1.png)