# [Сборный проект-2. Восстановление золота из руды](https://github.com/IvanZhoglik/yandex-practicum-projects/blob/main/09_integrated_project_2/integrated_project_2.ipynb)

## Описание проекта

Для Компании, разрабатывающей решения для эффективной работы промышленных предприятий, требуется разработать модель машиннного обучения. Можель должна предсказать коэффициент восстановления золота из золотосодержащей руды.

## Цель работы

Подготовка прототипа модели машинного обучения.

## Описание данных

**Технологический процесс**
<br>Rougher feed — исходное сырье
<br>Rougher additions (или reagent additions) — флотационные реагенты: Xanthate, Sulphate, Depressant
<br>Xanthate — ксантогенат (промотер, или активатор флотации);
<br>Sulphate — сульфат (на данном производстве сульфид натрия);
<br>Depressant — депрессант (силикат натрия).
<br>Rougher process (англ. «грубый процесс») — флотация
<br>Rougher tails — отвальные хвосты
<br>Float banks — флотационная установка
<br>Cleaner process — очистка
<br>Rougher Au — черновой концентрат золота
<br>Final Au — финальный концентрат золота

**Параметры этапов**
<br>air amount — объём воздуха
<br>fluid levels — уровень жидкости
<br>feed size — размер гранул сырья
<br>feed rate — скорость подачи

**Наименование признаков**
<br>Наименование признаков должно быть такое:
<br>[этап].[тип_параметра].[название_параметра]
<br>Пример: rougher.input.feed_ag

Возможные значения для блока [этап]:
<br>rougher — флотация
<br>primary_cleaner — первичная очистка
<br>secondary_cleaner — вторичная очистка
<br>final — финальные характеристики

Возможные значения для блока [тип_параметра]:
<br>input — параметры сырья
<br>output — параметры продукта
<br>state — параметры, характеризующие текущее состояние этапа
<br>calculation — расчётные характеристики

## Структура проекта

1. Подготовка данных
<br>1.1  Датасет recovery_train
<br>1.2  Датасет recovery_test
<br>1.3  Датасет recovery_full
<br>1.4  Проверка расчета эффективности обогащения признака rougher.output.recovery
<br>1.5  Анализ признаков, недоступных в тестовой выборке
<br>1.6  Предобработка данных
2. Анализ данных
<br>2.1  Анализ концентрации металлов (Au, Ag, Pb) на различных этапах очистки
<br>2.2  Анализ распределения размеров гранул сырья на обучающей и тестовой выборках
<br>2.3  Исследование суммарной концентрации всех веществ на разных стадиях: в сырье, в черновом и финальном концентратах
3. Модель
<br>3.1  Функция для вычисления итоговой sMAPE
<br>3.2  Обучение моделей и выбор лучшей модели
<br>3.3  Проверка модели на тестовой выборке
<br>3.4  Проверка модели на адекватность
4. Общий вывод

## Используемые библиотеки
`pandas` `matplotlib` `seaborn` `numpy` `sklearn`
