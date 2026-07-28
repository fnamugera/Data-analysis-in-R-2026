# Data-analysis-in-R-2026
## Webinar Series Overview
ACSPR plans to organize a two-part practical webinar series on Practical Data Analysis and Management Using R. The first webinar will be held on Thursday, 30th July 2026, from 4:00 PM to 6:00 PM EAT, while the second webinar will be held on Thursday, 27th August 2026, from 4:00 PM to 6:00 PM EAT. Each session will run for two hours and will combine conceptual guidance, live coding demonstrations, practical exercises, and interactive discussion.

The series will provide participants with foundational and applied knowledge on how to use R for data management, analysis, visualization, and presentation of results. The webinars will be facilitated by an experienced trainer with practical expertise in quantitative data analysis and research methods.


# Pre-Training Instructions for Participants

## R Training Workshop: Survey Data Management and Analysis Using R

To help the training run smoothly, please complete the steps below **before**
the first session. None of it is difficult, but a few steps (downloads,
installs) take time in the background, so it's best not to leave this until
the morning of the workshop.

**Estimated time:** 20--30 minutes

---

## At a Glance

- [ ] Install R
- [ ] Install RStudio
- [ ] Download the training materials
- [ ] Create a training folder (with a `data/` subfolder)
- [ ] Create an RStudio Project inside that folder
- [ ] Install the required R packages
- [ ] Verify your installation
- [ ] Pack your laptop, charger, and materials

---

## 1. Install R

Download and install the latest version of R from:

**[cran.r-project.org](https://cran.r-project.org/)**

> **Order matters:** install R *before* RStudio. RStudio is just an
> interface to R, and needs R already present on your machine to detect it.

## 2. Install RStudio

Download and install the free version of RStudio Desktop from:

**[posit.co/download/rstudio-desktop](https://posit.co/download/rstudio-desktop/)**

## 3. Download the Training Materials

The training materials are hosted on GitHub:

**[github.com/fnamugera/Data-analysis-in-R-2026](https://github.com/fnamugera/Data-analysis-in-R-2026)**

Since this is a GitHub repository rather than a direct file link, download it
as a ZIP folder:

1. Open the link above
2. Click the green **Code** button
3. Select **Download ZIP**
4. Extract (unzip) the downloaded folder on your computer

The repository contains:

- `DHS_data.dta` -- the Malawi DHS dataset (Stata format)
- `DHS_data.csv` -- the same dataset in CSV format
- `Data codes.csv` -- a codebook explaining what each variable and code means
- `README.md` -- a short description of the repository

> **Note:** the R Markdown training file (`.Rmd`) is not in the repository
> yet. Please check with the training coordinators closer to the date in
> case it's added separately or shared through another channel.

## 4. Create a Training Folder

Create a folder on your computer, for example:

```
R_Training/
```

Inside it, create a subfolder named:

```
data/
```

Save all downloaded datasets inside the `data/` folder, and save the
`.Rmd` training file (once you have it) in the main project folder. Your
folder structure should look like this:

```
R_Training/
|
|-- data/
|   |-- DHS_data.dta
|   |-- DHS_data.csv
|   `-- Data codes.csv
|
|-- R_Training.Rmd            (once available)
|
`-- (Project file will be created here)
```

## 5. Create an RStudio Project

Once R and RStudio are both installed:

1. Open **RStudio**
2. Select **File -> New Project**
3. Choose **New Directory**
4. Select **New Project**
5. Browse to the `R_Training` folder you created
6. Enter a project name (e.g., `R_Training`)
7. Click **Create Project**

Working inside an RStudio Project keeps all your files organized and
ensures file paths work correctly throughout the training.

## 6. Install the Required Packages

Open the **Console** in RStudio and run:

```r
install.packages(c(
  "tidyverse",
  "haven",
  "readxl",
  "labelled"
))
```

This may take a minute or two the first time. Once it finishes, confirm
everything loads without errors:

```r
library(tidyverse)
library(haven)
library(readxl)
library(labelled)
```

## 7. Verify Your Installation

Run the following in the RStudio Console:

```r
2 + 2
```

Expected output:

```
[1] 4
```

Then check your R version:

```r
version
```

If both commands run without errors, your installation is complete and
you're ready for the training.

## 8. What to Bring

- [ ] A laptop with administrator privileges
- [ ] Laptop charger
- [ ] The downloaded training materials
- [ ] A working installation of R and RStudio
- [ ] Internet access (recommended, in case additional packages or updates are needed)

## 9. Need Assistance?

If you run into any difficulty installing the software or accessing the
training materials, please contact the training coordinators **before**
the training date so support can be provided in advance.

---

We look forward to your participation, and wish you a productive
training experience!
