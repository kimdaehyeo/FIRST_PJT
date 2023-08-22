# django

1. 프로젝트 생성


```bash
django-admin startproject first_pjt .
```

2. 가상환경 설정
```bash
python -m venv venv

```


3. 가상환경 활성화/비활성화
```bash
source venv/Scripts/activate
deactivate
```


4. 가상환경 내부에 django 설치
```bash
pip install django
```

5. 서버 실행 확인(종료 : Ctrl + c)
```bash
python manage.py runserver
```

6. 앱 실행
```bash
django-admin startapp first_app<appname>
```

7. 앱 등록
```bash
settings.py 의 INSTALLED_APPS에 appname 등록
```

8. 서버 실행 확인(종료 : Ctrl + c)
```bash
python manage.py runserver
```

9. urls.py
```bash
from first_app import views

urlpatterns = [
    ...
    path('index/', views.index),
]
```

10. views.py
```bash
def index(request):
    return render(request, 'index.html')
```

11. templates 폴더 생성 => index.html 생성

