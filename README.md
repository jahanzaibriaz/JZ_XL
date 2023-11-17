# JZ Finance

**JZ Finance is a library of various useful financial functions to generate various schedules, tables and analysis using one simple formula** This library is written using Excel built-in formulas and lambda functions to hide the complexities of combining multiple excel functions.

## Categories

JZ Finance consists of below categories of functions:
- Full Schedules
    - `JZ.Loan_Schedule` to generate a full loan amortization schedule for any loan. User can select which columns to display and in what order
- Single Data Point

## Demo

Demo file is available in demo folder that demonstrates how to use this function

## Installation

**Excel version requirement:** Many functions of AutoXL are written with newly-introduced built-in functions of Excel, which require Microsoft 365 and probably don't exist in non-subscription Office 2019 or later. Therefore, AutoXL has the same requirement. You could simply type `=VSTACK` in a cell, if its intellisense shows up, that means your Excel meets the requirement.

<!-- If you don't have the good version of Excel on your machine, you could always use [Excel Online](https://www.office.com/launch/excel?ui=en-US&rs=GB&auth=1) which has new functions and is free. -->

**Get started quickly:** You could download the workbook `Demo/AutoXL-Demo.xlsx` where AutoXL has been already added. It also contains sample data and formulas which allow you to get familiar with use of functions. Formula Editor will be auto-opened.

**Installation:** Besides using Microsoft's AFE, you could use [Formula Editor](https://www.10studio.tech/docs/formulaEditor) to add the AutoXL library to your workbook, which will provide a version control. The latest stable versions of AutoXL will always be available in Formula Editor.

![alt text](Demo/VersionControl.gif)

**Uninstallation:** To remove the library from your workbook, 
- either you could go to "Name Manager" and manually delete all the functions starting with `A.` (make sure that you don't have other user-defined functions or ranged names starting with `A.`)
- or under Formula Editor, you could go to "Libraries => AutoXL => Remove"; it will only remove AutoXL's functions.

## License

JZ Finance is [MIT licensed](https://github.com/jahanzaibriaz/jz_finance/blob/main/LICENSE).

## Contact

You could [open an issue](https://github.com/jahanzaibriaz/jz_finance/issues).

## Full list of functions
- `JZ.LOAN_SCHEDULE`: generates the loan schedule

## Other resources

- Video courses: [Spreadsheet Language and Programming](https://chengtie.thinkific.com/courses/excel-programming-en) and [表格语言与编程](https://study.163.com/course/courseMain.htm?courseId=1211128814&share=2&shareId=480000002246464)
- Software for spreadsheets: [www.10studio.tech](https://www.10studio.tech)
- Social media: [YouTube](https://www.youtube.com/watch?v=Jr1x1EnP1qA&list=PLOeixAylgNENCnQr9pUWjyAVFzJGbiOSX), [LinkedIn](https://www.linkedin.com/in/chengtie/)
