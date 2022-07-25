# Новостной Всемогутор 3000
## Телеграм-бот, который сэкономит время и сделает вашу жизнь проще!

## Stack
[![Python](https://img.shields.io/badge/python-3670A0?style=plastic&logo=python&logoColor=ffdd54)](https://python.org)
[![PyTorch](https://img.shields.io/badge/pytorch-ee4c2d?style=plastic&logo=pytorch&logoColor=white)](https://pytorch.org/)
[![Aiogram](https://img.shields.io/badge/Aiogram-009cfb?style=plastic&logo=aiogram&logoColor=white)](https://docs.aiogram.dev/)
[![Selenium](https://img.shields.io/badge/Selenium-5fbb49?style=plastic&logo=selenium&logoColor=white)](https://www.selenium.dev/)
[![Beautiful Soup](https://img.shields.io/badge/Beautiful_Soup-212528?style=plastic&logo=BeautifulSoup&logoColor=white)](https://www.crummy.com/software/BeautifulSoup/)
[![Tesseract](https://img.shields.io/badge/Tesseract_OCR-158c64?style=plastic&logo=TesseractOCR&logoColor=white)](https://tesseract-ocr.github.io/)
[![HuggingFace](https://img.shields.io/badge/%F0%9F%A4%97-Models%20on%20Hub-yellow)](https://huggingface.co/)

## Функциональность
- Пользователь выбирает ресурс (habr/lenta/wiki), указывает интересующую тему. 
- С помощью библиотек Beautiful Soup, Selenium, Wikipedia происходит парсинг ресурса, выбираются релевантные статьи
- NLP-модель на основе MBart генерит абстрактивное саммари статьи
- Пользователю приходит сгенеренное короткое саммари с голосовой озвучкой и ссылкой на исходную статью
- Раз в день бот присылает статьи по темам, которые пользователь искал ранее

![Header](https://github.com/lena-sapr/final_project/blob/main/assets/1_parsers_resized.gif)

## Дополнительная функциональность:
- Пользователь может отправить длинный текст и бот выдаст его короткое саммари
- Текст для суммаризации может быть отправлен в виде картинки, например, скриншота статьи или документа. Перед тем, как отправить его в модель саммаризации, приложение сделает распознавание (OCR) исходной картинки с помощью Tesseract OCR
- Выделение сущностей (NER - named entity recognition) из введенного текста. Текстовая модель на основе BERT выделит и подсветит такие сущности как: Персоны, Даты, События, Организации, Деньги и т.д, что может быть полезно для анализа текстов
- Оцифровка документов - перевод скриншота или фото документа в редактируемый текст с помощью OCR

![Header](https://github.com/lena-sapr/final_project/blob/main/assets/2_add_feat_resized.gif)


## (БОНУС) Калькулятор расходов
- Пригодится, если несколько людей потратились на общее мероприятие и надо быстро посчитать, кто сколько кому должен перевести. 
- Потраченные суммы можно вводить вручную или прикрепить фото с чеком - бот самостоятельно выделит сумму!

![Header](https://github.com/lena-sapr/final_project/blob/main/assets/3_shekeli_resized.gif)
