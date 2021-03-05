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
