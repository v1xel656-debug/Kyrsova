# Аналіз структури та динаміки онлайн-замовлень

Курсова робота з дисципліни **«Мови програмування для аналізу даних»**  
Національний університет «Полтавська політехніка імені Юрія Кондратюка»  
Спеціальність: 122 «Комп'ютерні науки»

## Мета проєкту
Дослідження структури, часової динаміки, регіонального розподілу та логістичних показників онлайн-замовлень в електронній комерції засобами Python (Pandas, NumPy, Matplotlib, Seaborn) та створення інтерактивного дашборда в Tableau Public.

## Інтерактивний дашборд (Tableau Public)
Переглянути інтерактивну аналітичну панель можна за посиланням:  
[Відкрити дашборд у Tableau Public](https://public.tableau.com/app/profile/roman.katsai/viz/OnlineOrdersAnalysisCoursework/Dashboard1#1)

## Опис набору даних та джерело
Для аналізу використано відкритий реляційний набір даних **Brazilian E-Commerce Public Dataset by Olist**, що містить інформацію про ~100 000 реальних замовлень за 2016–2018 роки.
- **Джерело даних:** [Kaggle — Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
- **Використані таблиці:**
  1. `olist_orders_dataset.csv` — статуси та часові мітки виконання замовлень;
  2. `olist_order_items_dataset.csv` — товарні позиції, ціни та вартість доставки;
  3. `olist_products_dataset.csv` — категорії та фізичні характеристики товарів;
  4. `olist_customers_dataset.csv` — географія покупців (міста та штати);
  5. `product_category_name_translation.csv` — переклад назв категорій англійською мовою.

## Використані технології
- **Python 3**
- **Pandas, NumPy** — очищення, об'єднання таблиць, створення ознак та статистичний аналіз
- **Matplotlib, Seaborn** — статична візуалізація даних
- **Google Colab / Jupyter Notebook** — інтерактивне середовище розробки
- **Tableau Public** — побудова інтерактивної аналітичної панелі

## Структура репозиторію
- `notebooks/analysis.ipynb` — основний ноутбук із повним циклом завантаження, очищення, аналізу та візуалізації даних.
- `results/figures/` — згенеровані графіки у високій роздільній здатності (PNG).
- `requirements.txt` — перелік необхідних бібліотек Python.

## Інструкція із запуску
1. Завантажте вихідні CSV-файли набору даних із [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).
2. Встановіть необхідні бібліотеки командою:
   ```bash
   pip install -r requirements.txt
