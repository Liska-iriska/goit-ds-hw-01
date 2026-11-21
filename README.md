# goit-pycore-hw-08 — Персональний помічник

CLI-бот для адресної книги (контакти, телефони, дні народження).

## Віртуальне середовище (Poetry)
Інструмент: **Poetry**. Python: **3.13** (`python = "~3.13"` у `pyproject.toml`).
Сторонніх залежностей немає (лише стандартна бібліотека).

```
poetry env use python3.13
poetry install --no-root
poetry run python bot.py
```
У IDE (VS Code / PyCharm) обери інтерпретатор `.venv/bin/python` (`poetry env info --path`).

## Docker
```
docker build -t personal-assistant .
docker run -it personal-assistant            # запускає бота
docker run -it personal-assistant /bin/bash  # оболонка контейнера, далі: python bot.py
docker exec -it <container-id> /bin/bash     # у запущений контейнер
```
