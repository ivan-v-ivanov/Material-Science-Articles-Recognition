# Material-Science-Articles-Recognition

В проекте реализован алгоритм обучения модели, распознающей статьи журналов $Nature$ $Materials$ ($Q1$) и $Materials$ $Express$ ($Q4$) по их $abstract$.

На первом этапе проводился $scraping$ данных с использованием [двух скриптов](https://github.com/ivan-v-ivanov/Material-Science-Articles-Recognition/blob/main/data-scraping).

В дальнейшем текст подвергался очистке от символов, лемматизации. 
Классификация осуществлялась с использованием $XGBoostClassifier$. Используемая метрика для оптимизации параметров: $f1-score$ ([ссылка](https://github.com/ivan-v-ivanov/Material-Science-Articles-Recognition/blob/main/app/model/articles_recognition_model.ipynb)).

В дополнение реализованы клиентская и серверная части клиентов по доступу к модели с использованием $flask$ ([ссылка](https://github.com/ivan-v-ivanov/Material-Science-Articles-Recognition/tree/main/app)).
