---
layout: single
categories: python
---


# BASE_DIR

**PROJECT_ROOT는 현재 파일의 디렉터리이고, BASE_DIR 는 PROJECT_ROOT의 부모 디렉터리이다**

예를 들면, 아래 프로젝트에서 default.py파일의 PROJECT_ROOT는 C:\projects\myproject\config 이며, default.py파일의 BASE_DIR는 C:\projects\myproject 이다

![images](C:\workspace\blogging\peony-eugene.github.io\images\2021-11-10-파이썬\2021-11-10-base_dir.png)


- 코드

```
PROJECT_ROOT = os.path.dirname(os.path.abspath(__file__))
print(PROJECT_ROOT) # C:\projects\myproject\config
```

```
BASE_DIR = os.path.dirname(os.path.dirname(__file__))
print(BASE_DIR) # C:/projects/myproject
```

참고로,`__file__`은 모듈의 현재 파일 이름을 가리킨다

