---
title: Export Procedures
description: Learn how to export output from the ADRF and navigate the export review process.
order: 7
lastUpdated: 2025-03-31
---

# Export Procedures

All sensitive data accessed through the ADRF is subject to strict disclosure and export rules. Any attempt to export data—whether for analysis, reporting, or sharing—must go through the official **export review process** to ensure compliance with these rules. (See [Glossary: Export Controls and Disclosure Reviews](/docs/glossary.md#export-controls-and-disclosure-rules) for more information on disclosure review.)

- Jump to [Step-by-Step Guide to Submitting an Export Request](#step-by-step-guide-to-submitting-an-export-request)

> [!TIP]
> You can find **video walkthroughs** on how to use the ADRF Export Module in the `ADRF_Documentation\Exports` folder in the `G:\` Drive. Topics include:
> - How to submit an export request
> - How to edit an export request
> - How to download an approved export

## Exporting Output from the ADRF

ADRF Users can submit an export review request through the ADRF's Export Module.

When you are ready to remove output from the ADRF, you must follow these steps:

1. Review the output you want to remove from the ADRF to make sure that you have protected the confidentiality of the data
    - This means you must ensure that your output does not violate the data’s export rules. 
    - For example, you may be required to aggregate any output to ensure that there are at least 10 individual entities in a cell.
2. Submit your export request through the ADRF’s export request module – making sure to follow the instructions given in the export review module documentation. 

## Review Process and Support

- **Timeline**: The disclosure review can take several days. Coleridge reviewers aim to complete the initial review within five business days, but timelines may differ based on your agency.
- **Stages**: The process typically involves two stages:
    - **Primary Review** (initial review for micro-data, up to 5 business days) 
    -  **Secondary Review** conducted by an approved Data Steward.
- **Status Check**: Check your submission status by logging into the ADRF and opening the Export module.
- **Support**: If you are unsure about the review guidelines contact Coleridge Support by submitting a Support Request through **Coleridge PASS** or emailing `support@coleridgeinitiative.org`.
  - Reach out for help before submitting the request to reduce downtime.

## Step-by-Step Guide to Submitting an Export Request

1. Log into the ADRF (via http://adrf.okta.com) and select your project.
2. Access the Export Request Module via the SecurePASS page in Google Chrome when you first log in, or navigate to `secure-pass.adrf.net`.
3. Click **My Requests** in the drop down in the red menu on the left side of the Secure PASS page. 
4. Click **Create New Request** on the right side of the My Request page.
5. Complete the requested fields, upload your files (including supporting documentation).
6. Click **Submit Export Request** when you're ready to submit.

> [!TIP]
> You can find **video walkthroughs** on how to use the ADRF Export Module in the   `ADRF_Documentation\Exports` folder in the `G:\` Drive.

## General Best Practices for a Successful Export

Adhering to these practices will help expedite the review process:

### Output Control
1. **Code Generation**: Produce all output files (tables, graphs, etc.) through code rather than manually, as reviewers read your code.
2. **Documentation**: Every code file must have a header describing its contents. Document code with comments throughout, including details on the level of aggregation, as better documentation leads to a faster turnaround.
3. **Final Versions Only**: Only request review of final versions of output files; any file containing intermediate output will be rejected.
4. **File Limits**: Limit export requests to only the necessary outputs for a specific report. Requests for more than 10 files may incur an additional charge.

### Confidentiality Compliance
1. **Pre-submission Review**: Review your output to ensure it protects confidentiality and meets the data's specific export rules.
2. **Prohibitions**: You must not take a screen shot of any data point, table, graph, or metadata, nor write down any results or take notes outside of the ADRF.

## How to Check Your Export Review Status

You can check on the status of a submitted Export Request through the **ADRF Export Module**.

### Review status descriptions

To help you better understand the different stages of the Export Review process, here are the status descriptions you may encounter:

1. **Awaiting Reviewer**: Your export is currently under primary review. If any issues arise during the primary review, your reviewer will notify you. Upon completion of the primary review, the secondary reviewer(s) will be notified.
2. **Awaiting Secondary Review**: Your export is currently under secondary review. If your submission pertains to multiple data assets, it will require a review by each Data Steward before being approved.

## Preparing Data for Export

Each agency has specific disclosure review guidelines, especially with respect to the minimum allowable cell sizes for tables. Refer to these guidelines when preparing export requests. If you are unsure of what guidelines are in place for the dataset with which you are working in the ADRF, please reach out to [support@coleridgeinitiative.org](mailto:support@coleridgeinitiative.org)

### Tables

- **Cell Sizes**:
  - For individual-level data, please report the number of observations from each cell. For individual-level data, the default rule is to suppress cells with fewer than 10 observations, unless otherwise directed by the guidelines of the agency that provided the data.
  - If your table includes row or column totals or is dependent on a preceding or subsequent table, reviewers will need to take into account complementary disclosure risks—that is, whether the tables' totals, or the separate tables when read together, might disclose information about individuals in the data in a way that a single, simpler table would not. Reviewers will work with you by offering guidance on implementing any necessary complementary suppression techniques.
- **Weighted Data**: If weighted results are to be exported, you must report both weighted and unweighted counts.
- **Ratios**: If ratios are reported, please report the number of valid cases for both the numerator and the denominator (e.g., number of men in state X and number of women in state X, in addition to the ratio of women in state X).
- **Percentiles**: Do not report exact percentiles. Instead, for example, you may calculate a "fuzzy median," by averaging the true 45th and 55th percentiles.
- **Percentages**: For any reported percentages or proportions, the underlying counts of individuals contributing to the numerators and denominators must be provided for each statistic in the desired export.
- **Maxima and Minima**:
  - Suppress maximum and minimum values in general.
  - You may replace an exact maximum or minimum with a top-coded value.

### Graphs

- Graphs are representations of tables. Thus, for each graph (which may have, e.g., a jpg, pdf, png, or tif extension), provide the source data of the underlying table of the graph following the guidelines for tables above.
- Because graphs and other figures take the most time to review, the number of generated graphs should be as low as possible. Please consider the possibility that you could export the underlying table instead, and generate the graph in another package.
- If a graph is produced from aggregated data or from tables that have been disclosure-proofed following the guidelines above (e.g., bar charts of magnitudes), provide the underlying tables.
- If a graph is produced directly from unit-record data but aggregated in the visualization (e.g., frequency histograms), provide the underlying tables.
- If a graph is produced directly from unit-record data and displays unit-record values (e.g., scatterplots, plots of residuals), the graph can be released only after you ensure that individuals cannot be re-identified and that values can only be estimated with a high level of uncertainty. Further processing to meet this requirement can include, but is not restricted to, cutting off the tails of a distribution, removing outliers, jittering the actual values, and removing or modifying axis values.
- If a graph is produced from the results of modeling or derivation and uses the unit-record data (e.g., regression curves), the graph can be released only if the values cannot be used to find original data values.
  - Graphs of this type are generally automatically cleared.
  - For precision/recall graphs, you will need to report the sample size used to generate your model(s).

### Model Output

Output from regression or machine-learning models generally does not pose a risk of disclosing personally identifiable information, as long as the models are not based on small samples. Provide the counts for each variable that produces the model output. If categorical variables are used then provide the counts for each category.


<br>

---
# Support & Navigation

**Need help?**
- Email: support@coleridgeinitiative.org
- Hours: Monday-Friday, 9 AM - 5 PM ET

**Navigation**
- ⬅️ [Back to Home](../README.md)