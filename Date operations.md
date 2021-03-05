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
