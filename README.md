# greet-ci

인사말 출력 프로그램 및 GitHub Actions CI 실습 프로젝트입니다.

## 요구사항
- Python >= 3.11
- uv

## 설치
```bash
uv sync --locked
```

## 실행
```bash
uv run --locked python greet.py Hee
# 출력: Hello, Hee!

uv run --locked python greet.py
# 출력: Hello, world!
```

## 테스트 및 검증
```bash
uv run --locked pytest -q greet.py
uv run --locked black --check greet.py
uv run --locked flake8 greet.py
uv run --locked mypy greet.py
uv build
```
