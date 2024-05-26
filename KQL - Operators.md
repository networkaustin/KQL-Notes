- `from` operator - Used to select a table
	- You can also use just the name of the table to select it
	- `from [table]`
- `project` operator - Select specific fields or columns 
	- This query will select data from rows in `column1` and `column2`
```kusto
from Table
| project column1,column2
```
- `where` operator - Used to specify a filter condition
	- This query will select all values from `column1` and `column2` while the values from `column 1` are below 100
```kusto
from Table
| project column1,column2
| where column1 > 100
```

- `count` operator - used to count total rows from query
	- Will return a count of total rows selected by query
```kusto
from Table
| project column1,column2
| where column1 > 100
| count
```
## Tags
#kql