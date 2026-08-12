# java-core-training
Проект-тренажер для разработки и тестирования
## Цель проекта
Попрактиковать Java Core и продемонстрировать навыки автоматизации тестирования:
- Решение алгоритмических задач
- Написание модульных тестов
- Настройка CI/CD (GitHub Actions)
- Генерация отчётов Allure
- Базовые UI-тесты (Selenium)
- Работа с БД (JDBC)

## Список задач (Java Core)
<a name="table-of-contents"></a>
* [FizzBuzz](#task-1)
* [Перевернуть строку (Reverse String)](#task-2)
* [Проверка на палиндром (Palindrome Check)](#task-3)
* [Найти дубликаты в массиве/списке (Find Duplicates in Array/List)](#task-4)
* [Посчитать количество вхождений символа в строке (Count Character Occurrences)](#task-5)
* [Удалить дубликаты из списка (Remove Duplicates from List)](#task-6)
* [Проверка на анаграммы (Anagram Check)](#task-7)
* [Найти первый неповторяющийся символ в строке (Find First Non-Repeating Character)](#task-8)
* [Факториал числа (Factorial)](#task-9)
* [Найти второй по величине элемент в массиве/списке (Find Second Largest Element)](#task-10)
* [Проверка сбалансированности скобок (Balanced Parentheses Check)](#task-11)
* [Найти пару чисел в массиве, сумма которых равна заданному значению (Two Sum Problem)](#task-12)
* [Найти самый часто встречающийся элемент в массиве/списке (Find Most Frequent Element)](#task-13)
* [Группировка элементов списка по какому-либо признаку (Group List Elements)](#task-14)
* [Реализовать `equals()` и `hashCode()` для кастомного класса](#task-15)
* [Создание простого Singleton (Implement Singleton)](#task-16)
* [Создать Immutable класс (Create Immutable Class)](#task-17)
* [Сравнить два объекта кастомного класса (Compare Custom Objects)](#task-18)
* [Базовая валидация формата Email (Basic Email Format Validation)](#task-19)
* [Прочитать файл и посчитать строки/слова (Read File and Count Lines/Words)](#task-20)

---

## Список задач (UI-автотесты на Selenium)

<a name="table-of-contents-ui"></a>
* [Checkboxes](#task-ui-1)
* [Dropdown](#task-ui-2)
* [JavaScript Alerts](#task-ui-3)
* [Dynamic Controls](#task-ui-4)
* [Drag and Drop](#task-ui-5)

---

## Задания (Java Core)

<a name="task-1"></a>

### FizzBuzz

* **Описание:** Написать программу, которая выводит числа от 1 до N. Но для чисел, кратных 3, вывести "Fizz", для чисел,
  кратных 5 - "Buzz", а для чисел, кратных и 3, и 5 - "FizzBuzz". (Проверяет: циклы, условия)
* **Задание:** Напишите метод, например `generateFizzBuzz(int n)`, который принимает целое число n и возвращает
  последовательность FizzBuzz от 1 до n в виде списка строк (List<String>).
* **Пример:** Вызов `generateFizzBuzz(15)` должен вернуть список строк, эквивалентный: `List.of("1", "2", "Fizz", "4", "
  Buzz", "Fizz", "7", "8", "Fizz", "Buzz", "11", "Fizz", "13", "14", "FizzBuzz")`
* **Решение:**
  [`FizzBuzz.java`](),
  [`FizzBuzzTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-2"></a>

### Перевернуть строку (Reverse String)

* **Описание:** Написать функцию, которая принимает строку и возвращает её в перевернутом виде. (Проверяет: работа со
  строками, циклы/рекурсия/StringBuilder)
* **Задание:** Напишите метод `String reverseString(String str)`, который принимает строку и возвращает новую
  строку, являющуюся перевернутой версией исходной.
* **Пример:** `reverseString("hello")` -> `"olleh"`, `reverseString("Java")` -> `"avaJ"`.
* **Решение:**
  [`ReverseString.java`](),
  [`ReverseStringTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-3"></a>

### Проверка на палиндром (Palindrome Check)

* **Описание:** Написать функцию, которая проверяет, является ли строка палиндромом (читается одинаково слева направо и
  справа налево), игнорируя регистр и не буквенно-цифровые символы. (Проверяет: работа со строками, циклы, условия)
* **Задание:** Напишите метод `boolean isPalindrome(String str)`, который возвращает `true`, если строка `str`
  является палиндромом (игнорируя регистр и не буквенно-цифровые символы), и `false` в противном случае.
* **Пример:** `isPalindrome("A man, a plan, a canal: Panama")` -> `true`, `isPalindrome("race a car")` -> `false`,
  `isPalindrome(" ")` -> `true`.
* **Решение:**
  [`PalindromeCheck.java`](),
  [`PalindromeCheckTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-4"></a>

### Найти дубликаты в массиве/списке (Find Duplicates in Array/List)

* **Описание:** Написать функцию, которая находит и возвращает дублирующиеся элементы в массиве или списке целых
  чисел/строк. (Проверяет: работа с коллекциями, Set/Map, циклы)
* **Задание:** Напишите метод `List<Integer> findDuplicates(List<Integer> numbers)`, который принимает список целых
  чисел и возвращает список уникальных чисел, которые встречаются в исходном списке более одного раза.
* **Пример:** `findDuplicates(List.of(1, 2, 3, 2, 4, 5, 1, 5))` -> `[1, 2, 5]` (порядок не важен, можно вернуть
  `Set`).
* **Решение:**
  [`FindDuplicatesList.java`](),
  [`FindDuplicatesListTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-5"></a>

### Посчитать количество вхождений символа в строке (Count Character Occurrences)

* **Описание:** Написать функцию, которая подсчитывает, сколько раз каждый символ встречается в строке. (Проверяет:
  работа со строками, Map, циклы)
* **Задание:** Напишите метод `Map<Character, Integer> countCharacters(String str)`, который возвращает Map, где
  ключами являются символы из строки `str`, а значениями - количество их вхождений.
* **Пример:** `countCharacters("hello world")` ->
  `{'h': 1, 'e': 1, 'l': 3, 'o': 2, ' ': 1, 'w': 1, 'r': 1, 'd': 1}`.
* **Решение:**
  [`CountCharOccurrences.java`](),
  [`CountCharOccurrencesTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-6"></a>

### Удалить дубликаты из списка (Remove Duplicates from List)

* **Описание:** Написать функцию, которая принимает список и возвращает новый список без дубликатов. (Проверяет: работа
  с коллекциями, Set, циклы)
* **Задание:** Напишите метод `List<String> removeDuplicates(List<String> list)`, который принимает список строк и
  возвращает новый список, содержащий только уникальные строки из исходного списка, сохраняя порядок первого
  вхождения.
* **Пример:** `removeDuplicates(List.of("a", "b", "a", "c", "b"))` -> `["a", "b", "c"]`.
* **Решение:**
  [`RemoveDuplicatesList.java`](),
  [`RemoveDuplicatesListTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-7"></a>

### Проверка на анаграммы (Anagram Check)

* **Описание:** Написать функцию, которая проверяет, являются ли две строки анаграммами друг друга (состоят из одних и
  тех же символов в разном порядке). (Проверяет: работа со строками, сортировка/Map, сравнение)
* **Задание:** Напишите метод `boolean areAnagrams(String str1, String str2)`, который возвращает `true`, если
  строки `str1` и `str2` являются анаграммами (игнорируя регистр и пробелы), и `false` иначе.
* **Пример:** `areAnagrams("listen", "silent")` -> `true`, `areAnagrams("Dormitory", "dirty room")` -> `true`,
  `areAnagrams("hello", "world")` -> `false`.
* **Решение:**
  [`AnagramCheck.java`](),
  [`AnagramCheckTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-8"></a>

### Найти первый неповторяющийся символ в строке (Find First Non-Repeating Character)

* **Описание:** Написать функцию, которая находит первый символ в строке, который встречается только один раз. (
  Проверяет: работа со строками, Map/массивы для счетчиков, циклы)
* **Задание:** Напишите метод `Character findFirstNonRepeatingChar(String str)`, который находит и возвращает первый
  символ в строке `str`, который встречается только один раз. Если такого символа нет, верните null или выбросите
  исключение.
* **Пример:** `findFirstNonRepeatingChar("swiss")` -> `'w'`, `findFirstNonRepeatingChar("aabbcc")` -> `null`.
* **Решение:**
  [`FindFirstNonRepeatingChar.java`](),
  [`FindFirstNonRepeatingCharTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-9"></a>

### Факториал числа (Factorial)

* **Описание:** Написать функцию для вычисления факториала числа (итеративно или рекурсивно).
  (Проверяет: циклы/рекурсия, арифметика)
* **Задание:** Напишите метод `long factorial(int n)`, который вычисляет факториал неотрицательного целого числа
  `n`. Реализуйте итеративно.
* **Пример:** `factorial(5)` -> `120`, `factorial(0)` -> `1`.
* **Решение:**
  [`Factorial.java`](),
  [`FactorialTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-10"></a>

### Найти второй по величине элемент в массиве/списке (Find Second Largest Element)

* **Описание:** Написать функцию для поиска второго максимального элемента. (Проверяет: циклы, сравнения, обработка
  крайних случаев)
* **Задание:** Напишите метод `int findSecondLargest(int[] numbers)`, который находит и возвращает второе по
  величине число в массиве `numbers`. Если такого элемента нет (например, все элементы одинаковы или массив слишком
  мал), верните `Integer.MIN_VALUE` или выбросите исключение.
* **Пример:** `findSecondLargest(new int[]{1, 5, 2, 9, 3, 9})` -> `5`. `findSecondLargest(new int[]{3, 3, 3})` ->
  `Integer.MIN_VALUE`.
* **Решение:**
  [`FindSecondLargest.java`](),
  [`FindSecondLargestTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-11"></a>

### Проверка сбалансированности скобок (Balanced Parentheses Check)

* **Описание:** Проверить, правильно ли расставлены скобки `()`, `{}`, `[]` в строке. (Проверяет: Stack, работа со
  строками, логика)
* **Задание:** Напишите метод `boolean areBracketsBalanced(String expression)`, который проверяет, правильно ли
  сбалансированы скобки `()`, `{}`, `[]` в строке `expression`.
* **Пример:** `areBracketsBalanced("({[]})")` -> `true`. `areBracketsBalanced("([)]")` -> `false`.
  `areBracketsBalanced("{[}")` -> `false`. `areBracketsBalanced("()")` -> `true`.
* **Решение:**
  [`BalancedParenthesesCheck.java`](),
  [`BalancedParenthesesCheckTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-12"></a>

### Найти пару чисел в массиве, сумма которых равна заданному значению (Two Sum Problem)

* **Описание:** Дан массив чисел и целевое значение. Найти два числа, которые в сумме дают это значение. (Проверяет:
  циклы, Map/Set, логика)
* **Задание:** Напишите метод `int[] findTwoSumIndices(int[] nums, int target)`, который принимает массив целых
  чисел `nums` и целевое значение `target`. Метод должен вернуть массив из двух индексов элементов, сумма которых
  равна `target`. Если такой пары нет, верните пустой массив или `null`. Предполагается, что решение единственное.
* **Пример:** `findTwoSumIndices(new int[]{2, 7, 11, 15}, 9)` -> `[0, 1]`.
  `findTwoSumIndices(new int[]{3, 2, 4}, 6)` -> `[1, 2]`.
* **Решение:**
  [`TwoSumProblem.java`](),
  [`TwoSumProblemTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-13"></a>

### Найти самый часто встречающийся элемент в массиве/списке (Find Most Frequent Element)

* **Описание:** Написать функцию для поиска элемента с максимальным числом вхождений. (Проверяет: Map, циклы, сравнения)
* **Задание:** Напишите метод `int findMostFrequentElement(int[] numbers)`, который находит и возвращает элемент,
  который встречается в массиве `numbers` чаще всего. Если таких элементов несколько, верните любой из них.
  Обработайте случай пустого массива.
* **Пример:** `findMostFrequentElement(new int[]{1, 3, 2, 1, 4, 1, 3})` -> `1`.
  `findMostFrequentElement(new int[]{1, 2, 3})` -> `1` (или `2`, или `3`).
* **Решение:**
  [`FindMostFrequentElement.java`]()
  [`FindMostFrequentElementTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-14"></a>

### Группировка элементов списка по какому-либо признаку (Group List Elements)

* **Описание:** Например, сгруппировать список строк по первой букве. (Проверяет: Map, циклы, работа с коллекциями)
* **Задание:** Напишите метод `Map<Integer, List<String>> groupStringsByLength(List<String> strings)`, который
  принимает список строк и возвращает `Map`, где ключи - это длина строки, а значения - списки строк этой длины.
* **Пример:** `groupStringsByLength(List.of("apple", "bat", "cat", "apricot", "ball"))` ->
  `{5: ["apple"], 3: ["bat", "cat"], 7: ["apricot"], 4: ["ball"]}`.
* **Решение:**
  [`GroupListElements.java`](),
  [`GroupListElementsTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-15"></a>

### Реализовать `equals()` и `hashCode()` для кастомного класса

* **Описание:** Объяснить контракт между ними. (Проверяет: ООП, контракты Java)
* **Задание:** Для класса `Point` с полями `int x` и `int y`, переопределите методы `equals(Object o)` и
  `hashCode()` так, чтобы они соответствовали контракту: равные объекты (`p1.x == p2.x && p1.y == p2.y`) должны
  иметь одинаковый `hashCode`.
* **Пример:** `new Point(1, 2).equals(new Point(1, 2))` -> `true`. `new Point(1, 2).equals(new Point(2, 1))` ->
  `false`. `new Point(1, 2).hashCode()` должен быть равен `new Point(1, 2).hashCode()`.
* **Решение:**
  [`EqualsHashCode.java`]()
  [`EqualsHashCodeTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-16"></a>

### Создание простого Singleton (Implement Singleton)

* **Описание:** Реализовать паттерн Singleton. (Проверяет: основы паттернов проектирования, статические члены,
  синхронизация - опционально)
* **Задание:** Реализуйте класс `Logger` как Singleton, используя статическое поле и приватный конструктор. Добавьте
  статический метод `getInstance()` для получения единственного экземпляра и метод `log(String message)`, который
  просто выводит сообщение в консоль.
* **Пример:** `Logger logger1 = Logger.getInstance(); Logger logger2 = Logger.getInstance(); logger1 == logger2` ->
  `true`. `logger1.log("Test message")` выводит "Test message".
* **Решение:**
  [`Singleton.java`]()
  [`SingletonTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-17"></a>

### Создать Immutable класс (Create Immutable Class)

* **Описание:** Написать класс, состояние которого нельзя изменить после создания. (Проверяет: ООП, `final`)
* **Задание:** Напишите класс `ImmutablePoint` с приватными `final` полями `x` и `y` типа `int`. Сделайте класс
  `final`, предоставьте только геттеры и конструктор, который инициализирует поля. Объясните, почему этот класс
  является неизменяемым.
* **Пример:** После `ImmutablePoint p = new ImmutablePoint(1, 2);`, состояние `p` изменить нельзя.
* **Решение:**
  [`ImmutableClass.java`]()
  [`ImmutableClassTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-18"></a>

### Сравнить два объекта кастомного класса (Compare Custom Objects)

* **Описание:** Реализовать интерфейс `Comparable` или предоставить `Comparator` для кастомного класса (например,
  `Person` по возрасту). (Проверяет: ООП, интерфейсы)
* **Задание:** Модифицируйте класс `Person` (с полями `name`, `age`), чтобы он реализовывал интерфейс
  `Comparable<Person>`. Сравнение должно происходить сначала по возрасту (по возрастанию), а при одинаковом
  возрасте - по имени (в алфавитном порядке).
* **Пример:** `Collections.sort(listOfPersons)` должен отсортировать список объектов `Person` согласно заданным
  правилам. `new Person("Bob", 30).compareTo(new Person("Alice", 30))` -> положительное число.
  `new Person("Alice", 25).compareTo(new Person("Bob", 30))` -> отрицательное число.
* **Решение:**
  [`CompareCustomObjects.java`]()
  [`CompareCustomObjectsTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-19"></a>

### Базовая валидация формата Email (Basic Email Format Validation)

* **Описание:** Очень упрощенная проверка наличия `@` и `.`. (Проверяет: работа со строками, `contains`/`indexOf`)
* **Задание:** Напишите метод `boolean isValidEmailBasic(String email)`, который выполняет очень простую проверку
  формата email: строка должна содержать один символ `@` и хотя бы одну точку `.` после символа `@`.
* **Пример:** `isValidEmailBasic("test@example.com")` -> `true`. `isValidEmailBasic("test.example.com")` -> `false`.
  `isValidEmailBasic("test@examplecom")` -> `false`. `isValidEmailBasic("test@@example.com")` -> `false`.
* **Решение:**
  [`BasicEmailValidation.java`]()
  [`BasicEmailValidationTest.java`]()

[К оглавлению](#table-of-contents)

---

<a name="task-20"></a>

### Прочитать файл и посчитать строки/слова (Read File and Count Lines/Words)

* **Описание:** Написать код, который читает текстовый файл и выводит количество строк или слов. (Проверяет: основы I/O,
  обработка исключений)
* **Задание:** Напишите метод `int countLines(String filePath)`, который читает текстовый файл по пути `filePath` и
  возвращает количество строк в нем. Обработайте возможные `IOException`. (На собеседовании могут попросить
  использовать `try-with-resources`).
* **Пример:** Если файл `data.txt` содержит 3 строки, `countLines("data.txt")` -> `3`.
* **Решение:**
  [`ReadFileCount.java`]()
  [`ReadFileCountTest.java`]()

[К оглавлению](#table-of-contents)

---

## Задания (UI-тесты)

Тестовый объект - [The Internet](https://the-internet.herokuapp.com/)

<a name="task-ui-1"></a>

### Checkboxes

* **Ссылка на страницу:** https://the-internet.herokuapp.com/checkboxes
* **Описание:** Страница с двумя чекбоксами. Нужно протестировать их начальное состояние, возможность изменения и корректность переключения. (Проверяет: работу с `WebElement`, методы `isSelected()`, `click()`, явные ожидания `WebDriverWait`.)
* **Задание:** Напишите класс страницы `CheckboxesPage` с методами для получения состояния каждого чекбокса и их переключения. Создайте тестовый класс `CheckboxesTest`, который:
  1. Проверяет, что по умолчанию первый чекбокс не выбран, второй выбран.
  2. Устанавливает первый чекбокс в состояние "выбран", второй – в "не выбран".
  3. Проверяет, что состояния изменились корректно.
* **Пример выполнения:** После выполнения тестов оба чекбокса должны быть в противоположном начальному состоянии, и все проверки должны проходить успешно.
* **Решение:**  
  [`CheckboxesPage.java`]()  
  [`CheckboxesTest.java`]()

[К оглавлению](#table-of-contents-ui)

---

<a name="task-ui-2"></a>

### Dropdown

* **Ссылка на страницу:** https://the-internet.herokuapp.com/dropdown
* **Описание:** Страница с выпадающим списком, содержащим опции "Please select an option", "Option 1", "Option 2". Нужно протестировать выбор опций и обработку невалидных значений. (Проверяет: использование класса `Select`, методы `selectByVisibleText()`, `selectByValue()`, работу с `List<WebElement>`.)
* **Задание:** Напишите класс страницы `DropdownPage` с методами для получения выбранной опции, выбора по тексту и по значению, а также для получения количества опций. Создайте тестовый класс `DropdownTest`, который:
  1. Проверяет, что по умолчанию выбрана опция "Please select an option".
  2. Выбирает "Option 1" и проверяет, что она выбрана.
  3. Выбирает "Option 2" и проверяет, что она выбрана.
  4. Проверяет, что в списке ровно 3 опции.
  5. Обрабатывает попытку выбрать несуществующую опцию (ожидается исключение).
* **Пример выполнения:** Все выборы должны проходить успешно, и результат проверок должен быть положительным.
* **Решение:**  
  [`DropdownPage.java`]()  
  [`DropdownTest.java`]()

[К оглавлению](#table-of-contents-ui)

---

<a name="task-ui-3"></a>

### JavaScript Alerts

* **Ссылка на страницу:** https://the-internet.herokuapp.com/javascript_alerts
* **Описание:** Страница с тремя кнопками, вызывающими разные JavaScript-диалоги: Alert, Confirm, Prompt. Нужно протестировать взаимодействие с ними и обработку результатов. (Проверяет: работу с интерфейсом `Alert`, методы `accept()`, `dismiss()`, `sendKeys()`, обработку исключений.)
* **Задание:** Напишите класс страницы `JavaScriptAlertsPage` с методами для нажатия на каждую кнопку и получения текста результата. Создайте тестовый класс `JavaScriptAlertsTest`, который:
  1. Нажимает на `JS Alert`, подтверждает его и проверяет, что на странице появился текст "You successfully clicked an alert".
  2. Нажимает на `JS Confirm`, подтверждает – проверяет "You clicked: Ok", затем отменяет – проверяет "You clicked: Cancel".
  3. Нажимает на `JS Prompt`, вводит текст "Hello Selenium!" и подтверждает – проверяет, что результат содержит этот текст.
  4. Нажимает на `JS Prompt`, отменяет – проверяет, что результат содержит "null".
* **Пример выполнения:** Все диалоги должны быть обработаны корректно, текст результата на странице должен соответствовать ожиданиям.
* **Решение:**  
  [`JavaScriptAlertsPage.java`]()  
  [`JavaScriptAlertsTest.java`]()

[К оглавлению](#table-of-contents-ui)

---

<a name="task-ui-4"></a>

### Dynamic Controls

* **Ссылка на страницу:** https://the-internet.herokuapp.com/dynamic_controls
* **Описание:** Страница с двумя динамическими элементами: чекбокс, который можно добавлять/удалять, и поле ввода, которое можно включать/отключать. Нужно протестировать их динамическое поведение. (Проверяет: явные ожидания (`ExpectedConditions`), работу с состояниями `isDisplayed()`, `isEnabled()`, ожидание исчезновения/появления элементов.)
* **Задание:** Напишите класс страницы `DynamicControlsPage` с методами для работы с чекбоксом и полем ввода. Создайте тестовый класс `DynamicControlsTest`, который:
  1. **Для чекбокса:**
     - Проверяет, что чекбокс присутствует на странице.
     - Нажимает кнопку `Remove` и ожидает, что чекбокс исчезнет.
     - Нажимает кнопку `Add` и ожидает, что чекбокс появится снова.
     - Проверяет, что текст кнопки меняется с "Remove" на "Add" и обратно.
  2. **Для поля ввода:**
     - Проверяет, что поле по умолчанию выключено (`isEnabled() == false`).
     - Нажимает `Enable` и ожидает, что поле станет активным (`isEnabled() == true`).
     - Вводит текст "Hello World!".
     - Нажимает `Disable` и проверяет, что поле снова выключено.
* **Пример выполнения:** Все ожидания должны сработать, и состояния элементов должны меняться согласно действиям.
* **Решение:**  
  [`DynamicControlsPage.java`]()  
  [`DynamicControlsTest.java`]()

[К оглавлению](#table-of-contents-ui)

---

<a name="task-ui-5"></a>

### Drag and Drop

* **Ссылка на страницу:** https://the-internet.herokuapp.com/drag_and_drop
* **Описание:** Страница с двумя блоками (A и B), которые можно перетаскивать друг на друга. Нужно протестировать, что при перетаскивании блоки меняются местами. (Проверяет: использование класса `Actions`, метод `dragAndDrop()`, проверку текста элементов после перемещения.)
* **Задание:** Напишите класс страницы `DragAndDropPage` с методами для получения текста левого и правого блоков и для выполнения перетаскивания с блока A на блок B. Создайте тестовый класс `DragAndDropTest`, который:
  1. Проверяет, что изначально левый блок содержит текст "A", правый – "B".
  2. Выполняет перетаскивание A на B.
  3. Проверяет, что после перетаскивания левый блок содержит "B", а правый – "A".
* **Пример выполнения:** После перетаскивания текст блоков должен поменяться местами, и проверки должны проходить успешно.
* **Решение:**  
  [`DragAndDropPage.java`]()  
  [`DragAndDropTest.java`]()

[К оглавлению](#table-of-contents-ui)
