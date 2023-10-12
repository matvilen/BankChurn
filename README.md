# Расчет клиентской убыли банка

Часть программной подсистемы расчета клиентской убыли, представленная в виде нескольких Юпитер-ноутбуков. На вход подаются характеристики клиентов банка, далее эти данные обрабатываются определенным образом (с помощью моделей машинного обучения и нейронных сетей) и на выходе мы получаем новые данные с указанием вероятности ухода клиентов. Помимо функций предсказания, реализована возможность отслеживания корректности работы моделей по предсказанию ухода клиентов.

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://nbviewer.org/github/matvilen/BankChurn/blob/main/bank_churn_notebook.ipynb">
    <img src="images/churn_logo.png" alt="Logo" width="180" height="180">
  </a>
 <style>
a:link {
  background-color: yellow;
}

a:visited {
  background-color: cyan;
}

a:hover {
  background-color: lightgreen;
}

a:active {
  background-color: hotpink;
} 
</style> 
<p><a href="https://mozilla.org">A link to the Mozilla homepage</a></p>
  ## [Просмотр Юпитер-ноутбука через nbviewer](https://nbviewer.org/github/matvilen/BankChurn/blob/main/bank_churn_notebook.ipynb)

  <div align="center">Весь проект в одном файле с интерактивным содержанием</div>
  
  <p align="center">
    <br />
    <a href="https://github.com/matvilen/BankChurn/tree/main/docs"><strong>Изучить графические материалы проекта »</strong></a>
    <br />
  </p>
</div>

## Содержание

- [Предварительная обработка данных](https://github.com/matvilen/BankChurn/blob/main/bank_churn_notebook.ipynb)
    - Слияние датасетов
    - Трансформация категориальных переменных
    - Отсечение линейнозависимых признаков
    - Обработка пропущенных значений
    - Нормализация данных
    - Удаление выбросов
    - Разбиение выборки на обучающую, тестовую и валидационную
- [Построение моделей машинного обучения](docs/A1_DA.md)
    - XGB booster
    - LGBM booster
    - XGB forest
    - LogRegression
    - Построение графика AUC-кривой
- [Построение нейронных сетей](https://github.com/matvilen/BankChurn/blob/main/bank_churn_notebook.ipynb)
    - Построение сетей с использованием Sigmoid, Relu и различного количества слоев и нейронов в них
    - Построение графиков LOSS, AUC и ACCURACY кривых для выбора наилучшей модели сети
- [Калибровка полученных моделей](https://github.com/matvilen/BankChurn/blob/main/bank_churn_notebook.ipynb)
    - Калибровка моделей методом Плата
    - Калибровка моделей Калибровка с применением стратифицированной кросс-валидации
    - Построение кривых надежности для неоткалиброванных и откалиброванных моделей
- [Результаты работы моделей](docs/A2_MS.md)
    - Построение графика значимости характеристик (метод Light GBM) 
    - Построение графиков зависимости предсказания модели от значений признаков
    - Вывод результатов в виде таблиц
- [Разработка технологии мониторинга](https://github.com/matvilen/BankChurn/blob/main/bank_churn_notebook.ipynb)
    - Искусственное создание ситуации постепенного ухудшения показателей модели
    - Построение графика мониторинга модели

  
- [Просмотр всего проекта через nbviewer](https://nbviewer.org/github/matvilen/BankChurn/blob/main/bank_churn_notebook.ipynb)



Е.К. Матвиенко (metell-98@mail.ru)
