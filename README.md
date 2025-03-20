# DocPlusDB v1.6.0

## Описание
Является Пет-проектом, разработанным для облегчения рабочих процессов и структурированию данных. Написан на Python с использованием библиотек "psycopg2" для работы с базой данных и "PyQt5" для создания интерфейса. База данных разработана и администрируется в PostgreSQL, и настроена на доступ всем локальным машинам.

"DocPlusDB" - это программное обеспечение с пользовательским интерфесом включающим в себя базу данных медицинского оборудования. Имеет фильтры поиска по адресам/типу/наименованию и возможность добавления оборудования в пару кликов. Имеет две версии: пользовательскую и сервисную.

<details><summary><b>Инструкция</b></summary>

Программа состоит из двух вкладок:
1. Вкладка Оборудования
2. Вкладка журнала
   
1. Вкладка Оборудования состоит из блоков:
   1.1 Блок Поиска (Верхний)
   1.2. Блок Добавлений (Нижний)

   1.1 Блок Поиска состоит из:
      1.1.1. Трех зависимых друг от друга ячеек фильтров с выпадающими вариантами
      1.1.2. Редактируемой строкой
      1.1.3. Кнопки "Поиск"
      1.1.4. Кнопки "Очистить"
      1.1.5. Таблицы

Для формирования таблицы необходимо выставить фильтры в блоке поиска (по-умолчанию стоит фильтр "Всё"). Если выбран фильтр "По имени", то активируется редактируемая строка и в нее необходимо ввести наименования оборудования. Редактируемая строка имеет функцию выпадающих подсказок. Далее необходимо нажать на кнопку "Сформировать" для формирования таблицы. Кнопка "Очистить" нужна для удаления данных из таблицы (Не из базы данных).

   1.2 Блок добавления состоит из:
      1.2.1. Двух зависимых друг от друга ячеек фильтров с выпадающими вариантами - "Адрес" и "Кабинет"
      1.2.2. Одной независимой ячейки фильтра с выпадающими вариантами - "Тип оборудования"
      1.2.3. Трема редактируемыми строками -
         1.2.3.1. "Наименование"(С функцией выпадающих подсказок)
         1.2.3.2. "Серийный номер"
         1.2.3.3. "Год выпуска"
      1.2.4. Кнопки "Добавить"
      1.2.5. Кнопки "Очистить"

!!!Внимание!!!
Блок добавления активен только администратору.

Для добавления оборудования в базу данных необходимо заполнить все ячейки, ячейка "Год выпуска" принимает только целочисленные значения. Если будут заполненны не все ячейки - появится предупреждение. После заполнения необходимо нажать на кнопку "Добавить", после чего появится окно подверждения. В окне подтверждения необходимо выбрать "ОК" или "Cansel", взависимости от вашей решительности. Если вы подтвердили свое действие кнопкой "ОК", то появится следующее информативное окно, сообщающее об успешности операции.

В начале кода находятся настройки ваше БД

</details>

<details><summary><b>Стэк</b></summary>


-  Python
  
-  PostgreDB
  
</details>

<details><summary><b>Скриншоты</b></summary>

![Image alt](https://github.com/GarvelLoken1/DocPlusDB/raw/main/DocPlusDB1.jpg "Окно аутентификации") 

|*Скриншот окна аутентификации*|

![Image alt](https://github.com/GarvelLoken1/DocPlusDB/raw/main/DocPlusDB2.jpg "Окно БД") 

|*Скриншот окна базы данных*|

![Image alt](https://github.com/GarvelLoken1/DocPlusDB/raw/main/DocPlusDB3.jpg "Окно журнала") 

|*Скриншот окна журнала*|

![Image alt](https://github.com/GarvelLoken1/DocPlusDB/raw/main/DocPlusDB4.jpg "Окно оборудования") 

|*Скриншот окна оборудования*|

![Image alt](https://github.com/GarvelLoken1/DocPlusDB/raw/main/DocPlusDB5.jpg "Окно добавления работ") 

|*Скриншот окна добавления работ*|

</details>


