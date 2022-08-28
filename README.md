# Описание
Распределения ингредиентов на порции

# Локация дефекта
![image](https://user-images.githubusercontent.com/94808944/187080987-9b353715-9627-435c-8dfb-1d34a60e48f1.png)

# Шаги воспроизведения

1. Открыть код программы (https://github.com/Bikokli/resipeTesting/blob/main/src/com/company/Main.java) в IDEA
1. Выставить значение переменной water (миллилитров воды) - 3000
1. Выставить значение переменной potatoes ( картофелин) - 5
1. Выставить значение переменной chicken (куриных бёдер) - 6
1. Выставить значение переменной spices(специй) - 10
1. Запустить программу
1. Посмотреть на вывод в консоли

*Ожидаемый результат:* все ингредиенты делятся по ровну на кол-во порций

*Фактический результат:* так как переменая int работает с целыми числами, при делении на значение типа int, остаток от деления округляется до целого значения, что искажает результаты подсчета!
В место int подошел бы тип float, так как он работает с дробными числами

# Скриншот
    [Ссылка на дефект](https://github.com/Bikokli/resipeTesting/blob/4bdd1a5241a02e6902e20bc3abf29187bb9c763b/src/com/company/Main.java#L10)
   
# Окружение
* **Операционная система** Windows 11
* **IDE** IntelliJ IDEA 2020
* **Java** OpenJDK11
