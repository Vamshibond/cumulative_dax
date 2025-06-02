Cumulative Sales = 
CALCULATE(
    SUM('Sales'[SalesAmount]),
    FILTER(
        ALLSELECTED('Sales'[Date]),
        'Sales'[Date] <= MAX('Sales'[Date])
    )
)
