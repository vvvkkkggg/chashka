#### Функциональные требования:

- Предоставлять мобильное приложение для клиентов кофеен
- Предоставлять мобильное приложение для сотрудников кофеен
- Предоставлять веб-страницу со статистикой работы программы лояльности для бизнеса
- По QR-коду получать информацию о покупке через API ФНС России
- Хранить информацию о пользователе: число баллов в программе лояльности по каждой кофейне
- Ранжировать кофейни по отзывам пользователей
- Предоставлять возможности брендирования страниц кофеен
- Идентифицировать, аутентифицировать и авторизовывать без номера телефона, почт, SSO

#### Нефункциональные требования:

- Покрытие серверами по всей России для geo-доставки контента пользователям. Крупнейшая в России сеть CDN
- Доступ 24/7 для покрытия всех часовых поясов (SLA 99.7%)
- Быстрый и удобный онбординг бизнеса. Подключение за 10 минут
- Оценка кофейни в один клик
- Хранение обезличенных данных, аутентификация по secret key и fingerprint
- Онбординг клиента кофейни прямо на кассе не более чем за минуту
- Процесс начисления бонусов лояльности не более чем за 30 секунд
    - Открытие приложения
    - Клик
    - Скан
    - Результат
- Приятная и узнаваемая айдентика, которой можно адаптировать под дизайн помещения, для распространения в рамочку на
  кассе

#### Диаграммa требований

![](sysml.jpg)

#### Диаграммa случаев использования

![](usercase.jpg)

#### Screen flow

Экран администратора
![](admin_screen.jpg)

Экран пользователя
![](user_screen.jpg)

#### Wireframe

![](gui.jpg)

#### Work Structure

![](workstructure.png)

#### Риски

| Риск                                          | Последствия                                               | Вероятность | Предотвращение                             | Устранение последствий                        |
|-----------------------------------------------|-----------------------------------------------------------|------------|--------------------------------------------|-----------------------------------------------|
| Отказ в публикации в App Store                | Невозможность обслуживать посетителей с iOS               | Средняя    | Изучить регламент                          | Сменить страну регистрации                    | 
| Падение сервисной экономики                   | Нет необходимости удерживать клиентов в сфере обслуживания | Низкая     | Диверсификация по странам                  | Банкротство или релокация                     |
| Коммодитизация бренда кофейни                 | Нет интереса от кофеен с сильным брендом                  | Высокая    | Кастомизация опыта клиента с кофейней      | Маркетинг, направленный на возвращение кофеен |
| Невозможность оперировать фискальными данными | Нельзя использовать API касс                              | Средняя    | Регистрация ИП <br> Соблюдение закона о ОФД | Удовлетворение требований регулятора          |
| Низкий ценовой сегмент ЦА                     | Ниже цена подписки <br> Слабее вирусный эффект            | Средняя    | Хороший UI/UX                              | Маркетинг, нацеленный на спешиалти сегмент    |
