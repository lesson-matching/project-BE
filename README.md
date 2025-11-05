version: Python 3.13.9
DB_migrations 폴더 내의 마이그레이션 파일로 DB 구조 획일화
src 폴더 내에 소스 코드 보관

터미널로 프로젝트 폴더 내로 이동하여, 파이썬 가상환경 생성
py -3.13.9 -m venv venv

가상환경 활성화(터미널에서)
# PowerShell
.\venv\Scripts\Activate.ps1

# cmd
.\venv\Scripts\activate.bat

가상환경 활성화 후, requirements.txt의 패키지를 설치.
pip install -r requirements.txt

DB_migrations 폴더의 마이그레이션 파일을 참고해 DB를 초기화.
