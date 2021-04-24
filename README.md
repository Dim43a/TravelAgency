# Travel-agency
OO analüüs, disain ja programmeerimine 
Бюро путешествий организовывает поездки для групп состоящих из различного 
количества людей. 
Цель данной работы: составить программу, моделирующую работу бюро путешествий 
(сохранение и обработка данных для пакетов путешествий).
Программа должна соответствовать приведенным ниже требованиям, даже если они 
кажутся странными. 

1. У каждого пакета путешествий имеется тип (например, “suusareis”, “Saaremaareis”, 
“Tallinnaekskursioon”), длительность в часах, стоимость для одного клиента и 
максимальное количество людей в группе (например, в автобус помещается 40 человек). 
Для каждого пакета должна быть возможность следующих операций: 

• запрос типа пакета
• запрос длительности путешествия
• запрос стоимости путешествия для одного участника
• запрос максимального количества участников в группе
• возможность установить стоимость путешествия для одного клиента
• метод, который получает в качестве входного аргумента количество людей и 
проверяет, подходит ли данный пакет для группы с таким количеством людей
• метод, который получает в качестве входного аргумента количество людей и 
возвращает вычисленную общую стоимость путешествия для данного количества 
людей; eсли количество людей (входной параметр) превышает максимальное 
количество людей в группе, то (используя предыдущий метод) возращается 
значение -1
• возможность представить информацию о пакете путешествия в текстовом виде 
(переопределить метод ToString()); eсли длительность поездки больше, чем 24 
часа, то длительность поездки отобразить в количестве полных суток.

2. Спецпакет путешествия – это производный класс от предыдущего. 
Дополнительно к имеющимся возможностям необходимо реализовать:

• скидку (%), действующую для больших групп

• количество людей, начиная с которого действует скидка
Например, стоимость пакета для одного клиента 20 евро. 
Если пакет заказывается для количества людей больше 10 (количество людей, начиная с 
которого действует скидка), то применятся скидка 10 процентов.

• при создании Спецпакета (в конструкторе) проверяется, что количество людей, 
начиная с которого действует скидка, не превышает максимальное количество 
людей в группе; если превышает, то количество людей, начиная с которого 
действует скидка, приравнивается максимальному количеству людей в группе

• метод, который получает в качестве входного аргумента количество людей и 
возвращает вычисленную общую стоимость путешествия для данного количества 
людей; eсли количество людей (входной параметр) превышает максимальное 
количество людей в группе, то (используя предыдущий метод) возращается 
значение -1; метод применяет скидку, если количество людей соответствует 
правилам начисления скидки

• возможность представить информацию о пакете путешествия в текстовом виде 
(переопределить метод ToString() – использовать метод родительского класса и 
отобразить информацию о скидке )

3. Создать тестовый класс с методом Main(). 
Создать коллекцию, содержащую пакеты путешествий разных типов (как обычные пакеты, 
так и спецпакеты). Продемонстрировать работу всех методов. 
Если результаты работы методов зависят от каких-то условий, то продемонстрировать работу 
методов для всех условий
