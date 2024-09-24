Дисциплина: Технологии индустриального программирования

Институт: Институт перспективных технологий и индустриального программирования

Кафедра: Индустриального программирования

Преподаватель: Адышкин Сергей Сергеевич

Студент группы ЭФМО-02-24: Курнаков Кирилл Александрович

Практическая работа 3 (Диаграмма классов для библиотеки)

Пользователь авторизовывается в системе. В зависимости от типа пользователя (Библиотекарь или читатель) пользователь попадает в систему.
Класс Библиотекарь (librarian) наследуется от класса пользователь (user). Библиотекарь может добавить новую книгу в систему (если такой книги еще нет в системе), удалить существующую книгу (если она не арендована читателем) и изменить данные о книге (если она не арендована читателем).
В классе Книга (book) содержатся все необходимые данные о книге(название, дата публикации, количество страниц, жанр, статус аренды (1 арендована, 0- арендована).
Класс Читатель (reader) наследуется от класса пользователь. В классе читатель хранится список арендованных книг. Читатель может взять книгу в аренду (если она не арендована другим пользователем и у читателя нет штрафов на текущий момент), вернуть книгу в библиотеку (при возврате будет проверка истечения срока возврата. Если срок возрата превышен, штраф автоматически будет рассчитан и выставлен читателю в зависимости от количества дней просрочки). Читатель может оплатить штраф (при успешной оплате штрафа статус штрафа меняется на "Оплачен"). 
Класс Штраф (fine) хранит информацию о штрафах читателей.


Библиотекарь внес все книги, которые доступны для аренды. 

(Читатель сдал в срок)
Читатель арендует книгу 24.09.2024 и указывает, что вернет книгу через 10 дней, то есть 4.10.2024. В список арендованных пользователем книг добавляется выбранная книга, статус книги меняется на "арендована" и создается новая запись об аренде книги с указанием выбранной книги, даты аренды, количества дней, читателем. Читатель приходит через 9 дней и сдает книгу. При сдаче книги в методе "calculateFine" класса "rent" проверяется срок возврата. Так как читатель вернул книгу в срок, то штраф не выписывается. Статус книги меняется на "Доступна к аренде".

(Читатель не сдал в срок)
Читатель арендует книгу 24.09.2024 и указывает, что вернет книгу через 10 дней, то есть 4.10.2024. В список арендованных пользователем книг добавляется выбранная книга, статус книги меняется на "арендована" и создается новая запись об аренде книги с указанием выбранной книги, даты аренды, количества дней, читателем. Читатель приходит через 15 дней и сдает книгу. При сдаче книги в методе "calculateFine" класса "rent" проверяется срок возврата. Читатель просрочил срок сдачи киниг на 5 дней, в связи с этим читателю выставляется штраф в размере 100 рублей. Статус книги меняется на "Доступна к аренде". После оплаты штрафа статус штрафа изменяется на "оплачено" и читатель вновь может брать книги.


![image](https://github.com/user-attachments/assets/238d46ae-7a9e-4886-ac7c-ea4f466cab80)
