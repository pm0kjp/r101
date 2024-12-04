This is the GitHub repository for the workshop series called **R 101: Introduction to R For Clinical Data**, given at the Children's Hospital of Philadelphia (CHOP) by Arcus Education and the CHOP R User Group.

This repository contains the files you need to be able to complete the exercises in each of the workshop sessions.  

Exercises for you to complete are in the [exercises](https://github.com/arcus/r101/tree/main/exercises) folder, and working solutions files are found in [solutions](https://github.com/arcus/r101/tree/main/solutions).

## About This Workshop Series

Welcome to R101! 

This series is intended to be a gentle introduction to data science for healthcare professionals (e.g. MDs, RNs, NPs, data managers, clinical researchers) and others who interact with clinical or research data. This course is geared towards beginners who are comfortable with Excel but have no programming background.
 
The workshop will cover why and how to get started using the R statistical programming language in your work. We’ll talk about how to import data, transform data, and create lovely data visualizations in R, all while setting you up with best practices for creating reproducible reports. 

## Workshop Sessions

Material in later sessions does build on work done in earlier sessions, but don't let missing a session keep you away from attending later sessions.  We try to overlap material to help keep everyone caught up!

Use this form to [register to attend one or more workshop sessions](https://redcap.link/R101_Signup).

- **Introduction to R/RStudio**
  * Considerations for working with R at CHOP
  * What you need for the course
  * R and RStudio
  * R Markdown and literate statistical programming
  * Learning to learn data science
- **Data Ingestion and Projects**
  * Tabular data ingestion from files
  * Projects in R
  * File system considerations
  * Data visualization preview
- **Data visualization with ggplot2**
  * Ingesting data from REDCap
  * ggplot2 syntax
  * Aesthetics / visuals 
- **Transforming data using dplyr**
  * Selecting columns
  * Filtering rows
  * Creating new columns
  * Renaming, combining, splitting data
- **Tidying data**
  * Tidy data defined
  * Wide and long data formats 
  * Using pivot functions
- **Recap and next steps for growing in R**
  * Creating reports, manuscripts, slideshows, and dashboards
  * Machine learning
  * Statistical tests 

For all of the talks, you can [work hands-on with the code and see solutions in our Posit.cloud project](https://posit.cloud/content/7522885)

## Before your first workshop session

Before attending a workshop session, please do the following.  

**Necessary**:

* Create a free [Posit.cloud](https://posit.cloud) account.  We will use this as our training environment and you will have continued access to your code and materials after the workshop, through your account at Posit.cloud.
* Please review our [Code of Conduct](https://github.com/arcus/intro-to-r-for-clinical-data/blob/main/conduct.md).

**Highly Recommended**:

* Install or update the [Google Chrome browser](https://www.google.com/chrome/) on the computer you'll use.  We highly recommend you use Chrome to access our workshop training environment.
* Download and install the latest version of [Teams](https://www.microsoft.com/en-us/microsoft-teams/download-app) (you may also choose to join in a browser).
* Consider installing [R](https://cloud.r-project.org/) and [RStudio Desktop](https://rstudio.com/products/rstudio/download/) on your computer, so you can hit the ground running after the workshop finishes!
* Consider installing Git and GitHub Desktop on your computer, so you can hit the ground running after the workshop finishes!
* If you haven't already, and you're a CHOP or Penn employee, please consider [joining CHOP's R User Group](http://bit.ly/chopRusers).


In the first session, we will talk about how to request software at CHOP via a [service ticket](https://chop.service-now.com/esc?id=sc_cat_item&sys_id=fbf31958db4efe00de9e782bbf96192c).  We suggest installing these programs (or, if you don't have sufficient rights, asking DTS to install them) on your CHOP-assigned device(s):

* R -- the language we use to clean, analyze, and visualize data 
* RStudio Desktop -- an IDE for writing R 
* Git -- version control software that will allow you to easily get the latest version of our course materials and will also be helpful for tracking changes in your own projects
* GitHub Desktop -- a helper, or "client" software that makes working with Git easier

Even though all of these software are free, you'll need a Cost Center (or grant fund) to add to your request.  Get that from your manager, administrative staff, or other leadership within your area.  There will be no charge, but DTS uses this information for tracking resource utilization.

You'll also need the [MAC address](https://www.cmu.edu/computing/services/endpoint/network-access/mac-address.html) of the device you need the software installed to.

Having R, RStudio, Git, and GitHub installed locally on your CHOP-issued device is not the **only** way to work with R and RStudio, but it can be the most convenient, and will be compliant with the constraints of working with real clinical data.  You won't want to rely on RStudio on your personal device or on the cloud when it comes to working with real data!

**On the day of your workshop**

We suggest the following for virtual webinars:

* If available to you, use two monitors (or another two-screen setup such as a laptop and a tablet or two laptops).
* Follow along in the [slides](https://pm0kjp.quarto.pub/r101/quarto_slides/index.html#), if you like.

## Where to do the exercises

### Use Posit.cloud

The easiest way to do the workshop exercises is to create a free account at <https://posit.cloud> and then go to [our workshop project](https://posit.cloud/content/7522885) and make your own permanent copy of this project so you can make changes and work with it later.

Alternately, in Posit Cloud you can also add a new project and select "New Project from Git Repository" and enter the url of this repository, namely <https://github.com/arcus/r102>.

### Use Your Own R/RStudio

If you want, you can install R and RStudio Desktop for free on your computer, following the [instructions Posit offers](https://posit.co/download/rstudio-desktop/).  Then you can either:

* Use File > New Project to create a new project from version control and add the URL of this repository (namely, <https://github.com/arcus/r102>)
* Download the files in this repository (the green "Code" button will allow you to download a zip file of this repository's contents) and then use File > New Project > Existing Directory to create an R project in the directory where you stashed those files.

## Dependencies

The files here depend on several R libraries, which you can install using the following command:

```r
install.packages(c(
  "tidyverse",
  "rmarkdown",
  "medicaldata",
  "gtsummary"
))
```

## Slides

[Slides](https://rosemhartman.quarto.pub/r102/quarto_slides/index.html#/r102-mastering-the-fundamentals-in-r) of the teaching presentation that accompany each of the workshop sessions are available and you are welcome to follow along or refer back to them at a later date.  
The source code for these slides is included in the directory [quarto_slides](https://github.com/arcus/r102/tree/main/quarto_slides) in this repository.

## License

All of the material in this GitHub repository is copyrighted under the [Creative Commons BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) copyright to make the material easy to reuse. 
We encourage you to reuse it and adapt it for your own teaching as you like!

## Acknowledgements

Material for some of these sessions was adapted from [DART data science learning modules](https://arcus.github.io/education_modules/educators), a project developed by the Arcus Data Education team at CHOP. 
In particular, the following modules were adapted for workshop sessions: 

- [Missing Values in R](https://bit.ly/DART_r_missing_values)
- [Summary Statistics in R](https://bit.ly/DART_r_summary_stats)

Three cheers for remixing and reusing open education materials! 
