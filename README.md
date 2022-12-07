
# Test_BIM_FDS
Задача:
-------

На входе у вас есть BIM-модель в Revit (вы можете использовать модель из стандартных примеров Revit'а).

Необходимо получить из готовой BIM модели здания в Revit выгрузить следующие данные:
1. Геометрию здания (как вариант можно через gbXML, пример файла выгрузки: https://github.com/lotus-uems/Test_BIM_FDS/blob/main/ExerciseFacility.xml)
2. Добавленные дополнительно в BIM-модель объекты: человек, датчик, пожарный выход (вы можете добавить для теста любые 3 объекта)

Решение:
-------

1. - revit_base_file.rvt - исходный файл проекта Revit
   - solution1.xml - геометрия объекта через bgxml
   
![img](https://github.com/devdenh/Test_BIM_FDS_Solution/blob/main/my_three_objects.png) 

2. - solution2.txt - координаты в формате json моих 3х добавленных объектов (element.getlocation) через Dynamo
   - logic.dyn - логика выбора добавленных элементов через семейство

![img](https://github.com/devdenh/Test_BIM_FDS_Solution/blob/main/solution2.png)
