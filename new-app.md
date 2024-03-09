### clone the template repo

```
git clone https://
```

### make a new venv
```
python3 -m venv .venv
```

### upgrade pip and install requirements.txt

### make a settings folder and make a rename to base.py, dev.py and prod.py

To split Django settings into multiple files, you can create a settings directory to replace the settings.py file. Here's a step-by-step guide:

Create a new directory named settings in the same location as your current settings.py.
Move your settings.py into the new settings directory.
Rename settings.py to base.py.
Create new files such as dev.py and prod.py in the settings directory for your development and production settings respectively.
In dev.py and prod.py, import everything from base.py and then override the settings you need.
Here's how the code would look:

base.py
```
# All your base settings go here
```
dev.py
```
from .base import *

# Override base settings here
DEBUG = True
```
prod.py
```
from .base import *

# Override base settings here
DEBUG = False
```
Remember to update the DJANGO_SETTINGS_MODULE environment variable to point to the new settings file. For example, if your project name is myproject, and you want to use the development settings, you would set DJANGO_SETTINGS_MODULE=myproject.settings.dev.

### Start a new app
```
python manage.py startapp XXXXXX
```
and add to settings.py



