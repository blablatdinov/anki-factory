Создайте контроллер (view), которая возвращает Простой html в приложении `exersize`,
которая возвращает `<h1>Hello, wolrd!</h1>`. На url `/exerizes/hello`

Для проверки можете запустить:
```bash
pytest exersizes/tests/...
```
%
```python
# exersizes/urls/hello.py
from django.url import path

from exersizes.views.hello import hello_view

urlpatterns = [
    path('hello/', hello_view),
]
# exersizes/views/hello.py
def hello_view(request):
    return '<h1>Hello, world</h1>'
```
