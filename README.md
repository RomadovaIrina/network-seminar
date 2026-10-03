# Семинар: сети, HTTP, REST API и веб-скрейпинг

Основной файл — `network_seminar.ipynb`. В нём план на 60 минут, теория,
запускаемые локальные примеры, встроенные картинки, вопросы и ссылки на статьи.

## Запуск

После клонирования создайте окружение и установите зависимости (команды для Windows):

```powershell
git clone https://github.com/RomadovaIrina/network-seminar.git
cd network-seminar
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt jupyterlab
.\.venv\Scripts\python.exe -m jupyterlab
```

На macOS/Linux используйте `.venv/bin/python` вместо `.venv\Scripts\python.exe`.
В редакторе ноутбуков выберите интерпретатор из `.venv`, затем выполните ячейки
сверху вниз. В Jupyter с другим ядром установите зависимости в это ядро:

```python
%pip install -r requirements.txt
```

На Windows браузерный пример использует установленный Microsoft Edge.
Если Edge отсутствует или вы запускаете пример на другой ОС, предварительно установите
Chromium Playwright в том же окружении:

```powershell
python -m playwright install chromium
```

Установка пакетов и браузера требует интернета. После подготовки все демонстрации
работают локально, без внешних API, регистрации и настоящих ключей.

## Перед семинаром

1. Проверьте `Restart Kernel → Run All`.
2. Сверните длинные ячейки «Подготовка» и пропускайте блоки «Дополнительно» при основном показе.
3. Используйте расписание первой ячейки; вопросы по ходу включены в время разделов.

Схемы встроены в `.ipynb`; их отдельные PNG-копии лежат в `seminar_figures/`.
Снимок настоящей JS-страницы — `seminar_outputs/js_catalog.png`.
Сохранённые результаты и картинки можно смотреть без запуска кода.
