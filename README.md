# Clean CPSC course data

The repository contains the Quarto document `index.qmd` (requires Quarto version 1.4 or higher) for cleaning the UBC CPSC undergraduate and graduate course data.

## Setup

### Data

Data is not included in this repository. The analysis assumes that source data `course_counts_raw.xlsx` is located in `data/raw.` No personal data is contained in this repo other than instructor names.

### Development environment

#### Local install

We recommend using [RStudio](https://www.rstudio.com/products/rstudio/) (v2022.07.1+554 or newer will also include Quarto) and opening the contained R project.
Check the [Quarto documentation](https://quarto.org) for information on working with Quarto documents and alternative tools to RStudio for working with them.

[{renv}](https://rstudio.github.io/renv/index.html) tracks R package dependencies.
When you open the R project for the first time, {renv} should bootstrap the setup of the R environment.
You can manually restore the project's dependencies with

``` r
renv::restore()
```

and update any dependencies with

``` r
renv::snapshot()
```

#### Local devcontainer

We recommend developing content locally on your computer in a container accessed by [Visual Studio Code](https://code.visualstudio.com/).
Follow the setup instructions outlined in [Developing inside a Container using Visual Studio Code Remote Development](https://code.visualstudio.com/docs/devcontainers/containers) including the installation of Docker and the VS Code extension [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers).
After cloning this repo locally to your computer, open the directory using the command **Dev Containers: Open Folder in Container...** from the Command Palette in VS Code.
