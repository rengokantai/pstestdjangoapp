# pstestdjangoapp

## 5. Integration Testing in Django
```
django.test.TransactionTestCase
django.test.TestCase
django.test.LiveServerTestCase
```
what to avoid
- Unpredicable Tests: Tests that can be subject to different outcome based on race conditions or third place
- Too much details: Tests are written with a unit testing mentality or focus on too many testable features at once  



## 6. Measuring Test Coverage
### 2 Measuring Your Own Coverage
```
coverage run manage.py test
```
rich
```
coverage html
open htmlcov/index.html
```
create .converagerc
```
[run]
branch = True
omit = *.virtualenvs/*
       *.__init__.py
       */test*.py
       */migrations/*
       */urls.py
       */manage.py
       tasks/admin.py
       tasks/apps.py
```

```
coverage report
```
