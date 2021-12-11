# django_ai_test_deployment
django_ai_test_deployment




Managing Virtual Environments With virtualenvwrapper

$ pip install virtualenvwrapper
Note: For Windows, you should use virtualenvwrapper-win instead.

Once it’s installed, we’ll need to activate its shell functions. 
$ which virtualenvwrapper.sh

shell commands available help to manage the environments. Here are just a few of the ones available:

workon
deactivate
mkvirtualenv
cdvirtualenv
rmvirtualenv

Now, anytime you want to start a new project, you just have to do this:

$ mkvirtualenv my-new-project
(my-new-project) $
This will create and activate a new environment in the directory located at $WORKON_HOME, where all virtualenvwrapper environments are stored.

To stop using that environment, you just need to deactivate it like before:

(my-new-project) $ deactivate
$
If you have many environments to choose from, you can list them all with the workon function:

$ workon
my-new-project
my-django-project
web-scraper
Finally, here’s how to activate:

$ workon web-scraper
(web-scraper) $
If you would like to be able to use a single tool and switch between Python versions, virtualenv will allow you to do just that. virtualenv has a parameter -p that allows you to select which version of Python to use. Combine that with the which command, and we can easily select your preferred version of Python to use in a simple manner. For example, let’s say that we want Python 3 as our preferred version:

$ virtualenv -p $(which python3) blog_virtualenv
This will create a new Python 3 environment.
