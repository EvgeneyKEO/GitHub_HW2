### :large_blue_diamond: **_GitHub. HW_2_**
__________________________________________________________________________
**_Part 1. На локальном репозитории сделать ветки для:_**
- Postman						       
- Jmeter						       
- CheckLists						       
- Bag Reports								
- SQL
- Charles
- Mobile testing
1.
 1.1. Создать на GitHub репозитрой, в котором будут располагаться ветки [HW_31_group](https://github.com/EvgeneyKEO/HW_31_group.git)
 
 1.2. Клонируем внешний репозиторий на локальный репозиторий 
```
git clone https://github.com/EvgeneyKEO/HW_31_group.git
```
 1.3. Заходим в склонированный репозиторий 
 ```
 cd HW_31_group/
 ```
 1.4. Создаем ветки Postman, Jmeter, CheckLists, Bag Reports, SQL, Charles, Mobile testing:
``` 
git branch Postman
git branch Jmeter
git branch CheckLists
git branch SQL
git branch Charles
git branch Mobile_testing
``` 
      
**_Part 2. Запушить все ветки на внешний репозиторий_**
```
git push -u origin Postman
git push -u origin Jmeter
git push -u origin CheckLists
git push -u origin BagReports
git push -u origin SQL
git push -u origin Charles
git push -u origin Mobile_testing
```

**_Part 3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта_**
```
git checkout BagReports
cat >>  bagrep.txt --> добавляем структуру баг репорта
нажимаем ctrl+c
```
      
**_Part 4. Запушить структуру багрепорта на внешний репозиторий_**
```
git add . && git commit -m "add new file" && git push
```

**_Part 5. Вмержить ветку Bag Reports в Main_**
```
git checkout main
git merge BagReports
```
      
**_Part 6. Запушить main на внешний репозиторий._**
```
git push -u origin main
```

**_Part 7. В ветке CheckLists набросать структуру чек листа_**
```
git checkout CheckLists
cat >> CheckLists.json
забиваем структуру чек-листа в формате JSON
```

**_Part 8. Запушить структуру на внешний репозиторий_**
```
git add . && git commit -m "add new file" && git push
```

**_Part 9. На внешнем репозитории сделать Pull Request ветки CheckLists в main_**
```
Переходим на внешний репозиторий в ветку CheckLists, нажимаем кнопку Compare&pull requset
```

**_Part 10. Синхронизировать Внешнюю и Локальную ветки Main_**
```
git checkout main
git fetch - просмотрим действительно ли были какие-то изменения на внешнем репозитории
git pull
```
