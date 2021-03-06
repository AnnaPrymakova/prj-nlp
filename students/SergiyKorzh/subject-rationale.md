# Обгрунтування вибору теми

## Тема:
Автоматична генерація відповідей на запитання на сайті https://ukrainian.stackexchange.com (та інших SE сайтах).
 

## Чому саме ця тема

1. Це завдання включає в себе більшість з можливих типів NLP-задач: Linguistic, Analysis та Generation (за виключенням хиба що Transformation)

2. Це дуже практичне завдання, робота над яким (я сподіваюсь) буде корисною для проекта, над яким я зараз працюю (Aistant)


## Що буде в результаті
В кінцевому результаті це буде веб-сторінка (другій варіант: чат бот) на якій можна ставити запитання та отримувати відповіді з деякої бази SE


## Основні етапи

### 1. Збір даних
Треба буде або написати веб-скрапер для сторінок потрібного розділу StackExchange (https://ukrainian.stackexchange.com) або просто завантажити БД (https://archive.org/details/stackexchange) та витягнути потрібні дані звідти.


### 2. Побудова моделі
Скоріш за все доведеться побудувати щось на зразок пошукового індексу, щоб за текстом питання, що його ввів користувач, правильно знаходити у базі запитання, яке там вже було. А значить і віповідь на нього (якщо вона є звісно).

### 3. MVP
На цьому етапі ми зробимо варіант рішення який буде просто шукати питання у базі та видавати їснуючу відповідь якщо вона там є. Або якусь стандартру відповідь якщо ми не можемо знайти у нашому індексу запитання за введеним текстом.
На цьому етапі у нас має бути можливість оцінити результат роботи алгоритму на деякому тестовому набору питань-відповідей.


### 4. Вдосконалення 
Якимось чином вдосконалюємо пошуковий алгоритм, щоб покращити оцінку.
Можливо в подальшему ще додати навчання нашої моделі: користувач може поставити оцінку чи сподобалась йому відповідь (чи дісйсно відповідає вона на питання) і на основі цієї інформації ми вносимо зміни у модель.



