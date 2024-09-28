## poetry로 프로젝트 내부에 virtualenv 환경 구축하는 방법
```sh
poetry config virtualenvs.in-project true
poetry config virtualenvs.path "./.venv"

# 프로젝트 내부에 venv 새로 설치
poetry install && poetry update
```
[링크](https://amazingguni.medium.com/python-poetry%EB%A5%BC-%EC%82%AC%EC%9A%A9%ED%95%98%EB%8A%94-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%EB%A5%BC-vscode%EC%97%90%EC%84%9C-%EA%B0%9C%EB%B0%9C%ED%95%A0-%EB%95%8C-interpreter%EB%A5%BC-%EC%9E%A1%EB%8A%94-%EB%B0%A9%EB%B2%95-e1806f093e6d)
