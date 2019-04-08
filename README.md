# NRLcalc: calculation of the nucleosome repeat length

Code used from the paper 'What determines the decrease in nucleosome repeat length near bound CTCF?'

# Abstract
Nucleosome Repeat Length (NRL) is a calculation that I have had to perform many times throughout my PhD.

This measurement serves as a metric for nucleosome packing density for a piece of chromatin.

It involves manual point/peak picking on a plot called a phasogram.

This applet allows one to interactively click and pick points on phasograms, and easily calculate the NRL value for many different phasograms by use of a 'Next' and 'Back' button.

This applet saved me a lot of time.


# data
Contains example phasogram text files used in NRL calculations for CTCF predicted binding sites.

# scripts
Contains code that went into the preparation, processing and interpretation of the data. Can all be run sequentially from 'step_by_step.sh'

# Prerequisites

```
git clone https://github.com/arq5x/bedtools2 #bedtools
git https://github.com/homeveg/nuctools #nuctools
git clone https://github.com/chrisclarkson/nuctools_shiny # go to page for prerequisite installations and instructions

R
BiocManager::install("GenomicRanges")
BiocManager::install("AnnotationHub")
BiocManager::install("TFBSTools")
BiocManager::install("JASPAR2018")
BiocManager::install("TFBSTools")
BiocManager::install("BSgenome.Mmusculus.UCSC.mm9") 
install.packages("devtools")
devtools::install_github("matthuska/tRap")
```

# FigureS1
![embed](https://github.com/chrisclarkson/pics/blob/master/FigureS1.png)
