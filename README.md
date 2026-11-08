# Анализ каталога фильмов

Учебный проект из 9 этапов (22 задачи) на Python 3.12. Единственный исполняемый скрипт — `catalog_analysis.py`.

## Запуск

```bash
uv sync
uv run catalog_analysis.py
uv run ruff check .
```

Для знакомства с заданиями 3 и 8 можно отдельно выполнить:

```bash
uv run python -c 'from catalog_analysis import *; print_non_comedy(movies)'
uv run python -c 'from catalog_analysis import *; print(find_first_masterpiece(movies)); find_first_masterpiece([])'
uv run python -c 'from catalog_analysis import *; demonstrate_generators(movies)'
```

При успешном запуске выводится средний рейтинг 7.2, средний возраст 8 лет и топ-3 фильмов. Для воспроизводимого окружения коммитьте `pyproject.toml` и `uv.lock`, а `.venv` не добавляйте в Git.
