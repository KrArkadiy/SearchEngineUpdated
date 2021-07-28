# SearchEngine
Передо мной была поставлена задача по созданию поисковика, который считывает данные с файла и затем можно осуществлять поиск по данным из файла, также реализовать стратегию поиска и консольное меню для пользователя.

#О программе SimpleEngine 

<p>#Архитектура</p> 
Поисковик построен на Java SE8. 

Поисковик имеет консольное меню, которое включает в себя также стратегии поиска. Для поиска используется алгоритм инвертированных индексов, т.е. после считывания предложение разделяется на отдельные слова, которые помещаются в HashMap, где слово это непосредтвенно ключ, а значением является число. И затем с использованием именно данных чисел происходит поиск. В данном приложении применен такой паттерн проектирования, как шаблон.

Исходный код состоит из нескольких пакетов: service, template, utility. В пакете service находятся классы: Menu - реализация консольного меню, Strategy - реализация выбора стратегии поиска, Runner - класс, метод которого осуществляет всю непобходимую логику, для запуска приложения. В пакете template находятся классы, которые необходимы для реализации паттерна шаблон. В пакете utility находятся вспомогательный методы. Точкой входа в приложение является класс SearchEngineApplication.

##Демонстрация знаний

Ввод-вывод из потока - BufferedReader, InputStreamReader.
Работа с коллекциями - ArrayList, HashMap.
Алгоритм поиска - инвертированные индексы.
Паттерны проектирования - Template.

Для запуска приложения необходимо:
1) Скопировать скопировать код, используя зеленую кнопку Code
2) Создать новый проект, используя опцию From Version Control
3) Запустить приложение, используя класс SearchEngineApplication.

В ближайшее время приложение будет покрыто тестами.
