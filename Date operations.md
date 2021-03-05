## Get first day of month

```python
import datetime 
todayDate = datetime.date.today()
if todayDate.day > 25:
    todayDate += datetime.timedelta(7)
print todayDate.replace(day=1)
```
