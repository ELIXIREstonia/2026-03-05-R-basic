# 2025-09-01-R-basic

ELIXIR-EE training course on R and RStudio basic usage. Targeted to learners who have no or very little prior experience with R and RStudio.

The main instructional materials are the R Markdown documents in this repository:

- `R-basic.Rmd` — learner-facing workshop material
- `R-basic-instructor.Rmd` — instructor notes and solutions

R Markdown allows code (examples) and explanation/documentation to be in the same document in a nicely formatted, well structured manner. You can render the learner document locally with RStudio or from R with:

```r
# render learner material
rmarkdown::render("R-basic.Rmd")
```

Data files used in the examples are located in the `data/` folder. Current files included:

- `data/Islander_data.csv`
- `data/Islander_data.tsv`
- `data/Islander_data.xlsx`

Learning outcomes for the training:

1.  **Understanding Basic R Data Structures**:

    -   Learners will be able to distinguish between primary R data structures, namely vectors, matrices, data frames, and lists.

    -   They will be proficient in initializing and inspecting these structures using basic R functions.

2.  **Data Transformation with Tidyverse**:

    -   Participants will gain proficiency in using the **`%>%`** pipe operator to chain together functions for data manipulation.

    -   They will understand and be able to apply essential tidyverse functions like **`select`**, **`rename`**, **`filter`**, **`mutate`**, **`group_by`**, **`summarize`**, and **`arrange`** to transform and analyze datasets.
    -   They will also learn common data manipulations like **`pivot_wider`** and **`pivot_longer`**

3.  **Data Categorization and Conditional Operations**:

    -   Trainees will be equipped to generate new variables in a dataset based on conditional logic, such as categorizing numerical data into distinct groups.

4.  **Application of Data Manipulation Techniques**:

    -   By the end of the session, participants will have hands-on experience in applying the introduced concepts to real-world datasets, such as the "Memory Test on Drugged Islanders" dataset. They'll be able to group data, compute summary statistics, and create new columns based on specific criteria.

### Course materials (at a glance)

- Authors / date: Priit Adler & Nurlan Kerimov (2025-09-01).
- How to read data: `readr::read_csv()`, `readr::read_tsv()`, and `readxl::read_excel()` (examples shown in `R-basic.Rmd`).
- Tidyverse overview and common verbs taught: `%>%` (pipe), `filter()`, `mutate()`, `select()`, `rename()`, `arrange()`, `group_by()`, `summarize()`, `left_join()` (joins) and related helpers.
- Conditional operations and new columns: `case_when()` examples for creating categories (age groups, etc.).
- Reshaping data: `tidyr::pivot_wider()` and `tidyr::pivot_longer()` with examples (`fish_encounters`, `relig_income`).
- Practical dataset used in exercises: the "Memory Test on Drugged Islanders" dataset (Kaggle). Exercises include grouping, summarizing, dosage and age-group analyses, and comparing groups (happy/sad priming).

### Next step

Take a look at our follow-up course on how to create compelling visualisations using R and ggplot2: https://github.com/ELIXIREstonia/2024-10-09-R-visualisation

---

License: see `LICENSE`.

Feedback form is here: https://forms.gle/KaFiPPvuY4HY376G9