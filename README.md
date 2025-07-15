# 🌀 Прогнозирование оттока клиентов (Customer Churn Prediction)

Реализация задачи предсказания оттока клиентов телеком-компании с помощью машинного обучения на датасете [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn).

## 📋 Описание проекта

В проекте показан полный пайплайн решения задачи бинарной классификации: от загрузки и обработки данных до построения, сравнения и настройки моделей машинного обучения. Используются современные алгоритмы (Logistic Regression, Random Forest, XGBoost, CatBoost), проводится сравнение по ключевым метрикам, выполняется подбор гиперпараметров для улучшения качества.

## 📁 Структура проекта

<pre>
customer-churn-prediction/
│
├── files/
│   └── telco_churn.csv
├── notebooks/
│   ├── customer_churn_analysis.ipynb
│   └── catboost_info/ (указано в .gitignore)
├── requirements.txt
├── README.md
</pre>

## 📦 Датасет

- **Источник:** [Kaggle: Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Описание:** Примерно 7000 клиентов телеком-компании, для каждого — демография, информация по услугам, данные о договорах и метка “ушёл/остался”.

## 🚀 Быстрый старт

1. **Клонируйте репозиторий**
   ```bash
   git clone https://github.com/yourusername/customer-churn-prediction.git
   cd customer-churn-prediction
   ```

2. **Установите зависимости**
   ```bash
   pip install -r requirements.txt
   ```

3. **Скачайте датасет**
   - [Загрузите с Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
   - Поместите файл в папку: `files/telco_churn.csv`

4. **Откройте ноутбук**
   ```bash
   jupyter notebook notebooks/customer_churn_analysis.ipynb
   ```

## ⚙️ Основные этапы

- Обработка данных: заполнение пропусков, преобразование типов, one-hot encoding категориальных признаков, масштабирование числовых фичей.
- Анализ данных (EDA): быстрый обзор распределений, классов и признаков.
- Построение моделей: логистическая регрессия, случайный лес, XGBoost, CatBoost.
- Подбор гиперпараметров: GridSearch для CatBoost.
- Оценка моделей: Accuracy, Precision, Recall, F1-score, ROC-AUC, матрица ошибок.
- Сравнение моделей: сводная таблица по всем метрикам.
- Важность признаков: анализ наиболее значимых признаков для деревьев.

## 🏆 Результаты

- **Лучший ROC-AUC (CatBoost):** 0.86+
- **Accuracy:** ~0.81
- **Лучшие модели:** CatBoost (c настройкой параметров), XGBoost
- **Вывод:** CatBoost дал наилучшее качество на этих данных, логистическая регрессия показала максимальный recall, но ниже precision.

Подробнее — смотри ноутбук: `notebooks/customer_churn_analysis.ipynb`

## 📌 Требования

- Python 3.8+
- pandas
- numpy
- scikit-learn
- xgboost
- catboost

**Установка зависимостей:**
```bash
pip install -r requirements.txt
```

## 🙋‍♂️ Автор

- [German229](https://github.com/German229)
