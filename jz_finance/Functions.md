# JZ Finance

## Functions

- ### JZ.Loan_Schedule
    **Description**: Generates selected columns, selected rows, individual data point or a full loan schedule for a loan

    **Inputs**:
    | Argument      | Required | Values | Description |
    | :---        |    :----:   |          :---: | :---|
    | `annual_rate`      | Y       | example: 0.06   | interest rate per annum (reducing interest rate), it's divided by 12 to calculate monthly interest |
    | `months`      | Y       | example: 60   | loan duration in months |
    | `loan_amount`      | Y       | example: 100,000   | loan amount |
    | `balloon_payment_at_end`      | N       | example: 20,000 <br>default value = 0   | If there is large payment at the end of the loan |
    | `type`      | N       | 0 or 1 (0 = end of month, 1 = beginning of month) <br>default value = 0   | Whether payments are made at the beginning of the month or end of the month |
    | `cols_order`      | N       | {"Month", "Monthly Payment", "Principal", "Interest"} <br>default value = all columns  | An array of columns to be displayed. Columns will appear in the same sequence as defined in the array. <br>Possible values are "Month","Monthly Payment","Interest","Principal","Opening Balance","Ending Balance","Cumulative Interest","Cumulative Principal" |
    | `rows_order`      | N       | {5, 3} <br>default value = All rows from 1 to total number of months  | An array of rows to be displayed. Rows will appear in the same sequence as defined in the array. |

    **Usage**:
    - Full schedule:
    >```=JZ.Loan_Schedule(0.12, 60, 100000)``` 
    - Selected columns:
    >```=JZ.Loan_Schedule(0.12, 60, 100000,,,{"Month","Monthly Payment", "Principal", "Interest", "Ending Balance"})``` 
    - Rearranged columns:
    >```=JZ.Loan_Schedule(0.12, 60, 100000,,,{"Month","Interest", "Principal", "Monthly Payment", "Ending Balance"})```
    - First and last month:
    >```=JZ.Loan_Schedule(0.12, 60, 100000,,,,{1, 60})```
    - End of each year:
    >```=JZ.Loan_Schedule(0.12, 60, 100000,,,,{12, 24, 36, 48, 60})```
    - Outstanding balance at the end of each year:
    >```=JZ.Loan_Schedule(0.12, 60, 100000,,,{"Month","Ending Balance"},{12, 24, 36, 48, 60})```
    - Cumulative Interest paid till end of 27th month:
    >```=JZ.Loan_Schedule(0.12, 60, 100000,,,{"Cumulative Interest"},{27})```