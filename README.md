# dota2_prediction_model
Задача проекта - построить модель бинарной классификации исхода матча в игре Dota 2.

В Dota 2 участвуют две команды: Radiant и Dire. Нужно оценить вероятность победы команды Radiant.

В обычной игре Dota 2 каждая из двух команд — Radiant и Dire — состоит из 5 игроков. Каждый игрок выбирает героя, который играет определённую роль. Dota 2 — командная игра, поэтому состав команды имеет большое значение. Карта игры содержит базы команд (фонтан), 3 линии для каждой стороны, магазины, логово Рошана и другие элементы. В течение игры игроки улучшают своих героев, покупают предметы, разрушают башни, убивают героев противника, фармят крипов врага и "отрекаются" от своих крипов (не дают их убивать врагу). Цель игры — разрушить фонтан противника, и ничья невозможна.

Для оценки используется метрика ROC-AUC. Результат этой задачи — бинарный: для каждой игры нужно предсказать победу команды Radiant (1) или поражение (0). Поскольку мы оцениваем вероятность исхода, результат будет находиться в интервале [0,1]. Затем это значение сравнивается с определённым порогом для получения бинарного ответа.
