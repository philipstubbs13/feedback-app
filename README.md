# Build and Deploy a Python Web App

* <https://www.youtube.com/watch?v=w25ea_I89iM>
* Python Heroku Deployment: <https://gist.github.com/bradtraversy/0029d655269c8a972df726ed0ac56b88>

```bash
>>> from app import db
>>> db.create_all()
>>> exit()
```

```bash
heroku --version

heroku login

heroku create lexusfeedback13

heroku addons:create heroku-postgresql:hobby-dev --app lexusfeedback13

heroku config --app lexusfeedback13

pip freeze > requirements.txt

touch Procfile

heroku git:remote -a lexusfeedback13

git push heroku master

heroku open

heroku run python
from app import db
db.create_all()
exit()

heroku pg:psql --app lexusfeedback13
select * from feedback
```