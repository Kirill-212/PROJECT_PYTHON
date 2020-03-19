###### Идея проекта заключается  в парсинге данных с сайта(сайта с валютой) и с добавлением функционала + добавление того чего нет на других подобных сайтах.
# Реализация:
+ Статические файлы ,которые используются в проекте.
  * [CSS](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/static/css/first.css)
  * [JS](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/static/js/first.js)
  * [IMAGE](https://github.com/Kirill-212/PROJECT_PYTHON/tree/master/PROGECT/static/image)
+ Настройки проекта в которые я подключил проект и настроил пути статических файлов.
  * [SETTINGS](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/PROGECT/settings.py)
+ URL адрес главного проекта и созданного приложения.
  * [URL Project](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/PROGECT/urls.py) -адресация из главного проекта.
  * [URL Main](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/urls.py) -адресация в приложение Main.
+ Созданные модели.
  * [currency](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/models.py#L9) -модель в которой хранятся данных и с которой сравниваю данные при парсинге.
  * [annual_statistics](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/models.py#L16) -модель с валютой за год(которую я заполнил вручную).
  * [Message](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/models.py#L22) -модель которая хранит сообщения с форума.
  * [statistics](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/models.py#L34) -абстрактная модель которая хранит поле количестово зарег. пользователей.
  *[statistics_users](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/models.py#L42) -модель которая наследует абстрактную модель и у её есть поле с именами зарег. пользователями.
+ Админка
  * [admin](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/admin.py) -добавлены модели ,которые админ может редактироать.
+ Контроллеры.
  * [get html](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/views.py#L31) -Отпраление запроса серверу
  * [parse](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/views.py#L53) -вызов функции get_html и получение кода ответа от сервера.
  * [get_content](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/views.py#L37) -получение нужного контента с сайта.
  * [index](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/views.py#L63) -рендер гл. страницы и проверка зарег. пользователей +проверка данных полученных с сайта с данными из бд +вывод сообщений в форум.
  * [RegisterFormView](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/views.py#L106) -заполнение стандартной формы для регистрации в django.
  * [LoginFormView](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/views.py#L106) -заполнение стандартной формы для аутентификации пользователя в django.
  * [LogoutView](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/views.py#L129) -выход из учётной записи.
  * [PasswordChangeView](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/views.py#L136) -стандартная форма для смены пароля в django.
  * [post](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/views.py#L153) -контроллер для отправки сообщений в бд.
  * [HomeView](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/views.py#L163) -контроллер для отправки рендера страницы charts.html.
  * [ChartDate](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/views.py#L170) -контроллер для отрисовки графиков.
+ html файлы
  * [main](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/templates/main.html) -файл с главным контентом страницы.
  * [base_main](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/templates/base_main.html) -файл с контентом таблицы ,которая отрисовавываются в main.html.
  * [charts](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/templates/charts.html) -файл с графиками, в котором через ajax получают запрос на получение данных из ChartDate.
  * [login](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/templates/reg/login.html) -файл с формой для аутентификации пользователя.
  * [register](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/templates/reg/register.html) - файл с формой для регистрации пользователя.
  * [password_change_form](https://github.com/Kirill-212/PROJECT_PYTHON/blob/master/PROGECT/Main/templates/reg/password_change_form.html) -файл с формой для смены пароля.
 
 
 
 
 
 
  
