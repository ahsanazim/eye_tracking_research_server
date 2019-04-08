# Content Extraction API Server

A Python-based API server made using Flask. Deployed to heroku, it responds to a url with the "content" on the linked page. Uses the [goose](https://github.com/goose3/goose3) library to extract content from the page.

***Deployed to heroku:***

links:
* [https://dashboard.heroku.com/apps/](https://dashboard.heroku.com/apps/)
* [https://mysterious-fortress-86319.herokuapp.com/](https://mysterious-fortress-86319.herokuapp.com/)

testing server from command line w/ `curl`:

`curl -X POST -H "Content-Type: text/plain" --data "https://texasobserver.org/anatomy-tragedy/" https://mysterious-fortress-86319.herokuapp.com/`

commands:
* `heroku open`
* `git push heroku master`
* `heroku ps:scale web=1`
* `heroku logs --tail`

***Relevant links:***

* [https://stackoverflow.com/questions/17260338/deploying-flask-with-heroku](https://stackoverflow.com/questions/17260338/deploying-flask-with-heroku)
* [https://devcenter.heroku.com/categories/deployment](https://devcenter.heroku.com/categories/deployment), [https://devcenter.heroku.com/articles/getting-started-with-python](https://devcenter.heroku.com/articles/getting-started-with-python)
* Uses gunicorn [https://medium.com/the-andela-way/deploying-a-python-flask-app-to-heroku-41250bda27d0](https://medium.com/the-andela-way/deploying-a-python-flask-app-to-heroku-41250bda27d0)
