# ENVS 193DS Spring 2023 week 6 coding workshop

Since the midterm is due on Thursday, this coding workshop focuses on niche but potentially useful skills to have. By the end, you'll be able to:  
- use color palette packages in R (examples include `{NatParksPalettes}` and `{wesanderson}`)  
- make an interactive plot using `{plotly}`  
- insert images into `ggplot` objects using `{magick}`  
- do some more advanced data cleaning using functions from `{stringr}` and `{forcats}` (both `{tidyverse}` packages)  
- organize your Quarto/RMarkdown documents to better understand how they render/knit (useful for troubleshooting errors!)  
- set up a repository with GitHub pages

## Required packages

This workshop is going to be _more fun_ if you have the following packages installed:  

### Things you should already have

- `{tidyverse}`  
- `{here}`  
- `{naniar}` (or equivalent)  

### Things that you don't _have_ to have but would make this more fun for you:

- `{skimr}`: to quickly summarize data ([documentation](https://docs.ropensci.org/skimr/))  
- `{plotly}`: to make interactive plots using Javascript ([documentation](https://plotly.com/r/getting-started/))  
- `{magick}`: to put images into plots ([documentation](https://docs.ropensci.org/magick/index.html))  
- `{NatParksPalettes}`: a color palette package ([documentation](https://github.com/kevinsblake/NatParksPalettes))  
- `{wesanderson}`: another color palette package ([documentation](https://github.com/karthik/wesanderson))  
- `{patchwork}`: to put plots together ([documentation](https://patchwork.data-imaginist.com/))  

## New or new-ish functions

Not an exhaustive list!  

- `lubridate::year()` (in `{tidyverse}`)  
- `lubridate::month()` (also in `{tidyverse}`)  
- `forcats::fct_relevel()` (also in `{tidyverse}`)  
- `stringr::str_detect()` (also in `{tidyverse}`)
- `paste`/`paste0`  
- `skimr::skim()`  

## Rendered output

In this workshop, we'll talk about how to use GitHub pages. The rendered output is [here](https://an-bui.github.io/ENVS-193DS_week-06/key/workshop-06_2023-05-09_key.html).  

When using GitHub pages, the URL for any rendered/knitted output is "your github username.github.io"/ "repository name"/"file path". So, for example, the url for the rendered output (linked above) is:
`an-bui.github.io/ENVS-193DS_week-06/key/workshop-06_2023-05-09_key.html`.

## Data sources

The gray whale count data is from the Environmental Data Initiative's data portal. Source: SBC Marine Biodiversity Observation Network, M. Smith, and L. Kui. 2020. Santa Barbara Channel Marine BON: Gray Whales Count ver 2. Environmental Data Initiative. https://doi.org/10.6073/pasta/5ebbc61168c4e0fcd0546f4f68c70a11 (Accessed 2023-05-10).  

The gray whale count happens every year off of Coal Oil Point! Read more about those efforts [here](http://www.graywhalescount.org/GWC/About_GWC.html).

## Image sources

The object `whale_image1` comes from [NOAA Fisheries](https://www.fisheries.noaa.gov/species/gray-whale). The object `whale_image2` is read in using `magick::image_read()` from this [URL](https://www.acsonline.org/assets/images/eschrichtius-robustus.png) (current as of 2023-05-09).  


