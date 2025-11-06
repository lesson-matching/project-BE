- version: Python 3.10.11
- DB_migrations 폴더 내부에 마이그레이션 파일을 생성하여 SQLite를 이용한 DB 구조 공유
- src 폴더 내에 소스 코드 보관

- 터미널로 프로젝트 폴더 내로 이동하여, 파이썬 가상환경 생성
- py -3.10 -m venv venv

``` .gitignore에 아래와 같은 내용이 들어가 있어야 함. (db 파일, sqlite3 파일은 직접 공유하지 않고 마이그레이션으로 공유할 예정이기 때문.)
# filepath: .gitignore
venv/
__pycache__/
*.db
*.sqlite3
```
가상환경 활성화(터미널에서)
```
# PowerShell
.\venv\Scripts\Activate.ps1

# cmd
.\venv\Scripts\activate.bat
```

- 가상환경 활성화 후, requirements.txt의 패키지를 설치.
` pip install -r requirements.txt ` (지금은 아무것도 없어요)

DB_migrations 폴더의 마이그레이션 파일을 참고해 DB를 초기화.

- 지금은 폴더 생성용으로 더미 파일 넣어서 디렉터리만 분류해 놨어요.