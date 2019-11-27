## HEROKU

1. pip install

   ```bash
   $ Django
   $ django-decouple 
   $ django-heroku  
   $ gunicorn
   ```

2. setting설정

   - import django_heroku
   - django_heroku.settings(locals())

3. Procfile파일 만들기

   - web: gunicorn heroku_test.wsgi(프로젝트 이름명으로 설정) --log-file - 

4. runtime.txt파일 만들기

   -  python-3.7.4(자신의 버전에 맞게설정)

5. $ pip freeze > requirements.txt

6. heroku 사이트 들어가서 Heroku CLI 다운로드

   ```bash
   $ heroku # heroku상태확인
   $ heroku login # heroku login하기
   $ heroku create # herokuApp 만들기(name을 설정하면 랜덤으로 생성)
   ```

   

7. heroku에 올리기

   ```bash
   $ git push heroku master
   ```