## API для тестового задания

### url: `http://rc.appkode.ru:8883`
[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/d9faeef46905c1bd6907)



| Данные  |  Метод API  | 
|---|---|
| Фильмы  |  `GET /films`  | 
| Жанры  |  `GET /genres`  | 
| Фильм во всех кино сегодня  |  `GET /todayFilms`  | 
| Фильмы сегодня  |  `GET /seances`  | 
| Кинотеатры  |  `GET /cinemas`  | 

---
##### Выборка по параметрам происходит следующим образом:
`GET /films?Genre=фантастика&Country=США` - показать все фильмы в жанре фантастика производства США.

##### Ответ:
```
[
  {
    "FilmID": 4,
    "FilmNameRu": "Прибытие",
    "FilmNameEn": "Arrival",
    "Year": "2016",
    "Country": "США",
    "Tagline": "«Why are they here?»",
    "Directore": "Дени Вильнёв",
    "Scenario": "Эрик Хайссерер, Тед Чан",
    "Producer": "Пол Барбо, Глен Баснер, Дэн Коэн",
    "Operator": "Брэдфорд Янг",
    "Composer": "Йохан Йоханнссон",
    "Artist": "Патрис Верметт, Изабель Гюэ, Николас Лепаж",
    "Installation": "Джо Уокер",
    "Genre": "фантастика",
    "Budget": "$47 000 000",
    "ChargesUS": "$63 294 476",
    "ChargesWorld": "$30 900 000",
    "ChargesRu": "$3 493 196",
    "spectators": "863.6 тыс.",
    "PremiereWorld": "1 сентября 2016",
    "PremiereRU": "11 ноября 2016",
    "Age": "16",
    "MPAA": "PG-13",
    "Time": "116",
    "Description": "Неожиданное появление неопознанных летающих объектов в разных точках планеты повергает мир в трепет. Намерения пришельцев не ясны — вооруженные силы всего мира приведены в полную боевую готовность, а лучшие умы человечества пытаются понять, как разговаривать с непрошенными гостями. Правительство обращается за помощью к лингвисту Луизе Бэнкс и физику Яну Доннели, чтобы предотвратить глобальную катастрофу и найти общий язык с пришельцами. Отныне судьба человечества находится в их руках.",
    "Picture": "https://www.kinopoisk.ru/images/film_big/718811.jpg"
  },
  {
    "FilmID": 6,
    "FilmNameRu": "Доктор Стрэндж",
    "FilmNameEn": "Doctor Strange",
    "Year": "2016",
    "Country": "США",
    "Tagline": "«За гранью сознания лежит новая реальность»",
    "Directore": "Скотт Дерриксон",
    "Scenario": "Джон Спэйтс, Скотт Дерриксон, С. Роберт Каргилл",
    "Producer": "Виктория Алонсо, Стивен Бруссар, Луис Д’Эспозито",
    "Operator": "Бен Дэвис",
    "Composer": "Майкл Джаккино",
    "Artist": "Чарльз Вуд, Джим Барр, Томас Браун",
    "Installation": "Сабрина Плиско, Уайатт Смит",
    "Genre": "фантастика",
    "Budget": "$165 000 000",
    "ChargesUS": "$206 488 064",
    "ChargesWorld": "$617 734 618",
    "ChargesRu": "$21 247 427",
    "spectators": "4.9 млн",
    "PremiereWorld": "13 октября 2016",
    "PremiereRU": "31 октября 2016",
    "Age": "16+",
    "MPAA": "PG-13",
    "Time": "115",
    "Description": "Страшная автокатастрофа поставила крест на карьере успешного нейрохирурга Доктора Стрэнджа. Отчаявшись, он отправляется в путешествие в поисках исцеления и открывает в себе невероятные способности к трансформации пространства и времени. Теперь он — связующее звено между параллельными измерениями, а его миссия — защищать жителей Земли и противодействовать Злу, какое бы обличие оно ни принимало.",
    "Picture": "https://www.kinopoisk.ru/images/film_big/409600.jpg"
  }
]
```

---

##### Поиск по ключевому слову:
`GET /films?q=михаил`

##### Ответ:
```
[
  {
    "FilmID": 2,
    "FilmNameRu": "28 панфиловцев",
    "FilmNameEn": "",
    "Year": "2016",
    "Country": "Россия",
    "Tagline": "",
    "Directore": "Ким Дружинин, Андрей Шальопа",
    "Scenario": "Андрей Шальопа",
    "Producer": "Андрей Шальопа, Антон Юдинцев",
    "Operator": "Никита Рождественский",
    "Composer": "Михаил Костылев",
    "Artist": "Екатерина Лизогубова",
    "Installation": "Виталий Виноградов",
    "Genre": "военный",
    "Budget": "$1 700 000",
    "ChargesUS": "",
    "ChargesWorld": "",
    "ChargesRu": "$282 349",
    "spectators": "62.8 тыс.",
    "PremiereWorld": "",
    "PremiereRU": "24 ноября 2016",
    "Age": "12",
    "MPAA": "",
    "Time": "105",
    "Description": "Осенью 1941-го года немецкие части, стоявшие возле Волоколамска, отделяло от Москвы каких-нибудь два часа по шоссе. Однако, на этом шоссе стояла 316-я стрелковая дивизия под командованием генерала И. В. Панфилова. Этот военачальник обладал настолько высоким авторитетом среди личного состава, что бойцы дивизии сами называли себя панфиловцами. А дивизию — панфиловской.",
    "Picture": "https://www.kinopoisk.ru/images/film_big/764465.jpg"
  },
  {
    "FilmID": 9,
    "FilmNameRu": "Эластико",
    "FilmNameEn": "",
    "Year": "2016",
    "Country": "Россия",
    "Tagline": "",
    "Directore": "Михаил Расходников",
    "Scenario": "Жаргал Бадмацыренов, Евгений Замалиев, Александр Кузьминов",
    "Producer": "Георгий Малков, Владимир Поляков, Евгений Замалиев",
    "Operator": "Федор Стручев",
    "Composer": "Александр Вартанов, Александр Колпаков",
    "Artist": "",
    "Installation": "",
    "Genre": "спорт",
    "Budget": "",
    "ChargesUS": "",
    "ChargesWorld": "",
    "ChargesRu": "",
    "spectators": "",
    "PremiereWorld": "",
    "PremiereRU": "24 ноября 2016",
    "Age": "12+",
    "MPAA": "",
    "Time": "85",
    "Description": "Матвей — простой парень из провинциального города. Он вырос с друзьями «на районе», здесь же встретил свою любовь — Дашу. От других Матвея отличают уникальные физические данные — крепкие ноги, мощная дыхалка, поразительная выносливость. Свой талант он использует, выигрывая со своей командой всех в дворовом футболе… и в мелких криминальных авантюрах, которые ему подгоняет друг Каша. Любимую девушку Дашу это очень беспокоит, и она всячески пытается оградить своего парня от необратимой ошибки. А подруги пытаются убедить Дашу бросить Матвея, ведь у нее даже есть перспективный вариант — обеспеченный ухажер Вадим. Неожиданно у Матвея появляется просто сказочная возможность поехать на смотр в Москву в футбольный клуб Премьер-лиги, но он не хочет оставлять Дашу, когда рядом «вьется» Вадим. А для того, чтобы взять её с собой, нужно достать деньги.",
    "Picture": "https://www.kinopoisk.ru/images/film_big/980835.jpg"
  }
]
```

---

##### Пагинация:
`GET /films?_page=2&_limit=3`

* `_page` - номер страницы
* `_limit` - ограничение результатов на страницу

##### Ответ:
```
[
  {
    "FilmID": 4,
    "FilmNameRu": "Прибытие",
    "FilmNameEn": "Arrival",
    "Year": "2016",
    "Country": "США",
    "Tagline": "«Why are they here?»",
    "Directore": "Дени Вильнёв",
    "Scenario": "Эрик Хайссерер, Тед Чан",
    "Producer": "Пол Барбо, Глен Баснер, Дэн Коэн",
    "Operator": "Брэдфорд Янг",
    "Composer": "Йохан Йоханнссон",
    "Artist": "Патрис Верметт, Изабель Гюэ, Николас Лепаж",
    "Installation": "Джо Уокер",
    "Genre": "фантастика",
    "Budget": "$47 000 000",
    "ChargesUS": "$63 294 476",
    "ChargesWorld": "$30 900 000",
    "ChargesRu": "$3 493 196",
    "spectators": "863.6 тыс.",
    "PremiereWorld": "1 сентября 2016",
    "PremiereRU": "11 ноября 2016",
    "Age": "16",
    "MPAA": "PG-13",
    "Time": "116",
    "Description": "Неожиданное появление неопознанных летающих объектов в разных точках планеты повергает мир в трепет. Намерения пришельцев не ясны — вооруженные силы всего мира приведены в полную боевую готовность, а лучшие умы человечества пытаются понять, как разговаривать с непрошенными гостями. Правительство обращается за помощью к лингвисту Луизе Бэнкс и физику Яну Доннели, чтобы предотвратить глобальную катастрофу и найти общий язык с пришельцами. Отныне судьба человечества находится в их руках.",
    "Picture": "https://www.kinopoisk.ru/images/film_big/718811.jpg"
  },
  {
    "FilmID": 5,
    "FilmNameRu": "По соображениям совести",
    "FilmNameEn": "Hacksaw Ridge",
    "Year": "2016",
    "Country": "Австралия, США",
    "Tagline": "«Based on the incredible true story»",
    "Directore": "Мэл Гибсон",
    "Scenario": "Роберт Шенккан, Эндрю Найт",
    "Producer": "Майкл Бэссик, Лоуренс Бендер, Терри Бенедикт",
    "Operator": "Саймон Дагган",
    "Composer": "Руперт Грегсон-Уильямс",
    "Artist": "Бэрри Робисан, Джасинта Леонг, Марк Робинс",
    "Installation": "Джон Гилберт",
    "Genre": "драма",
    "Budget": "$40 000 000",
    "ChargesUS": "$52 608 579",
    "ChargesWorld": "$70 730 343",
    "ChargesRu": "$383 081",
    "spectators": "88.2 тыс.",
    "PremiereWorld": "4 сентября 2016",
    "PremiereRU": "17 ноября 2016",
    "Age": "",
    "MPAA": "R",
    "Time": "139",
    "Description": "Медик Американской армии времён Второй Мировой войны Дезмонд Досс, который служил во время битвы за Окинаву, отказывается убивать людей и становится первым идейным уклонистом в американской истории, удостоенным Медали Почёта.",
    "Picture": "https://www.kinopoisk.ru/images/film_big/649917.jpg"
  },
  {
    "FilmID": 6,
    "FilmNameRu": "Доктор Стрэндж",
    "FilmNameEn": "Doctor Strange",
    "Year": "2016",
    "Country": "США",
    "Tagline": "«За гранью сознания лежит новая реальность»",
    "Directore": "Скотт Дерриксон",
    "Scenario": "Джон Спэйтс, Скотт Дерриксон, С. Роберт Каргилл",
    "Producer": "Виктория Алонсо, Стивен Бруссар, Луис Д’Эспозито",
    "Operator": "Бен Дэвис",
    "Composer": "Майкл Джаккино",
    "Artist": "Чарльз Вуд, Джим Барр, Томас Браун",
    "Installation": "Сабрина Плиско, Уайатт Смит",
    "Genre": "фантастика",
    "Budget": "$165 000 000",
    "ChargesUS": "$206 488 064",
    "ChargesWorld": "$617 734 618",
    "ChargesRu": "$21 247 427",
    "spectators": "4.9 млн",
    "PremiereWorld": "13 октября 2016",
    "PremiereRU": "31 октября 2016",
    "Age": "16+",
    "MPAA": "PG-13",
    "Time": "115",
    "Description": "Страшная автокатастрофа поставила крест на карьере успешного нейрохирурга Доктора Стрэнджа. Отчаявшись, он отправляется в путешествие в поисках исцеления и открывает в себе невероятные способности к трансформации пространства и времени. Теперь он — связующее звено между параллельными измерениями, а его миссия — защищать жителей Земли и противодействовать Злу, какое бы обличие оно ни принимало.",
    "Picture": "https://www.kinopoisk.ru/images/film_big/409600.jpg"
  }
]
```
