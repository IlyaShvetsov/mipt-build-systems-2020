# Задание

## Необходимо создать структуру проекта в CMake, поддерживающую следующие возможности


### Алгоритм действия:
Исходный код лежит в трех папках A, B, C.
В папке А лежит скрипт на питоне, preparing.py, который генерирует хедер index.h.
В папке B лежит библиотека со своим собственным CMakeLists.txt, главный хедер - lib.h.
В папке С лежит два файла main.h и main.cpp, в main.h есть строчка #include "A/index.h" и строчка "include "B/lib.h".
После сборки проекта:
Должна быть создана папка bin, в которой должен быть лежать исполняемый файл C с главной точкой входа main.cpp
должна быть создана папка lib, в которой должны лежать собранные динамические библиотеки.

## Параметры запуска сборки проекта
Один из вариантов сборки проекта будет запускаться следующими командами:

mkdir build
cd build
cmake ..
make



При этом пользователь может в каком-угодно месте создать папку для сборки, используйте переменную для сборки проекта.

