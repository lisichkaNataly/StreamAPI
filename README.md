# StreamAPI
решение задач с применением StreamAPI и Optional
1. Написан метод findMinMax, находящий в стриме минимальный и максимальный элементы в соответствии порядком, заданным Comparator'ом.
Данный метод принимает на вход 3 элемента:
- Stream<? extends T> stream,
- Comparator<? super T> order,
- BiConsumer<? super T, ? super T> minMaxConsumer
Найденные минимальный и максимальный элементы передайте в minMaxConsumer следующим образом:
- minMaxConsumer.accept(min, max);
Если стрим не содержит элементов, то вызовите
minMaxConsumer.accept(null, null);

- Реализация через коллекцию(Например List или Queue)
- Логически верно определили результат
- Корректное получение необходимых данных
- Соблюден кодстайл

2. Реализован метод, который принимает на вход Список целых чисел и определяет количество четных и выводит их в консоль. Решено с применением Stream API
- Соблюден кодстайл
- Правильно реализован предикат
