# Material-Science-Articles-Recognition

В проекте реализован алгоритм обучения модели, распознающей статьи журналов _Nature Materials (Q1)_ и _Materials Express (Q4)_ по их __abstract__.

На первом этапе проводился __scraping__ данных с сайтов [_Nature Materials_](https://www.nature.com/nmat/research-articles) и [_Materials Express_](https://www.ingentaconnect.com/content/asp/me;jsessionid=2b52psp1jbwd8.x-ic-live-03).

В дальнейшем текст подвергался очистке от символов, лемматизации и преобразованию ***TF-IDF***. 
Классификация осуществлялась с использованием ***XGBoostClassifier***. Используемая метрика для оптимизации параметров: ***f1-score***.

В дополнение реализованы клиентская и серверная части для доступа к модели с использованием ***flask***.
