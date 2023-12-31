# Расчет клиентской убыли банка

Часть программной подсистемы расчета клиентской убыли, представленная в виде нескольких Юпитер-ноутбуков. На вход подаются характеристики клиентов банка, далее эти данные обрабатываются определенным образом (с помощью моделей машинного обучения и нейронных сетей) и на выходе мы получаем новые данные с указанием вероятности ухода клиентов. Помимо функций предсказания, реализована возможность отслеживания корректности работы моделей по предсказанию ухода клиентов.

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://nbviewer.org/github/matvilen/BankChurn/blob/main/bank_churn_notebook.ipynb">
    <img src="images/churn_logo.png" alt="Logo">
  </a>
  
  ## [Просмотр Юпитер-ноутбука через nbviewer](https://nbviewer.org/github/matvilen/BankChurn/blob/main/bank_churn_notebook.ipynb)
  <div align="center">Весь проект в одном файле с интерактивным оглавлением</div>
  
  <p align="center">
    <br />
    <a href="https://github.com/matvilen/BankChurn/tree/main/docs"><strong>Изучить графические материалы проекта »</strong></a>
    <br />
  </p>
</div>

## Содержание

- [Предварительная обработка данных](https://github.com/matvilen/BankChurn/blob/main/1_data_preprocessing.ipynb)
    - Слияние датасетов
    - Трансформация категориальных переменных
    - Отсечение линейнозависимых признаков
    - Обработка пропущенных значений
    - Нормализация данных
    - Удаление выбросов
    - Разбиение выборки на обучающую, тестовую и валидационную
- [Построение моделей машинного обучения](https://github.com/matvilen/BankChurn/blob/main/2_building_ml_models.ipynb)
    - XGB booster
    - LGBM booster
    - XGB forest
    - LogRegression
    - Построение графика AUC-кривой
- [Построение нейронных сетей](https://github.com/matvilen/BankChurn/blob/main/3_construction_of_neural_networks.ipynb)
    - Построение сетей с использованием Sigmoid, Relu и различного количества слоев и нейронов в них
    - Построение графиков LOSS, AUC и ACCURACY кривых для выбора наилучшей модели сети
- [Калибровка полученных моделей](https://github.com/matvilen/BankChurn/blob/main/4_calibration_of_models.ipynb)
    - Калибровка моделей методом Плата
    - Построение кривых надежности для неоткалиброванных и откалиброванных моделей
    - Калибровка классических моделей с применением стратифицированной кросс-валидации
- [Результаты работы моделей](https://github.com/matvilen/BankChurn/blob/main/5_results.ipynb)
    - Построение AUC-кривых для всех моделей
    - Построение графика значимости характеристик (метод Light GBM) 
    - Вывод полученных метрик
- [Разработка технологии мониторинга](https://github.com/matvilen/BankChurn/blob/main/6_monitoring.ipynb)
    - Искусственное создание ситуации постепенного ухудшения показателей модели
    - Построение графика мониторинга модели

  




Е.К. Матвиенко (metell-98@mail.ru)
