Создание архива
Чтобы создать новый архив необходимо воспользоваться классом ZipOutputStream. Вот список методов, которые могут понадобиться:
•	setLevel - установка уровня компрессии от 0 до 9, где 9 - максимальная компрессия;
•	putNextEntry - вызывается перед записью нового объекта в архив, с указанием имени объекта;
•	closeEntry - вызываем после записи объекта. putNextEntry автоматически вызывает метод closeEntry.
•	close - закрываем поток.
Небольшой пример - создадим архив с названием archive.zip, в котором будут находиться сжатые файлы из директории folder. В этом примере пустые директории будут игнорироваться. Уровень компрессии явно не задан, поєтому будет использоваться значение по-умолчанию
