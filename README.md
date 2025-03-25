## Диаграмма классов для задания Практика «Скользящее среднее»
![дк 2 1](https://github.com/user-attachments/assets/15fa2a86-cf4a-4419-b78c-7018aca2f595)


### Описание основных сущностей

- *DataPoint*
  - DataPoint(double x, double y): Конструктор для создания точки данных.
  - DataPoint(DataPoint point): Конструктор для копирования точки данных.
  - WithExpSmoothedY(double expSmoothedY): Создает новый экземпляр DataPoint с заданным сглаженным значением по экспоненциальному методу.
  - WithAvgSmoothedY(double avgSmoothedY): Создает новый экземпляр DataPoint с заданным сглаженным значением по методу скользящего среднего.
  - WithMaxY(double maxY): Создает новый экземпляр DataPoint с заданным максимальным значением.

- *MovingAverageTask*
  - MovingAverage(this IEnumerable data, int windowWidth): Вычисляет скользящее среднее последовательности точек данных с заданной шириной окна.

- *Queue*
  - Queue(): Конструктор для создания пустой очереди.
  - Enqueue(T item): Добавляет элемент в конец очереди.
  - Dequeue(): Удаляет элемент из начала очереди.
  - Count: Возвращает количество элементов в очереди.
