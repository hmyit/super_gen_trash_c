﻿# super_gen_trash_c

Всем привет.

В одном крипторе увидел неплохой генератор мусорного кода на си, генератор реально крутой, но детектился антивирусами.

Решил его немного модифицировать, что сделал:

1)Во первых генерируются inline функции, да увеличит вес, но почти 8К строк запутает реверсера и антивирус.)

2)Генерируется заголовочный файл, который можно подцепить куда-нужно.

3)Разное вхождение в ветки, в зависимости от параметра.

Как использовать:

1.В \super_gen_trash_c\super_tresh_c\Release запустить super_tresh_c.exe

2.Появится файл с мусором trash.h, его и можно использовать.

3.Пример использования:

Инициализация генератора случайных чисел:

srand(time(0));

Получение рандомного i, для случайного попадания в ветки:

int i = 1 + rand() % 255;

Запускаем мусорный код :)

int result_i = tresh_gen(i);

В репозитории есть пример:\super_gen_trash_c\super_tresh_c\Release\EXAMPLE.exe

