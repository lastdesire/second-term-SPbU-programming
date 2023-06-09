# Задание 2.1.
Реализовать контейнер использующий для хранения элементов кольцевой список. Контейнер обязан быть обобщенным (с помощью дженериков).

Для каждого метода нужно написать 1-2 тестовые функции. Написать тестирующую программу вызывающую эти тестовые функции по параметрам считанным из тестового файла. К проекту приложить не менее трех тестовых файлов.

# Требования по функционалу к кольцевому списку

Конструкторы:
  
- (!) CircleList<T>() – Инициализирует новый экземпляр пустого класса CircleList<T>. 
  
-  (*) CircleList<T>(IEnumerable<T>) – Инициализирует новый экземпляр класса CircleList<T>, содержащий элементы, скопированные из указанного класса IEnumerable, и обладающий емкостью, достаточной для того, чтобы вместить количество скопированных элементов.
  
Поля:

- (!) Count – Получает число узлов, которое в действительности хранится в CircleList<T>.

- (!) First – Получает первый узел объекта CircleList<T>.

- (!) Last – Получает последний узел объекта CircleList<T>.

Методы:

- (*) AddAfter(CircleListNode<T>, CircleListNode<T>) – Добавляет заданный новый узел после заданного существующего узла в CircleList<T>.

- (!) AddAfter(CircleListNode<T>, T) – Добавляет новый узел, содержащий заданное значение, после заданного существующего узла в CircleList<T>.

- (*) AddBefore(CircleListNode<T>, CircleListNode<T>) – Добавляет заданный новый узел перед заданным существующим узлом в CircleList<T>.

- (!) AddBefore(CircleListNode<T>, T) – Добавляет новый узел, содержащий заданное значение, перед заданным существующим узлом в CircleList<T>.

- (*) AddFirst(CircleListNode<T>)	 – Добавляет заданный новый узел в начало CircleList<T>.

- (!) AddFirst(T) – Добавляет новый узел, содержащий заданное значение, в начало CircleList<T>. 

- (*) AddLast(CircleListNode<T>)	 – Добавляет заданный новый узел в конец CircleList<T>.

- (!) AddLast(T) – Добавляет новый узел, содержащий заданное значение, в конец CircleList<T>.

- (!) Clear() – Удаляет все узлы из CircleList<T>.

- (!) Contains(T) – Определяет, принадлежит ли значение объекту CircleList<T>.

- ($) CopyTo(T[], Int32) – Копирует целый массив CircleList<T> в совместимый одномерный массив Array, начиная с заданного индекса целевого массива.

- (!) Equals(Object) – Определяет, равен ли указанный объект текущему объекту.

- (!) Find(T) – Находит первый узел, содержащий указанное значение.

- (!) FindLast(T) – Находит последний узел, содержащий указанное значение.

- ($) GetEnumerator() – Возвращает перечислитель, осуществляющий перебор элементов списка CircleList<T>.

- (*) GetType() – Возвращает объект Type для текущего экземпляра.

- ($) MemberwiseClone() – Создает неполную копию текущего объекта Object.

- (*) Remove(CircleListNode<T>)	 – Удаляет заданный узел из объекта CircleList<T>.

- (!) Remove(T) – Удаляет первое вхождение заданного значения из CircleList<T>.

- (!) RemoveFirst()	– Удаляет узел в начале CircleList<T>.

- (!) RemoveLast()	– Удаляет узел в конце CircleList<T>.

- ($) ToString() – Возвращает строку, представляющую текущий объект.
 
Методы расширения:

- ($) All<TSource>(IEnumerable<TSource>, Func<TSource,Boolean>)	–  Проверяет, все ли элементы последовательности удовлетворяют условию.

- (!) Any<TSource>(IEnumerable<TSource>) – Проверяет, содержит ли последовательность какие-либо элементы.

- ($) Any<TSource>(IEnumerable<TSource>, Func<TSource,Boolean>) Проверяет, удовлетворяет ли какой-либо элемент последовательности заданному условию.

- (*) Append<TSource>(IEnumerable<TSource>, TSource) – Добавляет значение в конец последовательности.

- (*) Concat<TSource>(IEnumerable<TSource>, IEnumerable<TSource>) – Объединяет две последовательности.

- (*) Contains<TSource>(IEnumerable<TSource>, TSource) – Определяет, содержится ли указанный элемент в последовательности, используя компаратор проверки на равенство по умолчанию.

- (!) Count<TSource>(IEnumerable<TSource>) – Возвращает количество элементов в последовательности.

- (*) Count<TSource>(IEnumerable<TSource>, Func<TSource,Boolean>) – Возвращает число, представляющее количество элементов последовательности, удовлетворяющих заданному условию.

- ($) Distinct<TSource>(IEnumerable<TSource>)	 – Возвращает различающиеся элементы последовательности, используя для сравнения значений компаратор проверки на равенство по умолчанию. 

- (*) ElementAt<TSource>(IEnumerable<TSource>, Index) – Возвращает элемент по указанному индексу в последовательности.

- (!) ElementAt<TSource>(IEnumerable<TSource>, Int32) – Возвращает элемент по указанному индексу в последовательности.

- (*) ElementAtOrDefault<TSource>(IEnumerable<TSource>, Index) – Возвращает элемент последовательности по указанному индексу или значение по умолчанию, если индекс вне допустимого диапазона.

- (!) ElementAtOrDefault<TSource>(IEnumerable<TSource>, Int32) – Возвращает элемент последовательности по указанному индексу или значение по умолчанию, если индекс вне допустимого диапазона.

- ($) Except<TSource>(IEnumerable<TSource>, IEnumerable<TSource>) – Находит разность множеств, представленных двумя последовательностями, используя для сравнения значений компаратор проверки на равенство по умолчанию.

- (!) First<TSource>(IEnumerable<TSource>) – Возвращает первый элемент последовательности.

- (*) FirstOrDefault<TSource>(IEnumerable<TSource>) – Возвращает первый элемент последовательности или значение по умолчанию, если последовательность не содержит элементов.

- ($) Intersect<TSource>(IEnumerable<TSource>, IEnumerable<TSource>) – Находит пересечение множеств, представленных двумя последовательностями, используя для сравнения значений компаратор проверки на равенство по умолчанию.

- (!) Last<TSource>(IEnumerable<TSource>) – Возвращает последний элемент последовательности.

- (*) LastOrDefault<TSource>(IEnumerable<TSource>) – Возвращает последний элемент последовательности или значение по умолчанию, если последовательность не содержит элементов.

- ($) LongCount<TSource>(IEnumerable<TSource>) – Возвращает значение типа Int64, представляющее общее число элементов в последовательности.

- (!) Max<TSource>(IEnumerable<TSource>) – Возвращает максимальное значение, содержащееся в универсальной последовательности.

- (!) Min<TSource>(IEnumerable<TSource>) – Возвращает минимальное значение, содержащееся в универсальной последовательности.

- (*) OrderBy<TSource,TKey>(IEnumerable<TSource>, Func<TSource,TKey>) –  Сортирует элементы последовательности в порядке возрастания ключа.

- ($) OrderBy<TSource,TKey>(IEnumerable<TSource>, Func<TSource,TKey>, IComparer<TKey>) – Сортирует элементы последовательности в порядке возрастания с использованием указанного компаратора.

- (*) OrderByDescending<TSource,TKey>(IEnumerable<TSource>, Func<TSource,TKey>) – Сортирует элементы последовательности в порядке убывания ключа.

- ($) OrderByDescending<TSource,TKey>(IEnumerable<TSource>, Func<TSource,TKey>, IComparer<TKey>) – Сортирует элементы последовательности в порядке убывания с использованием указанного компаратора.

- (*) Prepend<TSource>(IEnumerable<TSource>, TSource) – Добавляет значение в начало последовательности.

- (!) Reverse<TSource>(IEnumerable<TSource>) – Изменяет порядок элементов последовательности на противоположный.

- (*) SequenceEqual<TSource>(IEnumerable<TSource>, IEnumerable<TSource>) – Определяет, совпадают ли две последовательности, используя для сравнения элементов компаратор проверки на равенство по умолчанию, предназначенный для их типа.

- (*) Single<TSource>(IEnumerable<TSource>) –Возвращает единственный элемент последовательности и генерирует исключение, если число элементов последовательности отлично от 1.

- ($) SingleOrDefault<TSource>(IEnumerable<TSource>) – Возвращает единственный элемент последовательности или значение по умолчанию, если последовательность пуста; если в последовательности более одного элемента, генерируется исключение.

- (*) Take<TSource>(IEnumerable<TSource>, Int32) –Возвращает указанное число подряд идущих элементов с начала последовательности.

- ($) Take<TSource>(IEnumerable<TSource>, Range) – Возвращает указанный диапазон смежных элементов из последовательности.

- (*) TakeLast<TSource>(IEnumerable<TSource>, Int32) – Возвращает новую перечислимую коллекцию, содержащую последние count элементов из source.

- ($) Union<TSource>(IEnumerable<TSource>, IEnumerable<TSource>) – Находит объединение множеств, представленных двумя последовательностями, используя для сравнения значений компаратор проверки на равенство по умолчанию.

# Комментарий
Реализованы практически все требуемые методы и поля. К каждому из них написаны тесты. К каждому методу присутствует комментарий, поясняющий суть его работы.
