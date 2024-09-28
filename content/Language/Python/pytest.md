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