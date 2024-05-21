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