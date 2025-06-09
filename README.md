
2025873019 손형석 파이썬 리포트입니다.

프로그램을 작동시키기 위한 절차 안내입니다.

추가적으로 ll_admin/ll_admin 계정으로 로그인 해야만 모든 글을 다 볼 수 있습니다. 다른 계정은 모든 글이 보이지 않습니다.

아래 명령어들을 아나콘다 프롬프트에 작성하세요(Y/N에선 Y 선택)

1. 코드 내려받기
git clone https://github.com/KHCpython/setting_up_project.git
cd setting_up_project

2. 가상환경 생성·활성화
conda create -n ll_env python=3.12
conda activate ll_env

3. Django 설치
conda install django

4. DB 마이그레이션
python manage.py migrate

5. DB로 불러오
python manage.py loaddata fixtures/posts_fixture.json

6. 슈퍼유저 생성 (아이디와 비밀번호 모두 ll_admin 으로 입력)
python manage.py createsuperuser
Username: ll_admin
Password: ll_admin

7. 개발 서버 실행
python manage.py runserver

