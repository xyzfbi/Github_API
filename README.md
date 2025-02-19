# Получение данных о публичной информации профиля GitHub.
Программа на Python позволяет получить информацию о профиле пользователя GitHub, включая количество звёзд, коммитов, репозиториев, подписчиков и других данных. Скрипт использует GitHub API для получения данных.

## Зависимости
Для корректной работы программы понадобится python версии 3.8 и выше.

## Установка программы
1. `pip install requests python-dotenv`

2. Создать файл в формате `.env`
3. Добавить в него строку: 
`API_KEY = <ваш токен Github>`\
Найти токен можно по пути `Settings->Developer settings->Tokens`
## Запуска программы
В командной строке: `python Github_api.py`



## Дополнительная информация
* Для получения приватной ифнормации о своем профиле - расскомментировать строки:
  1. `'''HEADERS = {"Authorization": f"Bearer {TOKEN}",
             "Accept": "application/vnd.github+json"}'''`
  2. `    # response = requests.get(url, headers=HEADERS, timeout=5)`

  3. `    # response_stars = requests.get(stars_url, headers=HEADERS, timeout=5)`
  4. `        # commits_response = requests.get(commits_url, headers=HEADERS, timeout=5)`
* Удалить заменяющие их строки.
