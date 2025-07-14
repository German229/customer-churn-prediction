# Прогнозирование оттока клиентов (Customer Churn Prediction)

Реализация задачи предсказания оттока клиентов телеком-компании с помощью машинного обучения на датасете [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn).

---

## 📋 Описание проекта

В проекте показан полный пайплайн решения задачи бинарной классификации: от загрузки и обработки данных до построения, сравнения и настройки моделей машинного обучения. Используются современные алгоритмы (Logistic Regression, Random Forest, XGBoost, CatBoost), проводится сравнение по ключевым метрикам, выполняется подбор гиперпараметров для улучшения качества.

---

## 📁 Структура проекта

- customer-churn-prediction/
  - files/
    - telco_churn.csv
  - notebooks/
    - customer_churn_analysis.ipynb
    - catboost_info/ (в .gitignore)
  - requirements.txt
  - README.md

---

## 📦 Датасет

- **Источник:** [Kaggle: Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Описание:** Примерно 7000 клиентов телеком-компании, для каждого — демография, информация по услугам, данные о договорах и метка “ушёл/остался”.

---

## 🚀 Быстрый старт

1. **Клонируйте репозиторий**
   ```bash
   git clone https://github.com/yourusername/customer-churn-prediction.git
   cd customer-churn-prediction
Установите зависимости

bash
Копировать
Редактировать
pip install -r requirements.txt
Скачайте датасет

Загрузите с Kaggle

Поместите файл как files/telco_churn.csv

Откройте ноутбук

bash
Копировать
Редактировать
jupyter notebook notebooks/customer_churn_analysis.ipynb
⚙️ Основные этапы
Обработка данных: Заполнение пропусков, преобразование типов, one-hot encoding категориальных признаков, масштабирование числовых фичей.

Анализ данных (EDA): Быстрый обзор распределений, классов и признаков.

Построение моделей: Логистическая регрессия, случайный лес, XGBoost, CatBoost.

Подбор гиперпараметров: GridSearch для CatBoost.

Оценка моделей: Accuracy, Precision, Recall, F1-score, ROC-AUC, матрица ошибок.

Сравнение моделей: Сводная таблица по всем метрикам.

Важность признаков: Анализ наиболее значимых признаков для деревьев.

🏆 Результаты
Лучший ROC-AUC (CatBoost): 0.86+

Accuracy: ~0.81

Лучшие модели: CatBoost (c настройкой параметров), XGBoost

Вывод: CatBoost дал наилучшее качество на этих данных, логистическая регрессия показала максимальный recall, но ниже precision.

Подробности и графики смотри в ноутбуке: notebooks/customer_churn_analysis.ipynb

📌 Требования
Python 3.8+

pandas

numpy

scikit-learn

xgboost

catboost

(matplotlib — для графиков)

Установка зависимостей:

bash
Копировать
Редактировать
pip install -r requirements.txt
🙋‍♂️ Автор
Твоё Имя German229
