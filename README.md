# Тестирование "ВИЗЫ В РОССИЮ"
### 1. Заказ приглашения в Россию
> Изменение цены в Туристической визе
1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. Выбрать тип визы - Туристическая.
3. Выбрать кратность - Однократная.
4. Выбрать каждое количество гостей (1, 2, 3, 4, от 5 до 19, 20) с каждым параметром в строке “Готовность через”".

| Ожидаемый результат | Статус |
| ------ | ------ |
| Цена меняется при каждом изменении | Выполнено |

> Проверка полей в Деловой визе при изменении кратности
1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. Выбрать тип визы - Деловая.
3. Выбрать кратность однократная.

| Ожидаемый результат | Статус |
| ------ | ------ |
| В блоке “Готовность через" отображаются кнопки “14 - 22 дней”, “11-13 дней” и “7-10 дней” | Выполнено |

### 2. Данные гостей

> Проверка количества полей для заполнения (блок “Гость”) в зависимости от разного выбора гостей.
1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. выбрать количество гостей N.

| Ожидаемый результат | Статус |
| ------ | ------ |
| В блоке "Данные гостей" находится N блоков гостя. Над каждый блоком написан номер гостя | Выполнено |
> "Проверка полей “Имя” и “Фамилия” в блоке “Данные гостей”
```sh
Предварительные шаги:
Заполнить все поля, кроме тестируемых, корректной информацией.
````

1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. Ввести имя "Иван" фамилия "Иванов".
3. Нажать кнопку "Получить визовое приглашение".
4. В открывшейся странице проверить имя и фамилию под надписью "Проверить введенные данные".

| Ожидаемый результат | Статус |
| ------ | ------ |
| Данные сохраняются и отображаются корректно | Выполнено |
| Больше одного пробела подряд между символами стираются, остается один пробел | Выполнено |
| Пробелы вначале и в конце имени и фамилии удаляются | Выполнено |
> Проверка выбора пола
```sh
Предварительные шаги:
Заполнить все поля, кроме тестируемых, корректной информацией.
```
1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. В поле "Пол" выбрать (М/Ж).
3. Нажать кнопку “Получить визовое приглашение”.
4. В открывшейся странице нажать на имя и фамилию под надписью "Проверить введенные данные".
5. В открывшемся окне проверить пол.

| Ожидаемый результат | Статус |
| ------ | ------ |
| Пол (М/Ж) | Выполнено |

> Проверка Даты рождения
```sh
Предварительные шаги:
Заполнить все поля, кроме тестируемых, корректной информацией.
```
1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. В поле "Дата рождения" вписать корректную дату 01.01.1990.
3. Выбрать следующее поле.
4. Нажать кнопку “Получить визовое приглашение”.
5. В открывшейся странице нажать на имя и фамилию под надписью "Проверить введенные данные".
6. В открывшемся окне сравнить дату рождения с вписанной датой.

| Ожидаемый результат | Статус |
| ------ | ------ |
| Дата принята | Выполнено |

1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. В поле "Дата рождения" написать 01.01.1700.
3. Выбрать следующее поле.

| Ожидаемый результат | Статус |
| ------ | ------ |
| Сообщение об ошибке: Введите корректную дату рождения | `Не Выполнено` |

1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. В поле "Дата рождения" написать 01.01.2019
3. Выбрать следующее поле.

| Ожидаемый результат | Статус |
| ------ | ------ |
| Сообщение об ошибке: Введите корректную дату рождения | Выполнено |

1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. В поле "Дата рождения" написать сегодняшнюю дату.
3. Выбрать следующее поле.

| Ожидаемый результат | Статус |
| ------ | ------ |
| Дата принята | `Не Выполнено` |

> Гражданство
```sh
Предварительные шаги:
Заполнить все поля, кроме тестируемых, корректной информацией.
```

1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. В поле "Гражданство" из выпадающего списка выбрать страну для которых не нужна виза для посещения России. К таким странам относится, например: Абхазия, Армения, Черногория и т.д.

| Ожидаемый результат | Статус |
| ------ | ------ |
| Появляется сообщение: Вам не нужна виза для посещения России | Выполнено |

> Запрос визового приглашения

1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. В поле "Гражданство" из выпадающего списка выбрать страну для которых документы оформляются под запрос. К таким странам относится, например: Албания, Алжир, Мавритания и т.д. 
3. Нажать кнопку "Отправить заявку на приглашение".
4. Заполнить поле Имя - Иван.
5. `Некорректно` заполнить поле Email - "Почта123".
6. Нажать кнопку "Запросить".

| Ожидаемый результат | Статус |
| ------ | ------ |
| Сообщение об ошибке: введите корректный Email | `Не Выполнено` |

1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. В поле "Гражданство" из выпадающего списка выбрать страну для которых документы оформляются под запрос. К таким странам относится, например: Албания, Алжир, Мавритания и т.д. 
3. Нажать кнопку "Отправить заявку на приглашение".
4. Заполнить поле Имя - Иван.
5. Заполнить поле Email - Test@mail.ru.
6. `Некорректно` заполнить поле Телефон - 555-123456.
7. Нажать кнопку "Запросить".
8. Закрыть окно нажатием на крестик".

| Ожидаемый результат | Статус |
| ------ | ------ |
| Окно закрывается | `Не Выполнено` |

> Номер паспорта
```sh
Предварительные шаги:
Заполнить все поля, кроме тестируемых, корректной информацией.
```
1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. В поле "Номер паспорта" написать - "мдкфорч543535".
3. Нажать кнопку “Получить визовое приглашение”.
4. В открывшейся странице нажать на имя и фамилию под надписью "Проверить введенные данные".
5. В открывшемся окне сравнить номер паспорта с указанными нами данными.

| Ожидаемый результат | Статус |
| ------ | ------ |
| Номер паспорта совпадает | Выполнено |

### 3. Маршрут поездки
> Города посещения и места пребывания в России
```sh
Предварительные шаги:
Заполнить все поля, кроме тестируемых, корректной информацией.
```
1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. Выбрать тип визы - туристическая.
3. Нажать кнопку "+ Город".

| Ожидаемый результат | Статус |
| ------ | ------ |
| Появляется еще одно поле для ввода города и гостиницы | Выполнено |

1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. Выбрать тип визы - туристическая.
3. Создать больше одного города посещения.
3. Нажать кнопку "Удалить город".

| Ожидаемый результат | Статус |
| ------ | ------ |
| Последнее поле города удаляется | Выполнено |

### 4. Доставка и контактная информация
> Ваш Email
```sh
Предварительные шаги:
Заполнить все поля, кроме тестируемых, корректной информацией.
```
1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. Выбрать тип визы - туристическая.
3. В поле Ваш Email указать - Test@mail.ru.
5. Нажать кнопку “Получить визовое приглашение”.

| Ожидаемый результат | Статус |
| ------ | ------ |
| Email принят | Выполнено |

> Другие способы доставки
1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. Выбрать тип визы - туристическая.
3. В блоке "Другие способы доставки" выбрать "Факс".

| Ожидаемый результат | Статус |
| ------ | ------ |
| Появилоссь поле для заполнение данных факса |`Не Выполнено` |

1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. Выбрать тип визы - туристическая.
3. В блоке "Другие способы доставки" выбрать "Почта".

| Ожидаемый результат | Статус |
| ------ | ------ |
| Появилоссь поле для заполнение данных почты | `Не Выполнено` |

### 5. Итоговая стоимость
> Цена
```sh
Предварительные шаги:
Заполнить все поля, кроме тестируемых, корректной информацией.
```
1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. В поле гражданство выбрать миграционно опасную страну.

| Ожидаемый результат | Статус |
| ------ | ------ |
| В разделе Итоговая стоимость появилась дополнительная строка "наценка за миграционную опасность" | Выполнено |

### 6. Заказ визового приглашения в Россию
> Пустые поля
1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. Оставить все поля пустыми.
3. Нажать кнопку "Получить визовое приглашение"

| Ожидаемый результат | Статус |
| ------ | ------ |
| Поля подсвечиваются красным | Выполнено |

### 7. Оплата банковской картой
> Оплата
```sh
Предварительные шаги:
Заполнить все поля, кроме тестируемых, корректной информацией.
```
1. Открыть ссылку https://preview-broken-in-u5auzt.bronevik.com/ru/info/russian-visa-invitation/
2. Нажать кнопку "Оплатить банковской картой".

| Ожидаемый результат | Статус |
| ------ | ------ |
| Открылось окно оплаты банковской картой | `Не Выполнено` |

### 8. Страница заказа
> Отмена визового приглашения
```sh
Предварительные шаги:
Заполнить все поля, кроме тестируемых, корректной информацией.
```
1. Нажать на выделенные слова "Этой ссылке"
2. Подтвердить действие.

| Ожидаемый результат | Статус |
| ------ | ------ |
| Ваш заказ аннулирован | Выполнено |

### 9. Место работы
> Проверка места работы
```sh
Предварительные шаги:
Заполнить все поля, кроме тестируемых, корректной информацией.
```
1. Ввести место работы - "Работа".
2. Адрес работы - "Адрес".
3. Рабочий телефон - 654-321.
4. Нажать кнопку “Получить визовое приглашение”.
5. В открывшейся странице нажать на имя и фамилию под надписью "Проверить введенные данные".
6. В открывшемся окне сравнить введенные данные.

| Ожидаемый результат | Статус |
| ------ | ------ |
| Данные совпадают | Выполнено |

# Итоговый отчёт

| Объект проверки | Описание | Статус |
| ------ | ------ | ------ |
| Заказ приглашения в Россию | Изменение цены в Туристической визе | Выполнено |
|  | Проверка полей в Деловой визе при изменении кратности | Выполнено |
| Данные гостей | Проверка количества полей для заполнения (блок “Гость”) в зависимости от выбора количества гостей. | Выполнено |
|  | Проверка полей “Имя” и “Фамилия” в блоке “Данные гостей” | Выполнено |
|  | Проверка выбора пола | Выполнено |
|  | Проверка Даты рождения | `Не Выполнено` |
|  | Гражданство | Выполнено |
|  | Запрос визового приглашения | `Не Выполнено` |
|  | Номер паспорта | Выполнено |
| Маршрут поездки | Города посещения и места пребывания в России | Выполнено |
| Доставка и контактная информация | Ваш Email | Выполнено |
|  | Другие способы доставки | `Не Выполнено` |
| Итоговая стоимость | Цена | Выполнено |
| Заказ визового приглашения в Россию | Пустые поля | Выполнено |
| Оплата банковской картой | Оплата | `Не Выполнено` |
| Страница заказа | Отмена визового приглашения | Выполнено |
| Место работы | Проверка места работы | Выполнено |

# Рекомендации
1) Внимательнее отнестись к обработке некорректно введённых данных.
2) Уведомлять пользователя о невозможности некоторых частей сервиса.
3) Разбить 1 большу форму на несколько подформ, для более интерактивно-понятного использования.
4) Сделать акцент на информационном блоке справа, при выборе разного типа виз "Туристическая" или "Деловая"
