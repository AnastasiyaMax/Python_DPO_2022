# Python_DPO_2021_fall

Преподаватель – Максимовская Анастасия.

Материалы готовили Ян Пиле, Татьяна Рогович, Анастасия Максимовская.

Расписание занятий и список тем можно посмотреть [здесь](https://docs.google.com/spreadsheets/d/1OlJgZRiDicDdyn9jiz5yNyce0h13Ir7Np2gqdWwoUxE). Материалы лекций находятся в папках в этом репозитории.

Семинарские контесты хранятся в этом гугл-документе (появится позже).

* Задачи для семинара 1 – https://official.contest.yandex.ru/contest/29243/enter/
* Задачи для семинара 2 – https://official.contest.yandex.ru/contest/29360/enter/
* * Задачи для семинара 3 – https://official.contest.yandex.ru/contest/29484/enter/

## О курсе

Курс разделен на 3 части: основы программирования на python (8 занятий), сбор данных с помощью python (4 занятия), анализ данных на python (6 занятий).

**Формы контроля по основам программирования:**
* [Домашнее задание 1](https://official.contest.yandex.ru/contest/29361/enter/) – типы данных, условный оператор (выдается после 2 занятия)
* *Домашнее задание Р – регулярные выражения (выдается после 4 занятия) – БОНУС (необязательно)*
* Домашнее задание 2 – циклы, функции (выдается после 5 занятия)
* Домашнее задание 3 – классы (выдается после 7 занятия)
* *Домашняя контрольная по Python – БОНУС (необязательно)*

**Формы контроля по сбору данных:**

Обязательно нужно сделать или проект 2, или проект 3. Если сделаете оба, то оценка за второй пойдет как БОНУС.

* Проект 1 (первая часть) – парсинг данных с помощью requests и BeautifulSoup (выдается после 9 занятия)
* Проект 2 – сбор данных через API (выдается после 10 занятия)
* Проект 3 – сбор данных с помощью Selenium (выдается после 11 занятия).

* **Финальный проект по двум частям курса** – телеграм-бот, см. описание ниже + лекцию 12 (выдается после 12 занятия).

**Формы контроля по анализу данных**:
* Домашнее задание 4 – задания на использование библиотек pandas, numpy (выдается после 15 занятия)
* Проект 1 (вторая часть) – анализ и визуализация собранных данных (выдается после 17 занятия)

### Формула оценки:

О_итог = (ДЗ-1 + ДЗ-2 + ДЗ-3) * 0.15 + ДЗ-Р * 0.1 + КР * 0.15 + (ПРОЕКТ-2 + ПРОЕКТ-3) * 0.1 + БОТ * 0.2 + ПРОЕКТ-1 * 0.15 + ДЗ-4 *  0.1 + 0.1 * Дорешивания семинарских задач (БОНУС)

## Дополнительные материалы

1. [Курс на курсере](https://www.coursera.org/learn/python-osnovy-programmirovaniya) – поможет в изучении основ программирования на Python
2. [pythontutor.ru](https://pythontutor.ru/) – также для основ программирования, но материал текстом :)
3. Учебник Лутца:
* [учебник на английском](https://vk.com/doc44301783_517813011?hash=702af85baf625360b9&dl=95b74aab4d623be4c6)
* [учебник на русском](https://vk.com/doc44301783_517813053?hash=da4e86b2ebc1ab461d&dl=125d77221c81d99db0)


## Как работать с Github?
Для скачивания файлов с Github необязательно иметь аккаунт, достаточно кликнуть на зеленую кнопку Clone or download в правом верхнем углу, выбрать Download ZIP и распаковать архив. В папке DPO_2020_autumn будут все файлы, загруженные на Github на момент скачивания.

Если файл .ipynb сохраняется как текст или с лишним расширением (например, .txt), то нужно выбрать при сохранении тип файла все файлы, 
а не текст, или после сохранения убрать вручную расширение, переименовав файл.

Подробнее про работу с GitHub через клиента можно прочитать [здесь](https://github.com/pileyan/DPO_Python_2021/blob/main/lect01_git_basic_types/2021_DPO_1_0_git.ipynb)

А еще очень рекомендую посмотреть [вот эту ссылку](https://towardsdatascience.com/getting-started-with-git-and-github-6fcd0f2d4ac6)
Здесь в одной статье рассказана бОльшая часть того, что нужно знать про Git.

## Формулировка задания про бота выдается сразу. Она приведена ниже:

Реализовать телеграм-бота для предоставления пользователю некоторой информации из интернета (под капотом лежит парсер). У бота должны быть: набор команд, с помощью которых он отвечает на вопрос пользователя (например, сколько стоит билет на оперу/балет в большом театре на указанную дату на указанные места или какова средняя указанная зарплата на позициях из указанного номера страницы поисковой выдачи на сайте headhunter по запросу ‘аналитик данных’, каков курс доллара на вчера, сегодня, три месяца назад и тд). Обязательные условия:

1) Не должно быть сообщений, на которые бот отвечает неадекватно (у бота есть какая-то линия его взаимодействия с пользователем, если человек вводит какие-то данные неправильно, бот должен об этом сказать, если бот ответил на запрос клиента, программа должна выдать этот ответ и дать пользователю инструкции о том, как произвести новый запрос.) 
2) Должны быть команда с описанием функциональности бота и команда с описанием набора команд (веселая тавтология) , которые бот принимает.
3) бот должен на какой-то из запросов отправлять картиночки и/или смайлики/стикеры/видео
4) под капотом у бота обязательно должен быть парсер какой-то интернет ниформации (чтобы не было “узнать у пользователя его запрос - думать 5 минут - вывести число 42”

В идеале бот должен содержать взаимодействие с базой данных, например, если у вашего бота есть какой-то набор стадий взаимодействия с пользователем, база может хранить состояние последнего запроса пользователя, чтобы каждый вход в бота не обнулял историю (если это имеет смысл) например:

1) Я спрашивал у бота погоду в Усть-Ордынске, но не сказал за какой день
2) Бот запомнил, что я спрашивал про Усть-Ордынск и в момент моего следующего взаимодействия, скажем, через час, бот спросит: "Помню, вы хотели узнать про погоду в Усть-Ордынске, хотите уточнить день?"

ОЦЕНИВАНИЕ:
Реализация парсера - 5 баллов (вы выбрали тему вашего проекта (что будете искать?) и сделали парсер, который принимает ввод от пользователя в блокноте через input, обрабатывает ошибки в запросе и возвращает ответ).  Если вы используете принципиально другую штуку(не парсер): работу с картами, графами, координатами и т.д. Это будет оцениваться отдельно, но в минусе точно не окажетесь.


Дополнительные баллы: у вас сложный поисковый запрос с использованием Selenium или api, с которым пришлось повозиться (+ 1-2 балла)
Ваш парсер реализован внутри телеграм-бота. Бот умеет искать информацию по запросу и обрабатывать ошибку запроса. Бот умеет отвечать только на один запрос (например, выдача заболевших коронавирусом в определенной стране за вчерашний день). + 5 баллов


Опционально aka НЕ ОБЯЗАТЕЛЬНО:
1) Бота можно запустить на сервере heroku (или вашем собственном сервере, если такой имеется) - тогда вам самим не придется держать программу включенной постоянно www.heroku.com + 2 доп. балла **настоятельно рекомендуем это сделать :)**
2) Бот имеет расширенный функционал (уточнение запроса, агрегирование информации и т.д.) + 2 балла
2) Можно научить бота рисовать какие-то графики ( например статистику курса доллара относительно рубля за месяц) и отправлять их вам (картинки мы отправлять умеем, а графики рисовать очень просто: можно собрать интересующие данные в pandas-dataframe и воспользоваться встроенными методами визуализации) + 2 балла

Ни в чем себя не ограничивайте.
развесовка баллов дана, чтобы с помощью крутого бота вы могли компенсировать недоделанные задания 🙂

**Кто очень хочет, может приступать**

Бот вообще не обязан быть таким, как описано выше, если вы собираетесь для него применить что-то принципиально отличающееся от разобранного на курсе, например однажды мне выслали бота, который примерно высчитывал время, за которое человек пешком/на машине доберется из места с конкретными координатами до некоторого другого выбранного места, скажем, ресторана.

Карта Москвы при этом представляется в виде графа и время считается по кратчайшему пути прохода этого графа, загруженность дорог можно учитывать с помощью учета разных весов на ребрах: больше вес – сильнее загружена дорога, такую информацию можно попытаться достать из интернетов, но , как вы понимаете, решение точно не самое тривиальное.

**Ни в чем себя не ограничивайте.**
