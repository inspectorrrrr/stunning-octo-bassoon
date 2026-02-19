# Тестовые задания для Junior QA



---

## Задача 1: Тест-кейсы (Оплата картой)

Файл: `/task_1.md`

Содержит 17 тест-кейсов в табличном формате:
- Позитивный сценарий
- Негативные сценарии
- Проверка валидации
- Граничные значения
- Интеграция с платёжным шлюзом

---
## Задача 2: Playwright автотест

Файл: `tests/test_playwright_title.py`

Тест открывает страницу `https://playwright.dev/` и проверяет, что заголовок содержит слово **"Playwright"**. Запускается на двух браузерах: **Chromium** и **Firefox**.

---

### Шаг 1: Подготовка окружения

```bash
# 1. Создайте виртуальное окружение
python -m venv venv

# 2. Активируйте его:
# Для Linux/Mac:
source venv/bin/activate
# Для Windows:
venv\Scripts\activate

# 3. Установите зависимости
pip install pytest pytest-playwright

# 4. Установите браузеры для тестов
playwright install chromium firefox
```

---

### Шаг 2: Запуск теста

#### Запуск на двух браузерах:
```bash
pytest tests/test_playwright_title.py -v -s --browser chromium --browser firefox
```

#### Запуск на одном браузере:
```bash
# Только Chromium
pytest tests/test_playwright_title.py -v -s --browser chromium

# Только Firefox
pytest tests/test_playwright_title.py -v -s --browser firefox
```
## Задача 3: Теория вероятности

Файл: `/task_3.md`

Решение задачи: *«Монету подбрасывают три раза. Какова вероятность того, что выпадет ровно два орла?»*
 
> **Ответ:** 3/8 = 0.375 = 37.5%