Формат:

1) Краткое описание

2) Подробное описание (спойлер)

3) Кто автор

4) Как позвать этого бота себе (просто)

5) Как установить этого бота себе (сложно)


## Пан Бан
[@pan_ban_by](https://t.me/pan_ban_by)


### Описание
Автоматически удаляет троллей и лукоботов из чата сверясь по своему списку.

<details>
  <summary>Подробности</summary>
  
Пан Бан ведет базу троллей, и основываясь на ней делает две вещи:

1) При добавлении в чат смотрит есть ли среди участников тролли из базы. Если таковые находятся - Пан Бан удаляет их из чата

2) Если в чат заходит тролль из базы - он автоматически удаляется из чата в течение нескольких минут.

Обратите внимание, что Пан Бан - это не телеграм бот, а аккаунт.
Бот не может получить список участников чата, и, соответственно, не сможет выполнять описанные функции.

Как узнать результаты работы бота?
На текущий момент бот никак не оповещает о результатах своей работы. Но в скором времени у бота появится такая возможность и он будет отправлять в чат сообщение при каждом удалении из чата(либо агрегированно).

Что если бот удалит нормального участника?
Такие ошибки могут произойти. В этом случае нужно написать @dzechat_bot о ситуации. В @dzechat_bot можно писать в том числе если возникли какие-то вопросы/предложения.

Спасибо присоединившейся команде разработчиков бота к команде dze.chat!
</details>


### Автор
Антон Мотолько - белорусский активист, блогер, фотограф.
[Подробнее](https://cyclowiki.org/wiki/%D0%90%D0%BD%D1%82%D0%BE%D0%BD_%D0%93%D0%B0%D0%B4%D0%B8%D0%BC%D0%BE%D0%B2%D0%B8%D1%87_%D0%9C%D0%BE%D1%82%D0%BE%D0%BB%D1%8C%D0%BA%D0%BE)


### Установка
Для этого достаточно добавить [@pan_ban_by](https://t.me/pan_ban_by) в ваш чат и дать ему права администратора с разрешением удалять участников, а так же удалять сообщения(появилась функция удаления спам сообщений).
ВАЖНО: добавляйте Пан Бан только в чате где больше 100 участников.


### Собственная копия
К сожалению автор бота не поделился кодом этого бота, чтобы не раскрывать алгоритм вычисления троллей в чате, так что ставьте его только в том случае если всецело доверяете автору 


## DaySandBox

[@daysandbox_bot](https://t.me/daysandbox_bot)


### Описание
Простой, но эффективный бот для защиты от спама. 

<details>
  <summary>Подробности</summary>
Идея состоит в том, чтобы удалить ссылки, медиафайлы и перенаправленные сообщения, написанные пользователями, присоединившимися к чату менее 24 часов назад. Этот метод позволяет удалить большую часть спам-сообщений от новых пользователей. Обратной стороной этого подхода является то, что любой участник чата старше 1 дня может публиковать что угодно. Это компромисс между простотой и эффективностью. Вы получаете бесплатно инструмент, который автоматически удаляет много спам-сообщений, но не все. Вы можете установить список доменов и групп/каналов, которые никогда не должны блокироваться. Вы можете добавить нового участника чата в белый список, если хотите разрешить ему публиковать ссылки до истечения безопасного периода. По умолчанию удаление мультимедийных сообщений отключено. Прочтите «Команды», чтобы узнать, как включить удаление мультимедийных сообщений от новых пользователей. Также вы можете отключить новых пользователей на несколько часов с помощью опции mute_hours.

Тип сообщений, которые Daysandbox Bot считает возможным спамом:

* сообщение переадресовано из другого чата
* сообщение содержит ссылку на какой-либо веб-документ
* сообщение содержит упоминание @username, указывающее на группу или канал. Если @username указывает на какого-то пользователя, то это не считается ссылкой.
* сообщение содержит кнопку любого типа. Обычно такие сообщения отправляются через встроенных ботов.
* мультимедийные сообщения, отключены по умолчанию. Медиа - это аудио, игра, анимация, документ, фото, видео, голос, видеозаметка, контакт, местоположение.
</details>


### Автор
[Lorien](https://github.com/lorien)

[Сайт автора с описанием и инструкциями](https://tgdev.io)


### Установка
Следуйте этим шагам:

* Добавьте [@daysandbox_bot](https://t.me/daysandbox_bot) в качестве администратора в свой чат.
* Дайте боту разрешение на удаление сообщений. Никаких других разрешений не требуется.
* Необязательный шаг: настроить белый список доменов и групп/каналов.
* Необязательный шаг: разрешите удаление мультимедийных сообщений от новых пользователей.

<details>
  <summary>Команды</summary>
  
`/daysandbox set notify_actions=yes` - настроить бота писать сообщения в чат о каждом удаленном спам-сообщении

`/daysandbox set notify_actions=no` - настроить автоматическое удаление спам-сообщений

`/daysandbox set remove_media=yes` - настроить бота на удаление медиа-сообщений от новых пользователей (по умолчанию НЕТ)

`/daysandbox set remove_media=no` - настроить бота, чтобы он НЕ удалял мультимедийные сообщения от новых пользователей

`/daysandbox set safe_hours=X` - установить безопасный период на X часов. Значение X должно быть числом в диапазоне 0 <X <720. Другими словами, безопасный период должен быть больше нуля и меньше или равен одному месяцу.

`/daysandbox set mute_hours=X` - полностью отключить звук для новых пользователей на указанное количество часов. По умолчанию это ноль часов, т.е. для новых пользователей звук не отключен. Допустимое значение для этой опции находится в диапазоне от 0 до 720.

`/daysandbox config` - отобразить конфигурацию бота для текущего чата

`/daysandbox check` - проверить, правильно ли установлен бот

`/daysandbox reload_admins` - попросить бота перезагрузить админки для текущего чата. Список администраторов собирается один раз и кешируется. Используйте эту команду для обновления кэшированных данных.

`/daysandbox wl_add FOO` - запретить боту блокировать ссылки, содержащие FOO. FOO может быть доменом или именем пользователя группы/канала. Используйте "@" чат, чтобы указать имена пользователей групп / каналов. Пример: `/daysandbox wl_add google.com` или `/daysandbox wl_add @tgdev_en`.

`/daysandbox wl_del FOO` - удалить FOO из списка доменов/групп/каналов, которые никогда не должны блокироваться. Пример: `/daysandbox wl_del yahoo.com`

`/daysandbox userwl_add USER` - запретить боту блокировать сообщения от пользователя. Имя пользователя USER должно начинаться с символа "@". Пример: 

`/daysandbox userwl_add @foobar`

`/daysandbox userwl_del USER` - удалить пользователя USER из белого списка. Пример: `/daysandbox userwl_del @foobar`

`/daysandbox set lang=<lang-code>` - настроить язык уведомлений. Допустимые значения для этих настроек: `en` и `ru`.
</details>

Оригинальная инструкция на английском: [https://tgdev.io/bot/daysandbox_bot](https://tgdev.io/bot/daysandbox_bot)


### Собственная копия
Репозиторий находится по адресу [https://github.com/lorien/daysandbox_bot](https://github.com/lorien/daysandbox_bot) - написан бот на языке программирования Python. Как таковой инструкции по запуску нет, но возможно появится в будущем. Программы на Python запускать достаточно просто(чуть позже возможно сделаем pull request с автоматизацией и запуском в [Docker](https://ru.wikipedia.org/wiki/Docker)).


## Join Hider Bot
[@joinhider_bot](https://t.me/joinhider_bot)


### Описание
Бот для удаления сообщений о том, что пользователь присоединился или покинул чат.

<details>
  <summary>Подробности</summary>
 
По умолчанию он удаляет как сообщении о присоединившемся пользователе, так и сообщение о покинувшем чат пользователе. Вы можете настроить его для каждого конкретного чата. Например, вы можете настроить бота так, чтобы он удалял сообщения, присоединившегося к чату пользователя, но оставлял сообщения, о покинувшем  чат пользователе.

</details>


### Автор
[Lorien](https://github.com/lorien)

[Сайт автора с описанием и инструкциями](https://tgdev.io)


### Установка
Следуйте этим шагам:

* Добавьте [@joinhider_bot](https://t.me/joinhider_bot) в качестве администратора в свой чат
* Дайте боту разрешение на удаление сообщений. Никаких других разрешений не требуется

<details>
  <summary>Команды</summary>

`/joinhider check` - проверить, правильно ли установлен бот.

`/joinhider config` - отобразить конфиг бота для текущего чата

`/joinhider set delete_user_joined_msg MODE` - включить или отключить удаление сообщений о подключении пользователя к чату. MODE должен быть да или нет. Пример команды: `/ joinhider set delete_user_joined_msg yes`

`/joinhider set delete_user_left_msg MODE` - включить или отключить удаление сообщений о выходе пользователя из чата. MODE должно быть yes или no. Пример команды: `/joinhider set delete_user_left_msg yes`
</details>

Оригинальная инструкция на английском: [https://tgdev.io/bot/joinhider_bot](https://tgdev.io/bot/joinhider_bot)


### Собственная копия
Репозиторий находится по адресу [https://github.com/lorien/joinhider_bot](https://github.com/lorien/joinhider_bot) - написан бот на языке программирования Python. Как таковой инструкции по запуску нет, но возможно появится в будущем. Программы на Python запускать достаточно просто(чуть позже возможно сделаем pull request с автоматизацией и запуском в [Docker](https://ru.wikipedia.org/wiki/Docker)).


## CaptchaBot
[@captcha97_bot](https://t.me/captcha97_bot)


### Описание
Телеграм бот для противодействия ботам, выдаёт присоединившимся к чату пользователям каптчу на основе эмоджи. Обладает удобным и юморным интерфейсом для пользователя.

Может быть полезен в противодействии автоматизированному(без участвия человека) наполнению чата новыми пользователями.


### Автор
Некий анонимный [разработчик](https://github.com/F0rzend) из Беларуси.


### Установка
Следуйте этим шагам:

* Добавьте [@captcha97_bot](https://t.me/captcha97_bot) в качестве администратора в свой чат
* Дайте боту разрешения на изменение профиля группы, удаление сообщений, блокировку участников. Больше никаких настроек не требуется.


### Собственная копия
Код доступен [здесь](https://github.com/F0rzend/antirobot_aiogram), там же есть неплохая инструкция по запуску.


## Telegram Report Bot
[https://github.com/MasterGroosha/telegram-report-bot](https://github.com/MasterGroosha/telegram-report-bot)


### Описание
Очень эффективный бот-модератор - фактически добавляет функцию пользовательской модерации - любой пользователь может привлечь внимание администрации в чате с помощью команды `/report` в ответ на сообщение нарушающее правила(после этого в отдельный чат для администрации придёт 2 сообщения: пересланное сообщение нарушаующее правила, и собщение с кнопками "замьютит на 2 часа"/"удалить сообщение"/"удалит все сообщения пользователя и забанить его" для принятия решений), так же можно просто позвать администрацию написав в чате @admin (особенно актуально после появления анонимности для админов чата).


### Автор
[Профиль разработчика на github](https://github.com/MasterGroosha).


### Установка
К сожалению на данный момент нет возможности просто подключить бот, установка бота возможна только методом запуска приложения.


### Собственная копия
Репозиторий находится по адресу [https://github.com/MasterGroosha/telegram-report-bot](https://github.com/MasterGroosha/telegram-report-bot), там же есть и инструкция по запуску(правда на английском), имеется возможность запуска в [Docker](https://ru.wikipedia.org/wiki/Docker)(что несомненно большой плюс, так как значительно облегчает процесс запуска).
