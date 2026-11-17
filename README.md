# Account Sales Data -- Task 4

## Overview

This workbook contains a hypothetical account-level sales dataset
prepared for the **JPMC Excel Skills Virtual Experience**. It includes
account details, product-line indicators, marketing and promotion
indicators, annual Product 1 sales volumes from 2017 to 2021, and a
five-year compound annual growth rate (CAGR).

The main dataset covers 60 accounts across four account types, with 15
accounts in each type.

## Workbook structure

  -----------------------------------------------------------------------
  Worksheet                           Contents
  ----------------------------------- -----------------------------------
  `Sheet1`                            Original account-level dataset.
                                      Each account appears once, with
                                      account details, product and
                                      promotion indicators, five annual
                                      Product 1 sales figures
                                      (2017--2021), and 5-year CAGR.

  `Table2`                            Long-format version of the
                                      account-level data. Each account
                                      appears once for each year from
                                      2017 to 2021. The `Attribute`
                                      column identifies the year and
                                      `Value` contains the corresponding
                                      Product 1 sales volume.

  `Sheet2`                            Pivot-table summaries of sales for
                                      the Small Business segment in 2017.
                                      The summaries break the sales
                                      figure down by account and by
                                      decision maker.

  `Sheet3`                            Dashboard containing two charts
                                      that provide a visual summary of
                                      the workbook's sales information.
                                      
  -----------------------------------------------------------------------

## Data fields

### Account information

-   `Account Name` -- Account identifier.
-   `Account Address` -- Account address.
-   `Decision Maker` -- Contact associated with the account.
-   `Phone Number` -- Contact telephone number.
-   `Account Type` -- Customer category: Small Business, Medium
    Business, Online Retailer, or Wholesale Distributor.

### Product and promotion indicators

-   `Product 1`, `Product 2`, `Product 3` -- Indicate whether the
    account is associated with each product line (`Yes`/`No`).
-   `Social Media`, `Coupons`, `Catalog Inclusion`, `Posters` --
    Indicate whether the account is associated with each listed
    marketing or promotional programme (`Yes`/`No`).

### Sales and growth

-   `2017`--`2021` -- Annual Product 1 sales volume, measured in units,
    in the original account-level dataset.
-   `5 YR CAGR` -- Five-year compound annual growth rate for Product 1
    sales volume.
-   `Attribute` -- Year label (2017--2021) in the long-format dataset.
-   `Value` -- Product 1 sales volume for the corresponding account and
    year in the long-format dataset.

## Data dimensions

-   **Accounts:** 60
-   **Account types:** 4
-   **Accounts per type:** 15
-   **Annual sales period:** 2017--2021
-   **Main dataset:** 60 account records
-   **Long-format dataset:** 300 account-year records (60 accounts × 5
    years)

## Notes for analysis

1.  Use `Sheet1` for account-level analysis and comparisons across the
    five annual sales columns.

2.  Use `Table2` for year-wise analysis, time-series visualisations, or
    workflows that require long-format data.

3.  `Sheet2` contains pivot-table summaries for **Small Business in
    2017**; it should not be interpreted as an overall summary of every
    account type and year.

4.  Use `Sheet3` for a visual overview of the sales information. The
    charts are dashboard elements; consult the underlying data and pivot
    tables when exact values or additional breakdowns are required.

5.  The CAGR can be recalculated from the 2017 and 2021 sales volumes
    using:

    `CAGR = (Sales_2021 / Sales_2017)^(1/4) - 1`

    There are four year-to-year intervals between 2017 and 2021.
