# JZ Finance

**JZ Finance is a library of various useful financial functions to generate various schedules, tables and analysis using one simple formula** This library is written using Excel built-in formulas and lambda functions to hide the complexities of combining multiple excel functions.

## Categories

JZ Finance consists of below categories of functions:
- Full Schedules
    - `JZ.Loan_Schedule` to generate a full loan amortization schedule for any loan. User can select which columns to display and in what order (For details: [Click here](Functions.md))
- Single Data Point

## Demo

Demo file is available in [demo folder](https://github.com/jahanzaibriaz/JZ_XL/tree/main/jz_finance/Demo) that demonstrates how to use this function

## Installation
1) Get Excel Labs add-in from https://aka.ms/get-afe
2) On Home tab in Excel, click on Excel Lab
3) Click on Modules
4) Click on Import from URL button
5) Enter this URL https://gist.github.com/jahanzaibriaz/ee2752fc71a5f6eb11aa0cb897486f39
6) In any cell, enter "=JZ.Loan_Schedule(12%, 60, 100000)"

## License

JZ Finance is [MIT licensed](https://github.com/jahanzaibriaz/jz_finance/blob/main/LICENSE).

## Contact

You could [open an issue](https://github.com/jahanzaibriaz/jz_finance/issues).

## Full list of functions
- [`JZ.LOAN_SCHEDULE`](Functions.md): generate the full loan schedule, selected columns, selected rows or individual data point. It takes following aruments
