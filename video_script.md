## Introduction

Hi, this is joseph holler and I'd like to give you a preview of the infrastructure that myself and Dr. Kedron have been developing to facilitate reproducible and replicable research in the geographical sciences.
you may have landed here from our research website, or conference workshop website

- HEGSRR Website **-Navigate to template-**
- Template Repository (Github)
 - This template repository is designed to facilitate researcher adoption of OSRP, and by extension improve R&R of spatial data science and geographic research.
 - The template ships with the BSD license so that other researchers have legal permission to reproduce and extend your work with attribution.
 - **-Scroll readme, Show 1 sub-folder-** Much of the template structure is summarized in this top level readme, and each sub-folder in the template contains instructions on how to use that particular resource.
 - We are also presently developing a manual the demonstrates how to use this template in university courses.
 - In this video, we will illustrate how open science research practices are supported by our template structure by showing how we have deployed it to conduct a reproduction study and setup a replication study.

## Spielman et al. (2020)
**-Navigate to Spielman Repository-**
- Motivation: We attempted to reproduce a spatial analysis of the SOVI for 3 reasons:
 1. The paper is an example of a replication study of which there are few in geography,
 2. SOVI is a highly influential model (the original SOVI publication has garnered 7,134 citations).
 3. We wanted to use this as a hands on example to teach undergraduate GIS students OSRP

**-Navigate to original Spielman repository-**
- Another reason we selected this article is because the authors did make available the data and code used in their analyses.
- You may think that because these authors took the time to share their data and their code in a Github repository that it would be relatively easy to reproduce their results. That was not the case.
- In fact, reproducing this study took significant effort by a faculty member and RA with significant GIS, spatial analysis, and computer science experience.
- The raw materials were available, the paper was well-written, and the data and code were available. However, the organization of those materials and the tacit knowledge that went into producing the result were missing.
- Our template addresses with these challenges, and makes it easier for other to recreate, assess, and build on your work.

**-Navigate to OSF Project -> RPR Report & RPL PAP-**
- Our effort to reproduce Spielman et al. (2020) created many intermediate products, but the two key summary products are a report detailing our reproduction attempt and findings, and a PAP for a subsequent replication attempt that will extend this work.

- For those familiar, you may notice that these .pdf are renderings from Jupyter notebooks where all of our writing and analysis were done together.

- So how did we go about this research, and how did our template support that effort?

## Template Tour
**-Navigate to template repository-**
- already covered top-level
- structured template of directories for organizing all of the components of a research project with relative links
- we start a project by writing an analysis plan, and for computational studies this can be done with our Rmarkdown or Jupyter Notebook templates, and we strongly recommend keeping all research plans and procedures in one main comprehensive notebook
**-open template**, here is the jupyter version of our template, including code for managing folders and computational environment
- this template compendium and analysis plan is paired with growing user manual
**-navigate to metadata**
- analysis planning includes researching or creating metadata for research data inputs
- we provide ISO-standard markdown metadata templates for easy inclusion in a pre-analysis plan
- once a plan is complete, you can render a PDF, save to the docs folder, and register your plan.
- the benefit of working within a Git repository is that each step of research development is version tracked.

- for data science research, the next step is acquiring and creating data. We do this with the computational notebook and populating unmodified data in a raw directory and downstream processed data in a derived data folders.
- **navigate to data**

- once you reach the analysis stage of research, results are generated and displayed in the notebook, and figures can be saved to the results folder
- figures and tables in the paper are directly linked the data and analysis through code, so there's no risk of transcription errors
- from here, the researcher needs only to discuss results and add conclusions before rendering an analysis report.
- this can also be exported as a LaTeX document for manuscript preparation
