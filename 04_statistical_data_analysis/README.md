# [Определение перспективного тарифа для телеком компании](https://github.com/IvanZhoglik/yandex-practicum-projects/blob/main/04_statistical_data_analysis/determination_of_the_prospective_tariff.ipynb)

## Описание проекта

Федеральный оператор сотовой связи предлагает своим Клиентам два тарифных плана. Для корректировки рекламного бюджета, коммерческому департаменту нужна информация о том, какой тариф приносит больше денег.

## Цель работы

Выполнить предварительный анализ тарифов на небольшой выборке клиентов по данным 500 пользователей за 2018 год. Проанализировать поведение клиентов и сделать вывод — какой тариф лучше.

## Описание данных

**Тариф «Смарт»**
<br>Ежемесячная плата: 550 рублей
<br>Включено 500 минут разговора, 50 сообщений и 15 Гб интернет-трафика
<br>Стоимость услуг сверх тарифного пакета:
<br>минута разговора: 3 рубля
<br>сообщение: 3 рубля
<br>1 Гб интернет-трафика: 200 рублей

**Тариф «Ультра»**
<br>Ежемесячная плата: 1950 рублей
<br>Включено 3000 минут разговора, 1000 сообщений и 30 Гб интернет-трафика
<br>Стоимость услуг сверх тарифного пакета:
<br>минута разговора: 1 рубль
<br>сообщение: 1 рубль
<br>1 Гб интернет-трафика: 150 рублей
<br>Значения минут и мегабайтов округляются в большую сторону.

## Структура проекта

Шаг 1. Изучение файлов с данными. Общая информация
<br>Шаг 2. Подготовка данных
<br>Шаг 3. Анализ данных
<br>3.1  Пользователи тарифного плана "Смарт"
<br>3.2  Пользователи тарифного плана "Ультра"
<br>3.3  Построение гистограмм и описание распределений
<br>Шаг 4. Проверка гипотез
<br>4.1  Cредняя выручка пользователей тарифов «Ультра» и «Смарт» различается
<br>4.2  Cредняя выручка пользователей из Москвы отличается от выручки пользователей из других регионов
<br>Общий вывод

## Используемые библиотеки
`pandas` `matplotlib` `numpy`
