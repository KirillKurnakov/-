Дисциплина: Технологии индустриального программирования

Институт: Институт перспективных технологий и индустриального программирования

Кафедра: Индустриального программирования

Преподаватель: Адышкин Сергей Сергеевич

Студент группы ЭФМО-02-24: Курнаков Кирилл Александрович

Практическая работа 1 (Логическая и физическая модель БД)
  
  **Описание проекта**
Название проекта: "Интернет-магазин подарков и сувениров". В интернет-магазине будут продаваться оригинальные и интересные
подарки для различных мероприятий (дни рождения, праздники и тд).

Логическая модель базы данных
![image](https://github.com/user-attachments/assets/92432650-6dca-4210-a27d-5730e2a51f8f)

Физическая модель базы данных с указанием типов данных атрибутов
![image](https://github.com/user-attachments/assets/4ff4c596-171a-4dd4-a6fb-12b34b2b680d)

Описание сущностей
 1. Category (Категория товара) - сущность, которая представляет информацию о категории товара (кружка, тетрадь, блокнот и тд).
 2. Item (Товар) - сущность, которая представляет информацию о продаваемом товаре (категорию товара, цену, описание, количество товара на складе).
 3. Review (Отзыв) - сущность, которая представляет информацию об отзыве на определенный товар.
 4. User (Пользователь) - сущность, которая представляет информацию о пользователе интернет-магазина (фамилия, имя, контакты и тип пользователя).
 5. Type_User (Тип пользователя) - сущность, которая представляет информацию о типе пользователя интернет-магазина (пользователь, администратор).
 6. Gift_Box (Подарочная упаковка) - сущность, которая представляет информацию о подарочной упаковке к товару с указанием цены.
 7. Order_Item (Строка заказа) - сущность, которая представляет информацию о строке определенного заказа (товар, количество, цена, упаковка).
 8. Order (Заказ) - сущность, которая представляет информацию о заказе клиента (дату заказа, тип доставки, цену, статус заказа).
 9. Payment (Оплата) - сущность, которая представляет информацию об оплате заказа (дата платежа, сумма, подтверждение платежа).
 10. Delivery (Доставка) - сущность, которая представляет информацию о типе доставки (самовывоз, доставка, экспресс-доставка).
 11. Status_order (Статус заказа) - сущность, которая представляет информацию о статусе заказа (ожидает оплаты, оплачен, в доставке, доставлен).
 12. Type_payment (Тип оплаты) - сущность, которая представляет информацию о типе оплаты (наличные деньги, карта, СБП).
