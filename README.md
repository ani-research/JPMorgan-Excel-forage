# Account Sales Data -- Task 4

## Overview

This workbook contains a hypothetical account-level sales dataset
prepared for the **JPMC Excel Skills Virtual Experience**. It includes
account details, product-line indicators, marketing and promotion
indicators, annual Product 1 sales volumes from 2017 to 2021, and a
five-year compound annual growth rate (CAGR).

The workbook contains 60 accounts across four account types, with 15
accounts in each type.

## Workbook structure

  -----------------------------------------------------------------------
  Worksheet                           Contents
  ----------------------------------- -----------------------------------
  `Sheet1`                            Main account-level dataset. Each
                                      row represents one account and
                                      includes account details, product
                                      and promotion indicators, annual
                                      sales volumes (2017--2021), and
                                      5-year CAGR.

  `Table2`                            Reshaped version of the account
                                      data in long format. Each account
                                      appears five times---once for each
                                      year---with the year stored in
                                      `Attribute` and the corresponding
                                      sales volume stored in `Value`.

  `Sheet2`                            Pivot-table summary showing sales
                                      for the Small Business segment in
                                      2017, broken down by account and
                                      decision maker. The displayed pivot
                                      output is filtered to this segment
                                      and year.

  `Sheet3`                            Blank worksheet.
  -----------------------------------------------------------------------

## Data fields

### Account information

-   `Account Name` -- Account identifier.
-   `Account Address` -- Account address.
-   `Decision Maker` -- Named contact associated with the account.
-   `Phone Number` -- Contact telephone number.
-   `Account Type` -- Customer category: Small Business, Medium
    Business, Online Retailer, or Wholesale Distributor.

### Product and promotion indicators

-   `Product 1`, `Product 2`, `Product 3` -- Indicate whether the
    account carries or is associated with each product line
    (`Yes`/`No`).
-   `Social Media`, `Coupons`, `Catalog Inclusion`, `Posters` --
    Indicate whether the account is associated with each listed
    marketing or promotional programme (`Yes`/`No`).

### Sales and growth

-   `2017`--`2021` -- Annual Product 1 sales volume, measured in units.
-   `5 YR CAGR` -- Five-year compound annual growth rate for Product 1
    sales volume.

In `Table2`, the annual sales columns are unpivoted into: - `Attribute`
-- The year (2017--2021). - `Value` -- Product 1 sales volume for that
account and year.

## Data dimensions

-   **Accounts:** 60
-   **Account types:** 4
-   **Accounts per type:** 15
-   **Annual sales period:** 2017--2021
-   **Main dataset:** 60 rows
-   **Long-format dataset:** 300 rows (60 accounts × 5 years)

## Notes for analysis

1.  Use `Sheet1` when analysing accounts at the account level or
    comparing annual sales across years.

2.  Use `Table2` for year-wise analysis, time-series visualisations, or
    workflows that require a long-format dataset.

3.  `Sheet2` is a pivot-table output rather than a complete summary of
    all account types and years. Check its filters or
    refresh/reconfigure the pivot table before using it as an overall
    sales summary.

4.  The CAGR field is calculated from the 2017 and 2021 sales volumes.
    If recalculating it outside Excel, use:

    `CAGR = (Sales_2021 / Sales_2017)^(1/4) - 1`

    The exponent is `1/4` because there are four year-to-year intervals
    between 2017 and 2021.

5.  Treat the workbook as a hypothetical learning dataset, not as
    verified real-world customer or sales information.

## Suggested starting points

-   Compare total Product 1 sales volume across 2017--2021.
-   Compare sales growth across the four account types.
-   Identify accounts with the highest and lowest 5-year CAGR.
-   Explore whether product-line participation or marketing-programme
    indicators are associated with sales performance.
-   Use the long-format `Table2` sheet to build year-wise charts or
    pivot tables.
