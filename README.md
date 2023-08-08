# Homework  for Git @ Vadim Ksendzov's Course
## GitHub. HW_2

**1. На локальном репозитории сделать ветки для:**

**- Postman**

**- Jmeter**

**- CheckLists**

**- Bag Reports**

**- SQL**

**- Charles**

**- Mobile testing**

- `git branch Postman`
- `git branch Jmeter`
- `git branch CheckLists`
- `git branch Bag_Reports`
- `git branch SQL`
- `git branch Charles`
- `git branch Mobile_testing`

**2. Запушить все ветки на внешний репозиторий**
- `git push -u origin --all`

**3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта**
- `git checkout Bag_Reports`
```
vim BR_1.txt
i
ID - 503
Severity - Trivial
Environment- Samsung S20+ (Android 13 Chrome 11 ), Big Sur 11.7.7
Title- The texts "Trusted partner", "Powered by", "Group’s Parent Entity is audited by" at block "Partners" in Footer  is not translated into any languages except EN
Steps:
     1. Navigate to capital.com
     2. Selected language DE,RU.
     3. Hover over the menu section [More]
     4. Click on menu item  [Capital System status]
     5. Scroll to Tile  "Mobile App,Web....".

Expected Result- The tile "Mobile application, web...." translated into the selected language.
Actual Result- The name "Mobile application, web...."  not been translated into the selected language.
Comments- The bug is also reproduced for the mobile.
Attachment- https://drive.google.com/julia/...
ESC 
:wq
Enter
```

**4. Запушить структуру багрепорта на внешний репозиторий**
- `git add bag_report.txt`
- `git commit - m "add BR_1.txt"` 
- `git push`

**5. Вмержить ветку Bag Reports в Main**
- `git checkout Main`
- `git merge Bag_Reports`

**6. Запушить main на внешний репозиторий**
- `git add .`
- `git push -u origin main`

**7. В ветке CheckLists набросать структуру чек листа**
- `git checkout Checklists`
  
```
vim CheckListDraft.txt
i
Пример подробной структуры чек-листа для тестирования ПО, которая может быть дополнена и изменена в зависимости от потребностей и особенностей каждого проекта.
1. Описание продукта
- Понимание основной цели продукта
- Понимание целевой аудитории
- Описание основных функций продукта

2. Тест-кейсы
- Наличие тест-кейсов для каждой функции продукта
- Проверка тест-кейсов на полноту и достаточность
- Наличие документации для каждого тест-кейса

3. Функциональное тестирование
- Проверка работоспособности основных функций продукта
- Проверка работоспособности дополнительных функций продукта
- Проверка соответствия продукта требованиям

4. Тестирование совместимости
- Проверка совместимости продукта с различными операционными системами
- Проверка совместимости продукта с различными браузерами
- Проверка совместимости продукта с различными устройствами

5. Тестирование безопасности
- Проверка безопасности продукта
- Проверка уязвимостей продукта
- Проверка защиты от взлома и атак

6. Тестирование производительности
- Проверка производительности продукта при различных нагрузках
- Проверка времени отклика продукта
- Проверка запуска и завершения продукта

7. Тестирование пользовательского интерфейса
- Проверка пользовательского интерфейса на соответствие дизайну
- Проверка удобства использования пользовательского интерфейса
- Проверка наличия и правильности локализации

8. Тестирование документации
- Проверка наличия и полноты документации
- Проверка правильности и актуальности документации
- Проверка наличия руководства пользователя

9. Тестирование установки и обновления
- Проверка процесса установки продукта
- Проверка процесса обновления продукта
- Проверка совместимости установщика с различными операционными системами

10. Тестирование восстановления после сбоев
- Проверка восстановления продукта после сбоев и ошибок
- Проверка восстановления базы данных после сбоев и ошибок
- Проверка восстановления резервных копий после сбоев и ошибок
ESC 
:wq
Enter
```
**8. Запушить структуру на внешний репозиторий**
- `git add -A && git commit -m "add CheckListDraft.txt"`
- `git push`

**9. На внешнем репозитории сделать Pull Request ветки CheckLists в main**
![image](https://github.com/00Julie00/GitHub_HW/assets/115406267/422b6769-3047-4a29-a3e1-a0e42afd3ea5)

**10. Синхронизировать Внешнюю и Локальную ветки Main**
- `git pull`
