## Get first day of month

```python
import datetime 
todayDate = datetime.date.today()
if todayDate.day > 25:
    todayDate += datetime.timedelta(7)
print todayDate.replace(day=1)
```
## Get current date

```python
from datetime import date
today = date.today()
print("Current date =", today)
```
## Get current day, month and year

```python
from datetime import date
today = date.today() 

print("Current year:", today.year)
print("Current month:", today.month)
print("Current day:", today.day)
```

## Get yesterday date
```python
today = datetime.date.today()
yesterday = today - datetime.timedelta(days=1)
print(yesterday)
```

## Get current week start date
```python
from datetime import date, datetime, timedelta
start = date.today() - timedelta(days=date.today().weekday())
end = start + timedelta(days=6)
```


day = '12/Oct/2013'
dt = datetime.strptime(day, '%d/%b/%Y')
start = dt - timedelta(days=dt.weekday())
end = start + timedelta(days=6)
print(start)
print(end)

## Given a date, get week start and end
Example with DD/MM/YYYY date format input
```python

from datetime import datetime, timedelta
day = '14/11/2000'
dt = datetime.strptime(day, '%d/%m/%Y')
start = dt - timedelta(days=dt.weekday())
end = start + timedelta(days=6)
print(start)
print(end)
```
Output: 
```python
2000-11-13 00:00:00
2000-11-19 00:00:00
```
Example with YYYY-MM-DD date format input
```python
day = '2020-12-31'
dt = datetime.strptime(day, '%Y-%m-%d')
start = dt - timedelta(days=dt.weekday())
end = start + timedelta(days=6)
print(start)
print(end)
```
Output: 
```python
2020-12-28 00:00:00
2021-01-03 00:00:00
```
