# Генетический алгоритм оптимизации портфеля

Этот проект реализует генетический алгоритм для оптимизации распределения портфеля между несколькими акциями с целью максимизации доходности.

## Введение

Генетический алгоритм является эффективным методом поиска оптимального решения в пространстве переменных, учитывая определенные ограничения. В данном случае, мы стремимся распределить портфель между несколькими акциями с учетом указанных ограничений:

Ни одна из акций не может иметь 0 процентов в распределении.
Сумма процентов распределения по акциям должна быть равна 100.
Описание алгоритма
Инициализация первоначальной популяции: Создание начальной группы особей, каждая из которых представляет собой набор переменных, отражающих процентное распределение портфеля между акциями.

## Оценка приспособленности
Для каждой особи вычисляется доходность портфеля в соответствии с ее распределением акций.

## Формирование новой популяции

### Турнирная селекция
Две случайные особи соревнуются, выбирается лучшая для перехода в следующее поколение.
### Рулетка (пропорциональная селекция)
Особи выбираются пропорционально их приспособленности (доходности портфеля).
### Кроссовер
Две особи скрещиваются, создавая новые комбинации переменных.
### Мутация
Изменение случайных переменных в особи для разнообразия новой популяции.
Повторение алгоритма: Эти шаги повторяются некоторое количество раз или до достижения определенного условия останова.

## Завершение
Получение наилучшей особи (распределения портфеля), обеспечивающей максимальную доходность.

## Использование
Установите необходимые зависимости.
Задайте начальные параметры для алгоритма (количество особей, количество итераций и т.д.).
Запустите генетический алгоритм для оптимизации портфеля.
Примеры
Пример использования алгоритма для оптимизации портфеля можно найти в файле example.py.

## Зависимости
Python 3.x
Библиотеки: numpy, matplotlib (для визуализации, если требуется).
Вклад
Любые вопросы, предложения или улучшения приветствуются! Не стесняйтесь вносить свой вклад через pull request.

## Авторы
Ваше имя или контактная информация
Лицензия
Этот проект лицензирован в соответствии с лицензией MIT License.
