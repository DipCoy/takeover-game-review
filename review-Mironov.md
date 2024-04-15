# Ревью. Миронов Данил

## Общее
Моё почтение! Это выглядит прям бомбически. Респектос, что решились отрисовывать некоторые части напрямую через память и спрайты. 

Было интересно потыкаться в игру, но имхо поле очень большое, я так и не дошёл до конца игры. Быть может, было бы круто, если бы у пользователя была возможность задать размер поля.

Но отрисовано капец круто!

Только я чет не сразу догнал, что значит это правило *последующие ходы вы должны рисовать территории, которые присоединены к вашей хотя бы на 1 клетку*. Только после того, как увидел пример на Пикабу (спасибо за ссылочку).

## Возможности
Круто, что можно играть вдвоём. Было бы ещё круче, если бы было PVE, но это явно не на Джеке писать, а то глаза потекут, появятся мысли о суесыде))

Классно, что клеточки игроков по-разному отрисовываются. Да и вообще как по мне дизайн офигенен.

## Декомпозиция кода
Тут всё очень хорошо. Единственное, где, как мне кажется, логика представления просочилась в модель - это в файле **Player.jack**. Там вызывается и Output методы и начисление очков вместе.

Круто, что вынесли некоторые константы в отдельный класс **Consts**, но правда не все). Кажется, туда же можно поместить коды клавиш и время ожидания для **Sys.wait**. К отрисовке это не относится - там конечно всегда треш с байтами.

В классе валидатора **Validator.jack** есть небольшое дублирование с четырьмя циклами в методе **isAreaJoinedToExisting**. Но это пожалуй всё, в остальном всё отлично.

## Интересные трюки
Мне понравилось, что вы сделали по-нормальному мапинг игрового поля в пиксели на экране. Типа да, там простая математика, но всё равно круто, что получилось настолько хорошо отделить бизнес логику от логики представления.

## Объём кода
Ну не большой, не маленький. Средний такой по России код)))
Круто, что такую нетривиальную игру получилось довольно элегантно выразить на ~~конченном~~ Джеке.

## Оценочное мнение
Пушка-бомба. Ребятам респект.