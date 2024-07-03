# DocPlusDB v1.0.2

## Описание
Является Пет-проектом, разработанным для облегчения рабочих процессов и структурированию данных. "DocPlusDB" - это программное обеспечение с пользовательским интерфесом включающим в себя базу данных медицинского оборудования. Имеет фильтры поиска по адресам/типу/наименованию(в выпадающими строками) и возможность добавления оборудования в пару кликов. Имеет две версии: пользовательскую и сервисную. Проект внедрен и активно используется.

<details><summary><b>Инструкция</b></summary>

Программа состоит из двух блоков:
1. Блок Поиска (Верхний)
2. Блок Добавлений (Нижний)

Блок поиска состоит из:
1. Трех зависимых друг от друга ячеек фильтров с выпадающими вариантами
2. Редактируемой строкой
3. Кнопки "Поиск"
4. Кнопки "Очистить"
5. Таблицы

Для формирования таблицы необходимо выставить фильтры в блоке поиска (по-умолчанию стоит фильтр "Всё"). Если выбран фильтр "По имени", то активируется редактируемая строка и в нее необходимо ввести наименования оборудования. Редактируемая строка имеет функцию выпадающих подсказок. Далее необходимо нажать на кнопку "Поиск" для формирования таблицы. Кнопка "Очистить" нужна для удаления данных из таблицы (Не из базы данных).

Блок добавления состоит из:
1. Двух зависимых друг от друга ячеек фильтров с выпадающими вариантами - "Адрес" и "Кабинет"
2. Одной независимой ячейки фильтра с выпадающими вариантами - "Тип оборудования"
3. Трема редактируемыми строками -
   3.1. "Наименование"(С функцией выпадающих подсказок)
   3.2. "Серийный номер"
   3.3. "Год выпуска"
4. Кнопки "Добавить"
5. Кнопки "Очистить"

!!!Внимание!!!
Блок добавления активен только в сервисной версии.

Для добавления оборудования в базу данных необходимо заполнить все ячейки, ячейка "Год выпуска" принимает только целочисленные значения. Если будут заполненны не все ячейки - появится предупреждение. После заполнения необходимо нажать на кнопку "Добавить", после чего появится окно подверждения. В окне подтверждения необходимо выбрать "ОК" или "Cansel", взависимости от вашей решительности. Если вы подтвердили свое действие кнопкой "ОК", то появится следующее информативное окно, сообщающее об успешности операции.

В файле config.py находятся настройки подключения к БД

</details>

<details><summary><b>Стэк</b></summary>


-  Python
  
-  PostgreDB
  
</details>

<details><summary><b>Скриншоты</b></summary>

![Image alt](https://github.com/GarvelLoken1/DocPlusDB/raw/main/screenDocPlusDBClient.jpg "Пользовательская версия") 

|*Скриншот пользовательской версии*|

![Image alt](https://github.com/GarvelLoken1/DocPlusDB/raw/main/screenDocPlusDB.jpg "Сервисная версия") 

|*Скриншот сервисной версии*|

</details>


