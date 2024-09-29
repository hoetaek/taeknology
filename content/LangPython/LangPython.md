---
tags: []
---
[[poetry]]
[[pytest]]

## 입력이 끝날 때까지 값을 받아오는 방법
```python
while True:
    try:
        print(input())
	except EOFError:
		break
```

# Poetry
## poetry로 프로젝트 내부에 virtualenv 환경 구축하는 방법
```sh
poetry config virtualenvs.in-project true
poetry config virtualenvs.path "./.venv"

# 프로젝트 내부에 venv 새로 설치
poetry install && poetry update
```
[링크](https://amazingguni.medium.com/python-poetry%EB%A5%BC-%EC%82%AC%EC%9A%A9%ED%95%98%EB%8A%94-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%EB%A5%BC-vscode%EC%97%90%EC%84%9C-%EA%B0%9C%EB%B0%9C%ED%95%A0-%EB%95%8C-interpreter%EB%A5%BC-%EC%9E%A1%EB%8A%94-%EB%B0%A9%EB%B2%95-e1806f093e6d)

# Pyte
## fixture
- 공통으로 쓰이는 변수를 fixture로 사용할 수 있다
- convention으로 conftest.py에 다른 테스트에서 공통으로 쓰이는 fixture를 정의함
- conftest와 같은 위치 혹은 하위 폴더에 위치한 파일들은 모두 그 fixture를 사용할 수 있다
## pytest 병렬적으로 돌리기
`pip install pytest-xdist`
`pytest -n 3`

[[issue - moderate effect]]

## 활용 팁
- 승희 누나 방식처럼 tests 폴더를 앱 디렉토리와 같은 단계에 두니 관리하기 편리함
- conftest는 위에서 언급한 방식대로 하면 됨