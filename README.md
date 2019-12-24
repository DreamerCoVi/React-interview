# JS

* Какие типы данных существуют в js?
* Чем отличаются var let const?
* Что такое области видимости?
* Что такое прототип объекта?
* Что такое редюсер? Приведите пример

# React

* Жизненные циклы компонента, в каком из них следует выполнять ajax-запросы?
* Что такое state и props? Как создать и изменить?
* Что такое и для чего нужны ref?
* Что такое и чем отличаются контролируемые и неконтролируемые компоненты?
* Для чего нужен и какие параметры принимает setState() ?

# Smarty (необязательно)

* Как задать и вывести значение переменной?
* Как подключить файл шаблона и передать в него параметры?
* Как вывести только четные элементы массива, выделив первый из них?
* Что такое и для чего нужен {block}? Приведите пример.
* Что такое модификаторы переменных? Как использовать, приведите пример.



<details>
<summary>Тестовое 1</summary>
Необходимо создать приложение-задачник.
Документацию по back-end можно найти тут:

https://uxcandy.com/~shapoval/test-task-backend/docs/v2.html

Задачи состоят из:
- имени пользователя;
- е-mail;
- текста задачи;
- статус задачи;

Стартовая страница - список задач с возможностью сортировки по имени пользователя, email и статусу. Вывод задач нужно сделать страницами по 3 штуки (с пагинацией). Видеть список задач и создавать новые может любой посетитель без регистрации.

Сделайте вход для администратора (логин "admin", пароль "123"). Администратор имеет возможность редактировать текст задачи и поставить галочку о выполнении. Выполненные задачи в общем списке выводятся с соответствующей отметкой.

В приложении нужно использовать React и Redux. Сложная архитектура не нужна, решите поставленные задачи минимально необходимым количеством кода. К дизайну особых требований нет.
Результат нужно развернуть на любом бесплатном хостинге (например - zzz.com.ua), чтобы можно было посмотреть его в действии. Код можно выложить на github или bitbucket.

Будем ждать от Вас сообщение с результатом работы. Укажите, пожалуйста, в своём письме общее количество потраченного времени.

По окончанию выполнения ждем от Вас две ссылки: на репозиторий, где выложен код и на рабочее тестовое задание.

Если Вы не смогли выполнить тестовое по любым причинам, пожалуйста, сообщите нам. Будем ждать Вашего ответа в любом случае.

Для Вашего удобства предоставляю протокол тестирования, по которому проверяется тестовое задание.
1) Перейти на стартовую страницу приложения. Должен отобразиться список задач. В списке присутствуют поля: имя пользователя, email, текст задачи, статус. Не должно быть опечаток. Зазоры должны быть ровные. Ничего не ползет. Должна быть возможность создания новой задачи. Должна быть кнопка для авторизации.
2) Не заполнять поля для новой задачи. Сохранить задачу. Должны вывестись ошибки валидации. Ввести в поле email “test”. Должна вывестись ошибка, что email не валиден.
3) Создать задачку с корректными данными (имя “test”, email “test@test.com”, текст “test job”). Задача должна отобразиться в списке задач. Данные должны быть ровно те, что были введены в поле формы. После создания задачи должно вывестись оповещение об успехе добавления (обратная связь).
4) Создать задачу с тегами в описании задачи (добавить в поле описания задачи текст , заполнить остальные поля). Задача должна отобразиться в списке задач, при этом не должен всплыть alert c текстом ‘test’.
5) Создать еще 2 задачи. Должна появиться новая страница в пагинации.
6) Отсортировать список по полю “имя пользователя” по возрастанию. Список должен пересортироваться. Перейти на последнюю страницу в пагинации. Сортировка не должна сбиться, задачи с последней страницы должны быть отображены. Далее отсортировать по тому же полю, но по убыванию. Перейти на первую страницу. Имя пользователя, которое было последним в списке, должно стать первым. Проделать этот тест для полей “email” и “статус”.
7) Перейти на страницу авторизации пользователя. Попробовать залогиниться с пустыми полями. Должна вывестись ошибка, что поля обязательны для заполнения или, что введенные данные не верные. Ввести в поле для имени пользователя “admin1”, в поле для пароля “321”. Должна вывестись ошибка о неправильных реквизитах доступа. Админский доступ не должен быть предоставлен. Ввести данные “admin” в поле для имени и “123” в поле для пароля. Авторизация должна пройти успешно. Должна отобразиться кнопка для выхода из профиля админа.
8) Для созданной задачи проставить отметку “выполнено”. Перезагрузить страницу. В общем списке задача должна отображаться с двумя отметками: статус задачи “выполнено” и “отредактировано администратором”. Отредактировать текст задачи. Сохранить и перезагрузить страницу. Текст задачи должен быть тот, который ввели при редактировании.
9) Открыть параллельно приложение в новой вкладке. Разлогиниться в новой вкладке. В этой вкладке не должно быть возможности редактировать задачу. Вернуться в предыдущую вкладку. Отредактировать задачу и сохранить. Отредактированная задача не должна быть сохранена. Приложение должно запросить авторизацию.
</details>

<details>
<summary>Тестовое 2</summary>
Предпоготовка:

Внешний вид приложения и прочие моменты:

    верхнее / боковое меню с навигацией
    Логин ( /login)
    Новости (список новостей, роут /news)
    Профиль (страница с информацией о пользователе, /profile)
    Кнопка «войти/выйти»

Страница /profile недоступна для тех, кто не залогинился.
Б Бэкэнд

Приложение использует простой «бэк» расположенный на heroku. Свой бэкэнд делать не нужно.

Для проверки доступности бэкэнда, можете перейти по адресу:

https://mysterious-reef-29460.herokuapp.com/api/v1/

Удачный логин + редирект

Форма для входа включает в себя 2 поля: email + пароль.
По нажатию на «логин» (или после нажатия клавиши Enter) уходит POST запрос с введенными данными на бэкэнд.

Адрес и метод для запроса:

POST https://mysterious-reef-29460.herokuapp.com/api/v1/validate

Если введены корректные данные: (email = 'max@test.com', password = '12345', content-type: application/json), ответ будет:
```js
{
  "status": "ok",
  "data": {
    "id": 1
  }
}
```

В случае успеха — пользователя нужно редиректить на страницу профиля, на которой будет нужно получить подробную информацию о пользователе. Об этом ниже в разделе Профиль. Для выполнения этой задачи, рекомендую полученный id сохранять в стор (в какой-то из редьюсеров).

Обратите внимание на название полей (username, password), на их значения (строковые) и на то, что это POST запрос.

Если введены некорректные данные, то нужно уметь обрабатывать ответ с ошибкой:
```js
{
  "status": "err",
  "message": "wrong_email_or_password"
}
```

После получения такого ответа, необходимо очистить из формы поле пароля (email не трогать) и показать красивое сообщение об ошибке: Имя пользователя или пароль введены не верно.

Дополнительно:

    организовать код таким образом, чтобы можно было легко показывать сообщения на различные сообщения об ошибке от сервера.

    сделать обработку возможной сетевой ошибки с текстом: Сервер не доступен

Запрос должен быть выполнен через традиционный redux-подход: то есть мы «диспатчим (вызываем) экшены и сохраняем необходимое в редьюсере».
П Профиль

На странице профиля необходимо сделать GET запрос, и получить подробную информацию о пользователе:

GET https://mysterious-reef-29460.herokuapp.com/api/v1/user-info/:id

В реальном приложении, после user-info мог бы быть любой id, в нашем случае — это id 1, значит запрос должен выглядеть так:

https://mysterious-reef-29460.herokuapp.com/api/v1/user-info/1

Ответ:
```js
{
  "status": "ok",
  "data": {
    "userId": 1,
    "city": "Москва",
    "languages": [
      "English",
      "Русский"
    ],
    "social": [
      {
        "label": "vk",
        "link": "vk.com/maxpfrontend"
      },
      {
        "label": "telegram",
        "link": "t.me/maxpfrontend"
      },
      {
        "label": "web",
        "link": "https://maxpfrontend.ru"
      },
      {
        "label": "youtube",
        "link": "https://www.youtube.com/channel/UCqJyAVWwIqPWKEkfCSP1y4Q"
      },
      {
        "label": "twitter",
        "link": "https://twitter.com/MaxPatsiansky"
      },
      {
        "label": "twitch",
        "link": "http://twich.tv/maxpfrontend"
      }
    ]
  }
}
```

Полученные данные, положить в стор, и отрисовать на странице следующим образом:
```
Город: Москва

Знание языков:
 + English
 + Русский

Ссылки:

+ ссылка-иконка 1
+ ссылка-иконка 2
...
```

(
  т.е. кликабельная иконка каждого из сервисов.
  Ссылка открывается в новом окне
)

Иконки возьмите из google картинок, положите к себе в public директорию. Для «сайта» подойдет иконка глобуса или сито «Без воды» 🙂

Ахтунг!

В требовании к задаче, «дизайнер» захотел, чтобы сайт (web) был первым в списке, а бэкэнд-разработчик ответил, что ему «пофиг и некогда». Поэтому, сайт нужно отрисовать первым своими силами (то есть, как-то обработать входящие данные с MockAPI). Все остальное в любом порядке.

Дополнительно:

    обработать ситуацию, когда пользователь не найден.

Запрос:

GET https://mysterious-reef-29460.herokuapp.com/api/v1/user-info/2

Ответ
```js
{
  "status": "err",
  "message": "user_not_found"
}
```
Н Новости

На странице, нужно вывести новости в формате «заголовок» + «текст».
Внизу страницы — «всего новостей ХХ» (зависит от количества новостей, в нашем случае это всегда «2», но вы должны сделать это число не «захардкоженным»)

Если говорить, словами «разработчиков», то API endpoint:

GET https://mysterious-reef-29460.herokuapp.com/api/v1/news 

Если словами «новичков» — нужно сделать GET запрос, по адресу выше.

Ответ:
```js

{
  "status": "ok",
  "data": [
    {
      "id": 1,
      "title": "Не слишком ли быстро мы переходим на беспилотные автомобили",
      "text": "Автопроизводители и высокотехнологичные компании, тратящие миллиарды долларов на развитие беспилотных автомобилей и грузовиков, вовсю рекламируют автоматический транспорт, который, по их мнению, будет безопаснее, чище и сделает общество более мобильным."
    },
    {
      "id": 2,
      "title": "Интеллектуальная собственность: где заканчивается цитирование и начинается плагиат",
      "text": "Компьютерная программа или роман — это в первую очередь идея, творческий замысел. Но человек, купивший книгу, хоть и стал собственником её обложки и страниц, не может присвоить себе то, что написал или нарисовал автор, и продавать романы под своим именем. Иными словами, интеллектуальная собственность — это придуманный и созданный человеком результат. И одновременно с этим — права на него."
    }
  ]
}
```

Новости должны храниться в соответствующем редьюсере.
В Войти/выйти

Кнопка просто меняет свое состояние. Если пользователи уже залогинился — «Выйти», если нет — «Войти»
Т Требования ✍️

    Внимание к деталям.
    Для асинхронных запросов использовать redux-thunk, можно ducks или любой другой подход. Использование «саг» для такой задачи не рекомендуется.
    Пока новости / профиль грузятся — показывать прелоадер (использовать редьюсеры и экшены, как того требует redux).
    Пока запрос на логине «в процессе» блокировать повторные запросы (самый легкий способ, это блокировать нажатия кнопки Enter + сделать disabled кнопку отправки формы). Разумеется, чтобы пользователю было понятнее, текст disabled кнопки можно сделать: «Проверяю…» либо прелоадер как на профиле/новостях.
    В форме показывать ошибку + стандартную валидацию email (по типу инпута, либо по регулярному выражению).
    Код разместить на github
</details>

<details>
<summary>Тестовое 3</summary>
Необходимо разработать React-приложение для отображения таблицы с данными.
Дополнительным плюсом будет: Финальный билд приложения должен быть запускаться из __Docker контейнера__ (хотябы с минимальной конфигурацией)

__Функционал__

- Сортировка по столбцам: при нажатии на название столбца строки таблицы сортируются по возрастанию, при повторном клике &mdash; по убыванию. Графическим элементом или текстовым сообщением указывается направление сортировки.
- Клиентская пагинация: данные необходимо отображать постранично, максимум 50 элементов на страницу. Необходимо предоставить пользовательскую навигацию для перехода по страницам.
- Фильтрация: компонент предоставляет текстовое поле, в которое пользователь может ввести текст и строки таблицы, данные которых не содержат подстроку, введённую пользователем, скрываются. Перефильтрация осуществляется по нажатию на кнопку "Найти".
- По клике на строку таблицы значения полей выводятся в дополнительном блоке под таблицей.
- Данные в таблицу загружаются с сервера. Способ загрузки с сервера на ваш выбор.
- Над таблицей присутсвует кнопка __добавить__, по нажатии на которую выпадает форма добавления ряда
	+------+------------+-----------------+-----------------+---------------+
	| id   | firstName  | lastName        | email           | phone         |
	+------+------------+-----------------+-----------------+---------------+
	|input | input      | input           | input           | input         |
	+------+------------+-----------------+-----------------+---------------+
- После заполнения всех инпутов активируется кнопка __Добавить в таблицу__ которая вставляет заполненный ряд в начало таблицы
  

Для демонстрации работы компонента необходимо сделать простую HTML страницу.
Пользователю предлагается выбрать набор данных: маленький или большой.
При выборе набора данных он загружается с сервера и по данным строится таблица.

__Формат данных от сервера__

Сервер возвращает JSON-массив данных.
Пример данных: 
```js
[
	{
		id: 101,
		firstName: 'Sue',
		lastName: 'Corson',
		email: 'DWhalley@in.gov',
		phone: '(612)211-6296',
		address: {
			streetAddress: '9792 Mattis Ct',
			city: 'Waukesha',
			state: 'WI',
			zip: '22178'
		},
		description: 'et lacus magna dolor...',
	}
}
```

Маленький объем данных берется по ссылке
http://www.filltext.com/?rows=32&id={number|1000}&firstName={firstName}&lastName={lastName}&email={email}&phone={phone|(xxx)xxx-xx-xx}&address={addressObject}&description={lorem|32}

Большой объем данных берется по ссылке
http://www.filltext.com/?rows=1000&id={number|1000}&firstName={firstName}&delay=3&lastName={lastName}&email={email}&phone={phone|(xxx)xxx-xx-xx}&address={addressObject}&description={lorem|32}

__Замечания__

- Особое внимание следует уделить скорости работы. Зависание интерфейса при выполнении операций загрузки данных, фильтрации, сортировки недопустимо.
- Во время загрузки данных стоит показать какой-то индикатор
- Использование сторонних библиотек будет плюсом только в случае если это оправданно и вы сможете объяснить причину выбора. Показав свои знания в грамотном применении сторонних готовых решений, вы имеете шанс повысить свою профессиональную привлекательность для нас.
- Пишите код так, как бы вы его писали в работе &mdash; внутренности задания будут оцениваться даже тщательней, чем внешнее соответствие заданию. Код должен быть организован так, чтобы его можно было заново использовать.
- Помните про обработку ошибок!
- Верстка может быть самая простая. Визуализацию и украшение делайте на ваш вкус. Мы не против использования [Bootstrap](http://getbootstrap.com/) или похожего UI фреймворк, но только для UI представления (нельзя использовать JS код для решения задачи, но можно использовать для оформительских эффектов (анимации и тому подобное))!

__Схема визуального представления данных__

```
+------+------------+-----------------+-----------------+---------------+
| id ▲ | firstName ▼| lastName      ▼ | email          ▼| phone        ▼|
+------+------------+-----------------+-----------------+---------------+
| 101  | Sue        | Corson          | DWhalley@in.gov | (612)211-6296 |
+------+------------+-----------------+-----------------+---------------+
| 102  | Lor        | Ipsumd          | dwhalley@in.gov | (612)211-6296 |
+------+------------+-----------------+-----------------+---------------+
| 103  | Ips        | Umdolo          | dwhalley@in.gov | (612)211-6296 |
+------+------------+-----------------+-----------------+---------------+
```

Если выделен пользователем с `id = 101`, то под таблицей выводим следующую информацию:

	Выбран пользователь <b>Sue Corson</b>
	Описание:
	<textarea>
	et lacus magna dolor...
	</textarea>
	Адрес проживания: <b>9792 Mattis Ct</b>
	Город: <b>Waukesha</b>
	Провинция/штат: <b>WI</b>
	Индекс: <b>22178</b>

Дополнительно напишите нам, как вы тестировали результат своей работы. Какие используете инструменты и как вы осуществляете тестирование.

</details>

<details>
<summary>Работа с формами</summary>
	
__Схема визуального представления данных__
	Подача осуществляется в 4 шага.
```
1. Выбор категории сообщения:
 1.1.Отправляется запрос на БЭК за категорями, по получению ответа - выводятся на экран. Все пункты кликабельны(плитки)
 1.2.Выше категорий должна находиться строка поиска категорий с выпадающим списком и возможностью выбрать категорию в ней
 1.3.Из категорий извлекаются подкатегории и выводятся на экран. Выбранная ГЛАВНАЯ категория должна выводиться на экране с возможностью очистить или перевыбрать
 1.4.Также выбираем подкатегорию и переходим на следующий шаг
```
```
2.Текст сообщения, прикрепление файлов
 2.1. Выводятся 3 поля: Выбранные категории(с возможностью их изменить) и поле ввода текста сообщения
 2.2. Под вводом текста сообщения должна быть кастомная кнопка для прикрепления фотографий к форме
 2.3. После загрузки фото должен работать предпросмотр(показываются прикреплённые фото в уменьшённом формате)
 2.4. Должна быть возможность удаления файлов.
```
```
3. Ввод места жительства, координат:
 3.1. Выводятся следующие поля: Выбор района жительства, города,улицы,дома. 
 3.2 Под полем с выбором района должна быть надпись "Я не знаю места", по нажатию на которую будет открываться карта
 3.3 На карте должна быть возможность указать адрес, после выбора - внести выбранный адрес в поля формы.
 3.4. Также необходимо получить координаты
```
```
4. Предпросмотр всего сообщения?
 4.1  Выводятся текстовые поля,с данными, которые мы вводили. Поля read-only. 
 4.2. Если пользователь выбирал адрес через карту - должна выводиться карта с меткой по указанному адресу
 4.3. Также должны отображаться прикреплённые файлы
```
__Замечания__
- Если выходить из формы на другую страницу, то внесённые данные не должны пропадать
- Срок на выполнение: 1 месяц
- Грамотная архитектура приложения
- Соблюдение всех принципов BOLD,DRY,KISS


</details>
