# my_diplom_drf
## Азамат, приветствую Вас. Сдаю работу на проверку.
## Инструкция:

1.Скачиваем проект,  затем необходимо создать суперпользователя и сгенерировать ему токен:

python manage.py createsuperuser --email stas.ik1987@yandex.ru

python manage.py drf_create_token Admin

2. Затем создаем пользователей, минимум два (поставщик и покупатель). Для этого используем запросы 1-4 файла requests-examples.http. При этом генерируются токены и отправляются на почту.

3. Используя токены создаем контактные данные к этим пользователям (запросы 5 - 6 ).

4. Пользователь, которого мы принимаем за поставщика, создает магазин. (запросы 7 - 10). При этом все товары из прайса сразу загрузятся по ссылке. 

5. Используя запросы 11-1 - 11-6 покупатель просматривает товар.

6. После того как покупатель определился с товаром он копирует его external_id (считаем что он разный у всех товаров) и создает заказ используя запросы 12 - 14.

7. После того как покупатель создал заказ, его нужно подтвердить (запросы 15 - 16). Здесь отправляется письмо администратору для проверки.

8. Администратор, используя номер заказа из письма, проверяет заказ и отправляет его в доставку (запросы 17 - 18). После этого покупатель и продавец получат письма - продавец, что должен отправить товар по адресу, а покупатель что товар отправлен.

P.S. Сначала начал делать проект используя формы, достаточно много времени на это потратил. ТЗ так составлено, что кажется без форм не обойтись. Если интересно можно посмотреть https://github.com/StanislavGrekov/my_diplom
Там успел сделать формы для регистрации пользователей. Оставлю, может пригодиться в будущем.

