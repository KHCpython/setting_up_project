
2025873019 손형석 파이썬 리포트입니다.

프로그램을 작동시키기 위한 절차 안내입니다.

1. 코드 내려받기
   터미널을 열고 아래 명령을 입력하세요.  
   
   git clone https://github.com/KHCpython/setting_up_project.git
   cd setting_up_project

2. 가상환경 만들기 및 활성
conda create -n ll_env python=3.12
conda activate ll_env

3. 패키지 설치하기
pip install django
pip freeze > requirements.txt

4. DB설정
python manage.py migrate
python manage.py createsuperuser

5. 실행
python manage.py runserver

