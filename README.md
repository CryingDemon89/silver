1. Платформа Java: Java Development Kit (JDK): состав, назначение. Кроссплатформенность языка Java. 
Java Development Kit (JDK) - основной комплект инструментов для разработки приложений на языке программирования Java. Он включает в себя все необходимые компоненты для создания, компиляции и отладки программ  
Состав:  
-Java Runtime Environment (JRE): среда выполнения Java, которая необходима для запуска Java-приложений. Включает в себя Java Virtual Machine (JVM), библиотеку классов и другие компоненты, необходимые для выполнения Java-программ. 
-Компилятор (javac): инструмент, который компилирует исходный код на языке Java (файлы с расширением .java) в байт-код (файлы с расширением .class), который может быть выполнен JVM. 
-Библиотеки классов: JDK включает стандартные библиотеки Java 
Назначение:  
Предназначен для предоставления всех необходимых инструментов и библиотек для компиляции исходного кода, запуска и отладки программ, создания документации, упаковки приложений в JAR-файлы (архивные файлы, которые используются для упаковки и распространения java программ), разработки приложений для различных платформ 
Кроссплатформенность языка Java. 
Одним из ключевых преимуществ языка Java является его кроссплатформенность. Это означает, что программы, написанные на Java, могут выполняться на различных операционных системах без необходимости изменения кода 


2. Java virtual machine (JVM), JIT-компилятор – определение, свойства, функции.Принципы работы сборщика мусора. 
Java virtual machine (JVM) — основная часть платформы Java Runtime Environment, которая интерпретирует байт-код Java для запуска программ.
Функции:  
-Позволяет запускать программы, написанные на Java, на любых устройствах и операционных системах. 
-Управляет и оптимизирует память, которую используют программы
Свойства: позволяет запускать Java-программы на любом устройстве или в любой операционной системе, обеспечивает управление памятью и платформенную независимость в различных аппаратных средствах и операционных системах. 
JIT-компилятор отвечает за преобразование байткода Java в нативный машинный код во время выполнения. Он компилирует часто вызываемые методы, кэширует скомпилированный код и повторно использует его при последующих выполнениях, снижая затраты на повторную интерпретацию байткода
Функции:  
-Оптимизация производительности  
-Снижение времени выполнения  
-Преобразование байт-кода в оптимизированный машинный код .
Свойства:  
-Оптимизация: использует различные методы оптимизации, что позволяет повысить производительность 
-Кэширование: код может быть кэширован для повторного использования, что ускоряет выполнение часто вызываемых методов  
-Адаптивность: может адаптироваться к поведению программы, компилируя наиболее часто используемые методы.
Принципы работы сборщика мусора: он удаляет объекты, которые больше не используются программой, и восстанавливает память, которую они занимали. Процесс включает несколько этапов:
-Инициализация — проверка состояния памяти, определение надобности в очистке.
-Идентификация живых объектов, или маркировка — сборщик находит и помечает все объекты, которые могут быть достигнуты из корней (активные потоки, локальные переменные в стеке, специальные объекты Java VM и другие).
-Удаление мёртвых объектов — сборщик освобождает все фрагменты памяти, которые не были промаркированы на предыдущем этапе.
-Компактизация — это уплотнение памяти с целью уменьшения её фрагментации. То есть при компактизации оставшиеся объекты располагаются в начале кучи непрерывно.
***Сборка мусора выполняется в JVM автоматически через определённые отрезки времени и не требует отдельного внимания 
 
3. Системы сборки проектов. Фреймворк Apache Maven: определение, структура, Maven Coordinates, POM-файл. 
Системы сборки проектов - инструменты, которые автоматизируют процесс компиляции, тестирования, упаковки и развертывания программного обеспечения. Помогают управлять зависимостями, конфигурациями и процессами сборки 
Фреймворк Apache Maven - инструмент управления проектами и системой сборки, который основан на концепции "управления проектом через описание". Maven использует файл конфигурации (POM), в котором описываются все аспекты проекта, включая зависимости, плагины и цели сборки. 
Структура:  
–pom.xml: основной файл конфигурации проекта, в котором описаны зависимости, плагины и другие настройки. 
–src/main/java: каталог для исходного кода приложения. 
–src/main/resources: каталог для ресурсов (например, конфигурационных файлов). 
–src/test/java: каталог для тестов. 
–src/test/resources: каталог для ресурсов, используемых в тестах. 
Maven Coordinates - уникальный идентификатор для каждой зависимости в Maven. Он состоит из четырех основных компонентов:  
groupId - уникальный идентификатор группы или организации, которая разрабатывает артефакт  
artifactId -  уникальный идентификатор самого артефакта 
version - версия артефакта 
packaging - тип пакета 

  
4. Типы данных Java: простые и ссылочные. Простые (примитивные) типы данных. 
Простые типы данные - основные типы данных, которые существуют в Java. Они используются для представления простых значений, таких как числа, символы и логические значения  
-Boolean: представляет значение true или false. 
-int: представляет 32-битное число, которое может хранить значение 
-long: представляет собой 64-битное целое число, 
-float: представляет 32-битное число с плавающей запятой одинарной точности
-double - представляется 64-битное число с плавающей запятой двойной токи, 
Ссылочные типы данных - типы данных, которые используются для хранения ссылок на объекты, а не фактического значения объекта; Ссылочная переменная содержит адрес памяти объекта, наиболее распространенным ссылочным типом данных является объект 
-Массив: набор похожих типов данных любого типа, например, int[], String[], Object []. 
-Строка: последовательность символов. Пример: String e = “hello.”; 
-Объект: экземпляр класса, базовая единица данных, которую можно использовать для хранения данных. Пример: Employee employee = new Employee(1, “new”); 

 
5. Переменные: статические и нестатические. Местные переменные, область видимости переменных. Объявление и инициализация переменных. Константы. Спецификаторы доступа. 
Переменные в Java бывают трёх типов:
-Локальные. Объявляются в методах, блоках или конструкторах. Создаются, когда метод, блок или конструктор запускаются, и уничтожаются после завершения метода, конструктора либо блока. Видимы лишь в пределах объявленного метода, блока либо конструктора.
-Переменные экземпляра (локал переменные). Объявляются на уровне класса, до или после использования. Являются видимыми для всех методов, конструкторов и блоков в классе. Пример: int a, b, c;
-Статические переменные (переменные класса). Объявляются с использованием ключевого слова static внутри класса вне какого-либо метода, конструктора или блока. В отличие от переменных экземпляра, у статической переменной может быть только одна копия для каждого класса, независимо от того, сколько объектов создано. Статические переменные создаются в начале выполнения программы и автоматически уничтожаются по окончании выполнения. Пример: public static int my_number = 100; 
Объявление переменной в Java - указание её имени и типа данных. Инициализация - присваивание переменной начального значения. Для инициализации переменной используется оператор присваивания
Константы в Java - переменные, обозначенные специальным словом — final. Константы никогда не меняются от первоначального значения. Пример: final int const = 10;  
Модификаторы доступа - ключевые слова, которые регулируют уровень доступа к разным частям кода. В Java их четыре: private, default, protected, public  
-private - наиболее строгий модификатор доступа. Он ограничивает видимость данных и методов за пределами одного класса. 
-default (иногда называют package visible). Он не обозначается ключевым словом, установлен по умолчанию для всех полей и методов. Если спецификатор не указан, то доступен только внутри того же пакета 
-public - модификатор, который доступен из любого другого класса. 
-protected - модификатор, обозначающий, что он будет виден в пределах всех классов, находящихся в том же пакете, что и пакет, в котором объявлена переменная или в пределах всех классов-наследников (доступен внутри того же пакета и в подклассах)


6. Комментарии: виды, особенности применения. 
Комментарии в Java делятся на два типа:
-Комментарии реализации (кода). Используются для описания отдельных строк или блоков кода. Бывают строчными (описываются в одну строку) и блочными (описываются целым блоком, так как не помещаются в одну строку).
-Javadoc-комментарии. Поясняют, зачем создан тот или иной класс и пакет и что делает тот или иной метод. начинаются с /** и применяются для генерации документации. Включают теги (например, @param, @return): 
Особенности применения комментариев:
–Однострочные комментарии используются для описания функциональности кода. Начинаются с двух косых черт (//). 
–Многострочные комментарии применяются, когда нужно добавить информацию в исходный код, которая превышает одну строку. Выглядит как /* …… */
–Комментарии для документации( используются, когда нужно предоставить информацию для инструмента javadoc для создания HTML-документации для классов на основе чтения исходного кода.  


7. Операции языка Java – арифметические, отношения и логические, преобразования числовых типов. 
Арифметические операции: +, -, *, /, % для основных математических действий, включая остаток от деления. 
Операции отношений: ==, !=, <, >, <=, >= для сравнения значений. 
Логические операции: && (логическое И), || (логическое ИЛИ), ! (логическое НЕ) используются для работы с логическими значениями. 
Преобразование числовых типов: 
Неявное преобразование (widening): типы меньшей емкости, такие как int, могут быть преобразованы в типы большей емкости, например, long. 
Явное преобразование (casting): преобразование типов вручную, например, (int) 2.5. 


8. Символьные строки, методы работы со строками Java. 
Строки в Java представлены объектами класса String. Строка - неизменяемый объект, который хранит последовательность символов. 
Некоторые методы работы со строками в Java: 
-Получение длины строки (метод length()). 
-Получение символа в строке по его индексу (метод charAt()). 
-Конкатенация строк (метод concat() и оператор + для объединения двух строк). 
-Сравнение строк (методы equals() и equalsIgnoreCase()). 
-Извлечение подстроки (метод substring()). 
-Преобразование строки в нижний или верхний регистр (методы toLowerCase() и toUpperCase()). 
-Удаление начальных и конечных пробелов (метод trim()). 
-Разделение строки на массив подстрок (метод split()). 
-Замена символов или подстрок (методы replace() и replaceAll()). 
***Для изменения строк в Java рекомендуется использовать классы StringBuilder и StringBuffer, которые позволяют изменять строки без создания новых объектов. 
