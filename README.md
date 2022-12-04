# Домашнее задание к занятию "`9.3. Система мониторинга Zabbix. Часть 2 - Никулин Михаил`

---

### Задание 1

![Задание 1](img%2FTemplate.png)

---

### Задание 3

![Задание 2-3](img%2Fhosts_template.png)

---

### Задание 4

![Задание 4](img%2Fdashboard.png)

---

### Задание 5*

![task_5_1.png](img%2Ftask_5_1.png)
![Задание 5*](img%2Ftask_5.png)

---

### Задание 6*

![6_latest_data.png](img%2F6_latest_data.png)

```bash
#!/bin/bash

if [[ $1 -eq 1 ]]
then
  echo "Никулин Михаил Сергеевич"
elif [[ $1 -eq 2 ]]
then
  echo $(date "+%Y-%m-%d")
fi
```

---

### Задание 7*

```python
import sys
import os
import re
import datetime
if (sys.argv[1] == '-ping'): # Если -ping
 result=os.popen("ping -c 1 " + sys.argv[2]).read() # Делаем пинг по заданному адресу
 result=re.findall(r"time=(.*) ms", result) # Выдёргиваем из результата время
 print(result[0]) # Выводим результат в консоль
elif (sys.argv[1] == '-simple_print'): # Если simple_print
 print(sys.argv[2])
elif (sys.argv[1] == '1'):
 print("Никулин Михаил Сергеевич")
elif (sys.argv[1] == '2'):
 print(datetime.date.today())
else:
 print(f"unknown input: {sys.argv[1]}")
```
![7_latest_data.png](img%2F7_latest_data.png)

---

### Задание 8*

![Discovery.png](img%2FDiscovery.png)
![Discovery_hosts.png](img%2FDiscovery_hosts.png)
![Discovery_operations.png](img%2FDiscovery_operations.png)
![Discovery_rules.png](img%2FDiscovery_rules.png)

---

