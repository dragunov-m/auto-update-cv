# Auto-update CV
Скрипт для автоматического обновления резюме на сайтах hh.ru / rabota.by

Работает на Windows / Linux / Mac OS

Зависимости:
1. __Selenium__
2. __Google Chrome:__ [__Windows__, __Linux__ и __MacOS__](https://www.google.com/intl/ru/chrome/)
 - __Linux__ без графической оболочки - wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb

3. [__Chromedriver__](https://chromedriver.chromium.org/downloads), выбирайте исходя из вашей версии Google Chrome

***Необходим первый запуск через терминал, где нужно выбрать сайт и внести данные!***

# Планировщики задач

**LINUX или MAC OS**

Вызовите cron через команду 
```
crontab -e
```

Задайте внизу условие и сохраните
```
*/40 * * * * python -u /path/where/locate/script/hh.py >> /path/where/locate/log/crontab_chromedriver_error.log 2>&1
```

**WINDOWS**

Для Windows вам понадобится создать bat-файл.

В нём укажите директорию к бинарному файлу python и директорию куда загружен скрипт

```
C:\you-folder\python.exe C:\you-folder\hh-win.py
pause
```

![1](https://i.imgur.com/O5NF5Fa.png)
![2](https://i.imgur.com/jxcvidK.png)
![3](https://i.imgur.com/NnLALQV.png)
![4](https://i.imgur.com/lkPsGKs.png)
![5](https://i.imgur.com/04ewFOQ.png)
![6](https://i.imgur.com/6DIiBqd.png)
![7](https://i.imgur.com/WGE3UrE.png)

__WARNING!__ : Не рекомендую убирать тайминги, т.к. вам подсунут captch-у или просто дропнут.
