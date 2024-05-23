# Learning management system using django web framework

Feature-rich learning management system. You may want to build a learning management system(AKA school management system) for a school organization or just for the sake of learning the tech stack and building your portfolio, either way, this project would be a good kickstart for you.

Let's enhance the project by contributing! 👩‍💻👩‍💻

![Screenshot from 2023-12-31 17-36-31](https://github.com/adilmohak/django-lms/assets/60693922/e7fb628a-6275-4160-ae0f-ab27099ab3ca)

## Current features

- Панель инструментов: школьная демография и аналитика. Доступно только администраторам
- Новости и события: все пользователи могут получить доступ к этой странице.
- Администратор управляет студентами (Добавить, Обновить, Удалить)
- Администратор управляет лекторами (Добавить, Обновить, Удалить)
- Студенты могут добавлять и удалять курсы
- Преподаватели представляют оценки студентов: _Посещаемость, Промежуточный экзамен, Итоговый экзамен, Задание_.
- Система автоматически рассчитывает _Общее количество, среднее значение, баллы и оценки учащихся_
- Оценивайте каждого учащегося **зачет**, **не** или **зачет с предупреждением**.
- Страница результатов оценивания для учащихся
- Страница результатов оценок для учащихся
- Управление сессиями/годами и семестрами
- Оценки и оценки будут сгруппированы по семестрам.
- Загрузите видео и документацию для каждого курса.
- Генератор PDF-файлов для регистрации учащихся и результатов оценок.
- Ограничение доступа к странице
- Сохранение результатов викторины под каждым пользователем
- Рандомизация порядка вопросов
- Результаты предыдущих тестов можно просмотреть на странице категории.
- Правильные ответы могут отображаться после каждого вопроса или все сразу в конце.
- Пользователи, вошедшие в систему, могут вернуться к незавершенному тесту, чтобы завершить его, а пользователи, не вошедшие в систему, могут завершить тест, если их сеанс сохраняется.
- Викторина может быть ограничена одной попыткой для каждого пользователя.
- Вопросам можно присвоить категорию
- Уровень успеха для каждой категории можно отслеживать на странице прогресса.
- Для каждого результата вопроса может быть дано объяснение
- Можно установить проходные баллы
- Тип вопроса с множественным выбором
- Тип вопроса «Верно/Неверно»
- Тип вопроса для эссе
- Специальное сообщение отображается для тех, кто прошел или не прошел тест.
- Добавлено специальное разрешение (view_sittings), позволяющее пользователям с этим разрешением просматривать результаты викторины от пользователей.
- Страница оценивания, на которой перечислены выполненные тесты, может фильтроваться по тесту или пользователю и используется для отметки вопросов эссе.
# Quick note for future contributors

If you would like to contribute, simply begin by implementing one from the list in the `TODO.md` file.

# Requirements:

> The following programs are required to run the project

- [Python3.8+](https://www.python.org/downloads/)
- [PostgreSQL database](https://www.postgresql.org/download/)
- [Redis](https://redis.io/docs/latest/operate/oss_and_stack/install/install-redis/)

# Installation

- Clone the repo with

```bash
git clone https://github.com/adilmohak/django-lms.git
```

- Create and activate a python virtual environment

```bash
pip install -r requirements.txt
```

- Create `.env` file inside the root directory and include the following variables

```bash
# Database config
DB_NAME=[YOUR_DB_NAME]
DB_USER=[DB_ADMIN_NAME]
DB_PASSWORD=[DB_ADMIN_PASSWORD]
DB_HOST=localhost
DB_PORT=[YOUR_POSTGRES_PORT default is 5432]

# Email config
EMAIL_FROM_ADDRESS=Django LMS <youremail@example.com>
EMAIL_HOST_USER=[YOUR_EMAIL]
EMAIL_HOST_PASSWORD=[YOUR_EMAIL_PASSWORD]

# Other
DEBUG=True
SECRET_KEY=[YOUR_SECRET_KEY]
```

```bash
python manage.py migrate
```

```bash
python manage.py createsuperuser
```

```bash
python manage.py runserver
```

Make sure your Redis server is running

```bash
redis-server
```

Start the celery worker

```bash
celery -A config.celery worker -l INFO
```

Last but not least, go to this address http://127.0.0.1:8000

### References

- Quiz part: https://github.com/tomwalker/django_quiz

# Connect with me

<div>
<a href="https://www.linkedin.com/in/adilmohak" target="_blank">
<img src=https://img.shields.io/badge/linkedin-%231E77B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white alt=linkedin style="margin-bottom: 5px;" />
</a>
<a href="https://github.com/adilmohak" target="_blank">
<img src=https://img.shields.io/badge/github-%2324292e.svg?&style=for-the-badge&logo=github&logoColor=white alt=github style="margin-bottom: 5px;" />
</a>
<a href="https://stackoverflow.com/users/12872688/adil-mohak" target="_blank">
<img src=https://img.shields.io/badge/stackoverflow-%23F28032.svg?&style=for-the-badge&logo=stackoverflow&logoColor=white alt=stackoverflow style="margin-bottom: 5px;" />
</a>
<a href="https://www.facebook.com/adilmohak1" target="_blank">
<img src=https://img.shields.io/badge/facebook-%232E87FB.svg?&style=for-the-badge&logo=facebook&logoColor=white alt=facebook style="margin-bottom: 5px;" />
</a>
</div>

# Support

<p><a href="https://www.buymeacoffee.com/adilmohak"> <img align="left" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="adilmohak" /></a></p><br><br>

#### Show your support by ⭐️ this project!
"# django-lms" 
