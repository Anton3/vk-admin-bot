## Боты

Бот-админ выполняет все команды. Можно писать команды ему команды в личку. В беседе нужно дать "доступ ко всей переписке". Выбирайте одного любого:
1. [Бот Борис](https://vk.com/borya_bot)
2. [Бот Тор](https://vk.com/tor_bot) (англ. Thor)
3. [Ким](https://vk.com/kimcm)

Бот-помощник является инструментом бота-админа в управлении беседой. Нужно дать ему администратора беседы. Выбирайте одного любого:
1. [Ян Молотов](https://vk.com/banhammer_bot)
2. [Марина](https://vk.com/id541872196)

## Требуемые права

- 👑 `admin` — все команды; не путать с администраторами бесед ВК
- 🔑 `supermoderator` — все команды, кроме самых опасных
- 🔨 `moderator` — может исключать участников и управлять ими
- 🧑 Участник беседы — нет особых прав
- 🤖 Команду можно писать в личку боту

## Используемые обозначения

- Все команды начинаются или с `/`, или с `.`
- `/команда <аргумент>` Здесь внутри `<>` приводится название/описание аргумента. На месте `<аргумент>` надо написать то, что требует данная команда
- Сами угловые скобки `<>` писать не надо. Только то, что внутри
- `👤` — ссылка на профиль пользователя, с которым надо выполнить какое-то действие, например, [vk.com/id1](vk.com/id1). Также можно использовать упоминание, или вместе с командой переслать его сообщение.
- `👥` — Можно указать нескольких пользователей сразу
- `🕒` — Целое число и одна из букв `смчд`. Примеры: `30м`, `3ч`
- `<игра>` — или `кр` (то есть Clash Royale), или `бс` (то есть Brawl Stars)
- `#тег` — тег игрока или клана в игре

## Общие команды

- 🤖 `/start` Получить ссылки на основные команды и страницы
- 🧑🤖 `/help` Получить ссылку на эту страницу
- 🧑🤖 `/ping` Проверить, работает ли бот
- 🧑 `/write` Бот напишет, что захотите. В начале сообщения бот добавит значок ✍, в котором содержится ссылка на вас

## Приглашение и исключение из беседы

- 🔨 `/kick 👥` Кикнуть из беседы. Кик бессрочный. Кикнутого можно пригласить обратно
- 🔨 `/invite 👥` Пригласить в беседу
- 🔨 `/ban 🕒 👥` Забанить на определённый срок. Во время бана пользователя нельзя пригласить в беседу. Если он добавил в друзья бота-помощника, то этот бот его вернёт. При повторном применении `/ban` к уже забаненному пользователю, он перебанивается, начиная с текущего момента
- 🔨 `/ban perm 👥` Забанить навсегда. Такой пользователь не будет автоматически разбанен
- 🔨 `/unban 👥` Разбанить и пригласить в беседу
- 🔨 `/mute 🕒 👥` Заглушить на определённый срок. Пользователь сможет читать, но не писать в беседе
- 🔨 `/mute perm 👥` Бессрочное заглушение
- 🔨 `/unmute 👥` Отменить заглушение
- 🧑 `/banlist` Посмотреть список пользователей в бане и муте

## Роли

Управление ролями:

- 🧑 `/roles` Показать список ролей беседы
- 🧑 `/allroles` Список всех обладателей каждой из ролей
- 🔑 `/addrole <название роли>` Создать новую роль
- 🔑 `/remrole <название роли>` Удалить роль
- 🔑 `/rename <старое название роли> <новое название роли>` Поменять название роли
- 🔑 `/move <роль> <номер>` Передвинуть роль в списке ролей на позицию с указанным номером

Выдача ролей:

- 🧑 `/whois 👤` Показать роли участника
- 🧑 `/role <роль>` Показать список участников с указанной ролью
- 🧑 `/mention <роль>` Призвать в беседу участников с указанной ролью
- 🔨 `/give <роль> 👥` Выдать указанную роль пользователям
- 🔨 `/take <роль> 👥` Забрать указанную роль у пользователей

Особые роли: `admin`, `supermoderator`, `moderator`, `normal`. Особым ролям также можно давать "человеческие" названия.

Особые роли не отображаются в общем списке ролей, вместо этого их можно найти в списке `/staff`. Для выдачи особых ролей также есть сокращённые команды.

- 🧑 `/staff` Посмотреть руководящие роли и их обладателей
- 👑 `/admin 👥` = `/give admin`
- 👑 `/supermoderator 👥` = `/give supermoderator`
- 🔑 `/moderator 👥` = `/give moderator`
- 🔨 `/normal 👥` = `/give normal`

При переименовании особых ролей, соответствующие команды также переименовываются.

Чтобы иметь право кикнуть участника беседы или управлять его ролями, привязками к аккаунтам или описанием, вы должны иметь административную роль выше него. Исключение: `admin` может кикать и управлять другими `admin`.

## Настройка названия, фото, закрепа

- 👑 `/title <новое имя>` Изменить название беседы. Если не-`админ` изменит название беседы не через бота, то бот вернёт его обратно
- 👑 `/title` Разрешить изменять название беседы вручную
- 🔨 `/pin <переслать сообщение>` Закрепить сообщение
- 🔨 `/pin` Открепить текущий закреп

## Удаление сообщений

- 🔑 `/delete <переслать сообщения>` Удалить пересланные сообщения
- 🔑 `/purge 🕒` Удалить сообщения за указанный интервал времени
- 🔑 `/purge 🕒 👥` Удалить сообщения указанных пользователей за указанный интервал времени
- 🔑 `/noswear` Переключить удаление сообщений с руганью. Слова, считающиеся ругательствами, можно посмотреть [здесь](swear_words.txt)
- 🔑 `/novoice` Переключить удаление голосовых сообщений
- 🔑 `/nograffiti` Переключить удаление граффити
- 🔑 `/nocoffi` Переключить удаление шифровок от Coffi

## Борьба со спамом командами

- 🧑 `/pm <команда>` Модификатор команды, который заставляет бота ответить личным сообщением. Пример: `/pm staff`
- 🧑 `/here <команда>` Модификатор команды, который заставляет бота ответить в беседе и не удалять ответ. Пример: `/here staff`
- 🔑 `/cleanup 🕒` Автоматически удалять некритичные команды через определённое время. Рекомендуется от `2m` до `30m`, в зависимости от активности беседы
- 🔑 `/cleanup` Выключить автоудаление
- 🔑 `/allpm` Переключить ответы на команды в ЛС. Ответы на не-административные команды будут посылаться в личку тому, кто написал команду
- 🧑 `/log` Посмотреть последние модерские команды, выполненные в беседе

## Настройка беседы

- 🧑 `/settings` Показать текущие значения настроек беседы

Настройки, которые не вошли в другие категории команд:

- 🔑 `/autokick` Кикать участников, покидающих беседу, чтобы они не могли вернуться, когда их не ждут
- 🔑 `/fixinvite` Добавлять людей в беседу можно только через бота. Добавленных вручную будет кикать
- 🔑 `/slowmode <число>` Указать ограничение на число сообщений в минуту для не-модеров
- 🔑 `/slowmode` Снять ограничение
- 🔑 `/maxstreak <число>` Указать ограничение на число сообщений подряд для не-модеров
- 🔑 `/maxstreak` Снять ограничение
- 🔑 `/allmute` В беседе могут писать только модераторы, остальные сообщения удаляются
- 🔑 `/antiraid` Бот будет кикать за слишком частые сообщения или за подозрение на спам от новичков
- 👑 `/reset` Удалить всю информацию о беседе и деактивировать ботов

## Приват

Приват — это мягкая форма мута, когда все сообщения от участника удаляются через заданный срок.

- 🧑 `/softmute` Список участников в привате
- 🔨 `/softmute 🕒 👥` Отправить участников в приват, сообщения от них будут удаляться спустя указанный срок
- 🔨 `/softmute 👥` Снять приват с участников

## Описания

Описание пользователя, если оно у него имеется, выводится в `/whois`.

- 🔑 `/describe 👤 <текст>` Задаёт описание
- 🔑 `/describe 👤` Удаляет описание

## Рейтинг

Рейтинг участника беседы на текущий момент состоит из количества отправленных сообщений и их среднего размера (в символах)

- 🧑 `/rating 👤` Рейтинг пользователя в беседе. По умолчанию, ваш
- 🧑 `/ratings` Список пользователей с самым большим рейтингом

## Макросы

Макросы — это пользовательские команды. Структура макросов [описана здесь](https://github.com/Anton3/vk-admin-bot/blob/master/macros.md).

- 🧑 `/macros` Список всех макросов
- 🧑 `/macro <название>` Показать определение макроса
- 🔑 `/addmacro <название> <определение>` Создать макрос
- 🔑 `/delmacro <название> <определение>` Удалить макрос

## Серверы

Беседы можно объединять в серверы. В составе серверов, беседам присваиваются короткие имена (также известны как каналы; не путать с заголовком беседы), которые используются в командах.

- 👑 `/newserver <имя-сервера>` Создать новый сервер на базе текущей беседы. Имя сервера может содержать только буквы, цифры, дефисы и подчёркивания (но не пробелы), и иметь длину от 1 до 30 символов. Также имя сервера не может совпадать с именами уже созданных серверов. Новый сервер после создания будет состоять из одной беседы с именем `main` — текущей беседы
- 👑 `/attach <имя-сервера> <имя-канала>` Присоединить беседу к существующему серверу, а также задать короткое имя беседы

После присоединения к серверу можно выполнять следующие команды:

- 🧑 `/channels` Показывает название сервера и всех бесед. Текущая беседа помечена `[*]`
- 👑 `/namechannel <новое-имя-канала>` Изменить короткое имя текущей беседы
- 👑 `/nameserver <новое-имя-сервера>` Изменить название сервера
- 👑 `/detach` Отсоединить беседу от сервера

Основные функции серверов:

- Сервер играет роль хранилища тегов, привязанных к пользователям. В разных серверах может быть разный набор тегов
- 🧑 `/to <имя-канала> <команда>` Выполнить команду в другой беседе сервера. Например, `/to main kick https://vk.com/id1` кикнет пользователя из беседы с коротким именем `main`, но не из текущей беседы

## Привязка акканутов CR и BS

Модераторы бесед могут привязать к любому пользователю ВК его аккаунты Clash Royale

- 🔨 `/bind <игра> #тег-игрока 👤` Привязать пользователю аккаунт CR или BS
- 🔨 `/unbind <игра> #тег-игрока 👤` Отвязать от пользователя аккаунт CR или BS
- 🔨 `/allunbind 👤` Отвязать от пользователя все аккаунты

После этого можно будет легко смотреть, кто он такой, через другие команды.

- 🧑🤖 `/whois 👤` Показать роли и краткое описание аккаунтов пользователя
- 🧑🤖 `/tag 👤` Показать теги аккаунтов указанного пользователя
- 🧑🤖 `/profile 👤` Показать подробную информацию по аккаунтам указанного пользователя
- 🧑🤖 `/profile <игра> #тег-игрока` Показать аккаунт без привязки
- 🧑🤖 `/trophies 👤` Показать количество трофеев на аккаунтах указанного пользователя
- 🧑🤖 `/chests 👤` Показать будущие сундуки на аккаунтах CR указанного пользователя

Эти команды можно применять к самому себе, если не указывать пользователя.

## Списки аккаунтов CR и BS

- 🧑 `/alltags` Список всех аккаунтов всех участников беседы
- 🧑 `/allclans` Список кланов, в которых состоят все участники беседы
- 🧑 `/alltrophies` Список рекорда по кубкам всех участников беседы

## Настройка беседы для CR и BS

- 🔑 `/nogames` Если включено, команды, связанные с CR, недоступны, и в `/whois` не отображаются профили CR
- 👑 `/setclan <игра> #тег-клана` Задать клан беседы. Командам из раздела "Управление кланами CR" необязательно будет указывать клан
- 👑 `/setclan` Убрать клан по умолчанию
- 🔑 `/clannews` Показывать предупреждение о полном клане и несоответствующем пороге для клана беседы

## Подтверждение аккаунтов CR и BS

Пользователь может самостоятельно привязать и подтвердить себе аккаунт. Рядом с подтверждёнными аккаунтами в `/whois` отображается значок ✅.

- 🤖 `/verify <игра> #тег-игрока` Подтвердить ваше владение аккаунтом. Бот потребует создать с этого аккаунта клан со специальным названием и описанием. В CR эта операция стоит 1000 золота, в BS бесплатно. Внимание: после выполнения всех указаний нужно повторить команду!
- 🤖 `/unverify <игра> #тег-игрока` Отменить подтверждение аккаунта

## Другие команды CR и BS

- 🧑🤖 `/findnick <часть ника>` Поиск пользователя ВК по привязанному к нему нику
- 🧑🤖 `/decks cr #тег-игрока` Ссылки на колоды CR, которые игрок использовал в последнее время, вместе с описанием, против каких колод эта дека хороша и плоха
- 🤖 `/war` Помощь в выборе колоды для КВ

## Управление кланами Clash Royale

- 🧑🤖 `/clan <игра> #тег-клана` Краткая сводка по клану
- 🔨🤖 `/claninfo <игра> #тег-клана` Текущие кубки и донат всех игроков клана
- 🔨🤖 `/clanhistory <игра> #тег-клана <число недель>` Кубки и донат всех игроков на момент нескольких недель назад. Чтобы включить запись истории вашего клана, напишите оператору бота
- 🔨🤖 `/donations <игра> #тег-клана` Донат всех игроков клана на протяжении последних 6 недель. Слева новые недели, справа старые, текущей недели нет
- 🧑🤖 `/alldonations <игра> #тег-клана` Донат топ-10 игроков (по донату) на протяжении последних 6 недель. Слева новые недели, справа старые, текущей недели нет
- 🧑🤖 `/lowmembers <игра> #тег-клана` Список участников клана (без стариков и соруков) с наименьшими кубками, которые не участвуют в КВ и которых можно сейчас кикать. Наверху списка кубки меньше, снизу больше
- 🧑🤖 `/warlosers <игра> #тег-клана` Список игроков клана с наименьшим процентом выигранных КВ в этом клане. Формат: [кубки] выиграно/всего
- 🧑🤖 `/warwinners <игра> #тег-клана` Список игроков клана с наибольшим процентом выигранных КВ в этом клане. Формат: [кубки] выиграно/всего
- 🧑🤖 `/cwready <игра> #тег-клана` Список игроков клана с худшей прокачкой для КВ. За карту 12+ уровня даётся 2 балла, за карту 11 уровня даётся 1 балл. Формат: ник [кубки] рейтинг
- 🧑🤖 `/lowcwready <игра> #тег-клана` Список 10 игроков клана с худшей прокачкой для КВ. За карту 12+ уровня даётся 2 балла, за карту 11 уровня даётся 1 балл. Формат: ник [кубки] рейтинг

Если для беседы задан клан по умолчанию (`/setclan`), то `<игра> #тег-клана` можно не указывать.
