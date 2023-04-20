# Django permissions translation

#### A simple way to translate the permissions of your Django project.

## Overview

This package helps you translate the permissions of your Django project.<br> 
It's very useful when you have a project with multiple languages or when you use the Django Admin for end users.

## Requirements
- Python 3.8+
- Django 4.2 (tested)

## Installation

```bash
pip install django-perm-trans
```

#### settings.py
```python
INSTALLED_APPS = [
    ...
    'django_perm_trans',
    ...
]
```

##### Configuration
```python
DJANGO_PERM_TRANS = {
    'separator': '->', # Default: '|' - Separator between words (change | to ->)
    # 'capitalize_words': True, # Default: False
    # 'remove_app': True, # Default: False
    # 'remove_model': True, # Default: False
    
    # Custom function to translate the permission and format
    # ATTENTION: This function overrides the other options
    # 'custom_function': lambda perm: perm.name, # Default: None
}
```


## Roadmap

- [x] Apply of capitalize in the words.
- [x] Separator configurable.
- [x] Remove app name from the permission.
- [x] Remove model name from the permission.
- [x] Custom function to translate the permission.
- [ ] Unit tests.
- [ ] Compatibility tests (Django versions).
- [ ] Use translation from database (configurable in admin).
- [ ] Command to translate the permissions from API.
- [ ] Documentation.


## License
[MIT](LICENSE.md)