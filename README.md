# Тестовое задание
В представленном коде мы используем модель под названием DirectoryModel для представления и манипулирования древовидной структурой каталогов в базе данных.

Модель DirectoryModel определяет два метода: getDescendantsAsTree и getDescendantsAsFlatList. Метод getDescendantsAsTree извлекает всех потомков в виде древовидной структуры, а метод getDescendantsAsFlatList извлекает всех потомков в виде плоского списка.

Модель DirectoryModel использует одну таблицу базы данных под названием directories для хранения структуры дерева каталогов. Таблица имеет три столбца: id, name и parent_id. Столбец id является первичным ключом таблицы, а столбцы name и parent_id хранят имя каждого каталога и ID его родительского каталога соответственно.

Модель DirectoryModel использует расширение PDO для подключения к базе данных и выполнения SQL-запросов. Она также использует рекурсивную функцию getChildren для получения всех потомков каталога в виде древовидной структуры путем построения многомерного массива каталогов и их дочерних элементов.

В целом, модель DirectoryModel обеспечивает простой и эффективный способ представления и манипулирования древовидной структурой каталогов в базе данных с помощью PHP и SQL.
