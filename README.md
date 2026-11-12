# M08 Reflection — Quarto RevealJS

## What is included

- `M08-Reflection-gtsummary.qmd`: the editable presentation source.
- `ga4_session_medium.csv`: actual aggregate GA4 session-medium export used in Prompt 3.
- `google_ads_daily.csv`: actual Google Ads campaign-day export used in Prompt 4.
- `styles.css`: simple formatting adjustments.
- `project-mark.svg`: small slide logo.
- `M08_Reflection_Project.Rproj`: opens the folder as an RStudio project.

No simulated survey data or call-level exports are included.

## Install packages (once)

In the **RStudio Console**, not inside a Quarto code chunk:

```r
install.packages(c("tidyverse", "gtsummary", "gt", "broom", "broom.helpers"))
packageVersion("broom.helpers")
```

`broom.helpers` must be version 1.20.0 or later for the `gtsummary` installation you are using. If you are only missing that dependency, `install.packages("broom.helpers")` is enough.

## Render

Open the `.Rproj` file in RStudio and render `M08-Reflection-gtsummary.qmd` to RevealJS HTML. Do not rename or move the CSVs before rendering; the QMD reads them from the project folder.

A complete Quarto render has not been tested here because R and Quarto are unavailable in this runtime. If you see a new error, send the *first* error message and the chunk label, and it can be corrected in the source.

## Final steps

1. Replace the two GitHub placeholder lines on the last slide with your published repository and Pages URLs.
2. Render the QMD again after editing the URLs.
3. Submit the final rendered `.html` and `.qmd` files to Canvas.
4. When publishing the repo, do not include the original Google Ads ZIP or call-level exports, which may contain sensitive information.

The data examples here are **exploratory analyses of actual client exports**. GA4 counts represent sessions, not people. Google Ads data represent campaign days, not consultations or survey respondents.
