<<<<<<< Updated upstream
# ML_CP
 Course project
## Итоговый проект курса "Машинное обучение в бизнесе"

Стек:

ML: sklearn, pandas, numpy, xgboost API: flask

Данные: с kaggle - https://www.kaggle.com/c/sberbank-russian-housing-market/data

Задача: предсказать цену жилья по известным признакам (общая площадь, год постройки дома, число комнат)

Используемые признаки:

full_sq (float)
build_year (int)
num_room (int)
Преобразования признаков: NaN и нули заменяю на медиану.

Модель: xgboost

**Клонируем репозиторий и создаем образ:**

$ git clone https://github.com/Slonozebra/ML_CP.git

$ cd ML_CP

$ docker build -t course_project .

Запускаем контейнер:

Здесь Вам нужно создать каталог локально и сохранить туда предобученную модель (<your_local_path_to_pretrained_models> нужно заменить на полный путь к этому каталогу)

$ docker run -d -p 8180:8180 -p 8181:8181 -v <your_local_path_to_pretrained_models>:/app/app/models course_project
Переходим на localhost:8181
=======
# python-flask-docker
Итоговый проект (пример) курса "Машинное обучение в бизнесе"

Стек:

ML: sklearn, pandas, numpy
API: flask
Данные: с kaggle - https://www.kaggle.com/spscientist/students-performance-in-exams

Задача: предсказать по данным обучения пол ученика (поле gender). Бинарная классификация

Используемые признаки:

- race/ethnicity (категория)
- parental level of education(категория)
- lunch(категория)
- test preparation course(категория)
- math score(значение)
- reading score(значение)
- writing score(значение)

Преобразования признаков: категориальные - OHE, числовые значения - стандартизация

Модель: logreg

### Клонируем репозиторий и создаем образ
```

$ git clone https://github.com/Slonozebra/ML_CP.git
$ cd ML_CP
$ docker build -t 1/gb_docker_flask_ .
```

### Запускаем контейнер
```
$ docker run -d -p 8180:8180 -p 8181:8181 1/gb_docker_flask_
```

### Переходим на localhost:8181
>>>>>>> Stashed changes
