https://education.yandex.ru/handbook/ml/article/about

# Типы задач машинного обучения

Все задачи, решаемые с помощью ML, относятся к одной из следующих категорий.

1)Задача регрессии – прогноз на основе выборки объектов с различными признаками. На выходе должно получиться вещественное число (2, 35, 76.454 и др.), к примеру цена квартиры, стоимость ценной бумаги по прошествии полугода, ожидаемый доход магазина на следующий месяц, качество вина при слепом тестировании.

2)Задача классификации – получение категориального ответа на основе набора признаков. Имеет конечное количество ответов (как правило, в формате «да» или «нет»): есть ли на фотографии кот, является ли изображение человеческим лицом, болен ли пациент раком.

3)Задача кластеризации – распределение данных на группы: разделение всех клиентов мобильного оператора по уровню платёжеспособности, отнесение космических объектов к той или иной категории (планета, звёзда, чёрная дыра и т. п.).

4)Задача уменьшения размерности – сведение большого числа признаков к меньшему (обычно 2–3) для удобства их последующей визуализации (например, сжатие данных).

5)Задача выявления аномалий – отделение аномалий от стандартных случаев. На первый взгляд она совпадает с задачей классификации, но есть одно существенное отличие: аномалии – явление редкое, и обучающих примеров, на которых можно натаскать машинно обучающуюся модель на выявление таких объектов, либо исчезающе мало, либо просто нет, поэтому методы классификации здесь не работают. На практике такой задачей является, например, выявление мошеннических действий с банковскими картами.

https://habr.com/ru/articles/448892/

# Краткий обзор основных алгоритмов машинного обучения:

1. **Линейная регрессия (Linear Regression)**:
   - Используется для предсказания непрерывной целевой переменной на основе линейной комбинации признаков.
   - Оценивает веса признаков с помощью метода наименьших квадратов или других оптимизационных методов.

2. **Логистическая регрессия (Logistic Regression)**:
   - Применяется для задач бинарной классификации, где целевая переменная принимает два возможных значения.
   - Основана на логистической функции для моделирования вероятности принадлежности к классу.

3. **Метод ближайших соседей (K-Nearest Neighbors)**:
   - Классификационный алгоритм, основанный на принципе большинства голосов среди k ближайших соседей.
   - Использует расстояние между объектами в пространстве признаков для определения ближайших соседей.

4. **Деревья решений (Decision Trees)**:
   - Позволяют разбить пространство признаков на более простые области с помощью серии вопросов.
   - Могут использоваться для задач классификации и регрессии.

5. **Случайный лес (Random Forest)**:
   - Ансамблевый метод, состоящий из множества деревьев решений.
   - Каждое дерево строится на подвыборке данных и подмножестве признаков для уменьшения переобучения и повышения обобщающей способности.

6. **Метод опорных векторов (Support Vector Machines, SVM)**:
   - Используется для задач классификации и регрессии.
   - Находит оптимальную гиперплоскость, разделяющую классы, максимизируя расстояние между классами.

7. **Кластеризация K-средних (K-Means Clustering)**:
   - Неразмеченный метод кластеризации, целью которого является разбиение набора данных на заранее определенное число кластеров.
   - Минимизирует среднеквадратичное отклонение от центров кластеров.

8. **PCA (Principal Component Analysis)**:
   - Метод снижения размерности данных.
   - Используется для уменьшения количества признаков путем проецирования данных на новое пространство признаков, сохраняющее максимальную дисперсию.

Это лишь краткий обзор некоторых основных алгоритмов машинного обучения. В зависимости от конкретной задачи и данных, может потребоваться использование комбинации различных алгоритмов или их модификаций.

# Ещё несколько основных алгоритмов машинного обучения:

9. **Наивный Байесовский классификатор (Naive Bayes Classifier)**:
   - Базируется на теореме Байеса и предполагает независимость признаков.
   - Часто используется для задач классификации текстовых данных, таких как анализ тональности текста или спам-фильтрация.

10. **Метод главных компонент (Principal Component Regression, PCR)**:
    - Метод регрессии, основанный на снижении размерности признаков с помощью метода главных компонент (PCA).
    - Используется для уменьшения мультиколлинеарности в данных и улучшения обобщающей способности модели.

11. **Метод главных компонент и регрессии (Partial Least Squares Regression, PLSR)**:
    - Метод регрессии, который комбинирует метод главных компонент и линейную регрессию.
    - Позволяет учитывать не только структуру признаков, но и связь с целевой переменной при снижении размерности данных.

12. **Методы кластеризации на основе плотности (Density-Based Clustering)**:
    - Кластерные алгоритмы, которые определяют кластеры, исходя из плотности распределения данных.
    - Примеры включают DBSCAN (Density-Based Spatial Clustering of Applications with Noise) и OPTICS (Ordering Points To Identify the Clustering Structure).

13. **Градиентный спуск (Gradient Descent)**:
    - Основной метод оптимизации, используемый для обучения моделей машинного обучения.
    - Минимизирует функцию потерь, обновляя параметры модели в направлении наибольшего убывания градиента.

14. **Методы оптимизации для глубокого обучения (Optimization Methods for Deep Learning)**:
    - Включают в себя методы стохастического градиентного спуска (SGD), Adam, RMSprop и другие.
    - Применяются для обучения нейронных сетей и оптимизации их параметров.

15. **Сверточные нейронные сети (Convolutional Neural Networks, CNN)**:
    - Специализированные архитектуры нейронных сетей для анализа изображений и видео.
    - Используются для задач классификации, детекции объектов, сегментации изображений и др.

Это ещё не весь список, но эти алгоритмы представляют собой важные инструменты в арсенале машинного обучения.


# Линейная регрессия

https://proglib.io/p/linear-regression

Линейная регрессия - это один из наиболее простых и широко используемых методов в машинном обучении для моделирования зависимости между одной или несколькими независимыми переменными (признаками) и зависимой переменной (целевой переменной), которая представляет собой непрерывное значение.

Вот основные аспекты линейной регрессии:

1. **Модель**: Линейная модель представляет собой линейную комбинацию входных признаков с весами (коэффициентами), добавленными смещением (интерсептом):
   \[ y = w_0 + w_1 * x_1 + w_2 * x_2 + ... + w_n * x_n \]
   Где \( y \) - целевая переменная, \( x_1, x_2, ..., x_n \) - независимые переменные, \( w_0, w_1, w_2, ..., w_n \) - параметры модели.

2. **Оценка параметров**: Целью линейной регрессии является нахождение оптимальных значений параметров \( w_0, w_1, w_2, ..., w_n \), которые минимизируют сумму квадратов ошибок между фактическими и предсказанными значениями целевой переменной. Этот процесс называется обучением модели.

3. **Функция потерь**: Чаще всего в линейной регрессии используется среднеквадратичная ошибка (Mean Squared Error, MSE) в качестве функции потерь:
   \[ MSE = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y_i})^2 \]
   Где \( y_i \) - фактическое значение целевой переменной, \( \hat{y_i} \) - предсказанное значение целевой переменной, \( n \) - количество наблюдений.

4. **Методы оптимизации**: Для нахождения оптимальных параметров модели часто используется метод градиентного спуска или его вариации, которые итеративно обновляют значения параметров, исходя из градиента функции потерь.

5. **Оценка качества модели**: После обучения модели оценивают её качество на отложенной выборке или с помощью кросс-валидации. Распространенными метриками оценки качества включаются коэффициент детерминации (R-squared), средняя абсолютная ошибка (MAE) и другие.

Линейная регрессия широко используется в реальных приложениях, таких как прогнозирование цен на недвижимость, анализ финансовых данных, медицинские исследования и другие области. Важно помнить, что линейная регрессия предполагает линейную зависимость между признаками и целевой переменной, и её результаты могут быть недостаточно точными, если эта зависимость нелинейна.

Давайте проведем практическое задание по изучению линейной регрессии на примере набора данных о жилищных ценах в Бостоне. Этот датасет часто используется для начального обучения машинного обучения и содержит информацию о жилищных ценах в разных районах Бостона, а также различные атрибуты, такие как среднее количество комнат в доме, уровень преступности и другие.

### Задание

1. **Цель задания**: Используя линейную регрессию, постройте модель, предсказывающую медианную стоимость домов (целевая переменная `MEDV`) на основе выбранных признаков.

2. **Шаги выполнения**:
   - Загрузите датасет о жилищных ценах в Бостоне. Описание датасета и сам датасет можно найти в репозиториях с открытыми данными или встроить его непосредственно из библиотеки `scikit-learn`.
   - Проведите первичный анализ данных: изучите распределение целевой переменной, проверьте наличие пропущенных значений, оцените корреляцию между признаками.
   - Выберите один или несколько признаков для построения модели линейной регрессии. Обоснуйте свой выбор.
   - Разделите датасет на обучающую и тестовую выборки.
   - Обучите модель линейной регрессии на обучающей выборке.
   - Оцените качество модели на тестовой выборке, используя метрики MAE (средняя абсолютная ошибка) и MSE (среднеквадратичная ошибка).
   - Проанализируйте полученные результаты: какие признаки наиболее важны для модели, удовлетворительно ли качество предсказания?

### Ресурсы для выполнения задания

- Для загрузки датасета из `scikit-learn` используйте следующий код:
  ```python
  from sklearn.datasets import load_boston
  boston = load_boston()
  X, y = boston.data, boston.target
  ```
  Обратите внимание, что использование этого датасета напрямую из `scikit-learn` может быть устаревшим в новых версиях библиотеки. В таком случае, датасет доступен на множестве открытых платформ для работы с данными.

- Описание датасета доступно в документации `scikit-learn` или на сайтах с открытыми данными.

### Подсказки

- Важно не только обучить модель, но и правильно обработать данные перед обучением: проверить на наличие пропусков, нормализовать данные, если это необходимо.
- Использование кросс-валидации поможет лучше оценить качество модели на различных подвыборках данных.
- Построение графиков может помочь в анализе данных и в интерпретации результатов моделирования.

Это задание даст вам представление о том, как работать с реальными данными, применять линейную регрессию и интерпретировать результаты моделирования.

# Логистическая регрессия
 — это статистический метод для анализа набора данных, в котором одна или несколько независимых переменных определяют исход. В отличие от линейной регрессии, которая предсказывает непрерывное значение (например, цену на дом), логистическая регрессия используется для бинарной классификации (например, спам/не спам, болен/здоров).

 https://habr.com/ru/companies/skillfactory/articles/714244/

Основное отличие логистической регрессии от линейной заключается в том, что она использует логистическую функцию (также известную как сигмоид) для ограничения выходного значения в диапазоне между 0 и 1. Это делает ее особенно подходящей для задач, где необходимо предсказать вероятность принадлежности к определенному классу.

### Основные аспекты логистической регрессии:

- **Сигмоидная функция**: Основной элемент логистической регрессии, преобразующий линейное уравнение \(\ln(\frac{p}{1-p}) = b_0 + b_1x_1 + ... + b_nx_n\) в вероятность \(p\), где \(p\) – вероятность принадлежности к классу 1. Сигмоидная функция выглядит как S-образная кривая, и ее формула: \(p = \frac{1}{1 + e^{-(b_0 + b_1x_1 + ... + b_nx_n)}}\).

- **Оценка модели**: Для оценки качества модели логистической регрессии часто используют такие метрики, как точность (accuracy), ROC AUC, логарифмическая потеря (log loss), точность (precision), полнота (recall) и F1-мера.

- **Регуляризация**: Для предотвращения переобучения модели логистической регрессии могут применяться методы регуляризации, такие как L1 (лассо) и L2 (ридж), которые добавляют штраф к величине коэффициентов.

- **Многоклассовая классификация**: Хотя логистическая регрессия в первую очередь предназначена для бинарной классификации, ее можно расширить на многоклассовую классификацию с использованием таких подходов, как метод «один против всех» (OvA) или «один против одного» (OvO).

- **Применение**: Логистическая регрессия широко применяется в медицине (для диагностики заболеваний), в финансах (для оценки кредитоспособности), в маркетинге (для прогнозирования оттока клиентов), в социальных науках и многих других областях.

Логистическая регрессия является мощным и гибким инструментом, чья простота и интерпретируемость делают ее одним из популярных выборов для задач классификации.

Конечно! Вот задание для изучения логистической регрессии:

### Задание: Прогнозирование вероятности диабета у пациентов

**Описание:**
Вы работаете в медицинской клинике и вам предоставлен набор данных о пациентах, включающий информацию о различных медицинских параметрах и наличии или отсутствии диабета. Ваша задача - построить модель логистической регрессии для прогнозирования вероятности наличия диабета у пациентов.

**Шаги:**

1. **Импорт данных**: Загрузите данные в DataFrame (например, из CSV-файла).

2. **Исследование данных**: Изучите данные, чтобы понять их структуру, типы признаков, наличие пропущенных значений и т. д.

3. **Подготовка данных**: Проведите необходимую предобработку данных, включая заполнение пропущенных значений, кодирование категориальных признаков и масштабирование признаков.

4. **Разделение данных**: Разделите данные на обучающую и тестовую выборки.

5. **Обучение модели**: Обучите модель логистической регрессии на обучающих данных.

6. **Оценка модели**: Оцените производительность модели на тестовых данных, используя метрики классификации, такие как точность, полнота, F1-мера и ROC AUC.

7. **Интерпретация результатов**: Проанализируйте коэффициенты модели, чтобы понять, какие медицинские параметры оказывают наибольшее влияние на вероятность наличия диабета.

**Дополнительные задачи:**

- Попробуйте улучшить модель, используя методы выбора признаков, регуляризацию или инженерию признаков.
- Исследуйте важность признаков и попробуйте объяснить, какие медицинские параметры оказывают наибольшее влияние на вероятность наличия диабета.

Чтобы выполнить это задание, вам понадобится набор данных. Вы можете скачать набор данных о диабете по следующей ссылке: [Diabetes Dataset (Kaggle)](https://www.kaggle.com/datasets/mathchi/diabetes-data-set).

В наборе данных о диабете содержатся различные медицинские параметры, а также информация о наличии или отсутствии диабета у пациентов. Вот описание столбцов в этом наборе данных:

    Признаки:
        Pregnancies: Количество беременностей.
        Glucose: Концентрация глюкозы в плазме через 2 часа после теста на глюкозу.
        BloodPressure: Артериальное давление (мм рт. ст.).
        SkinThickness: Толщина кожной складки (мм).
        Insulin: Концентрация инсулина в сыворотке крови (мкЕд/мл).
        BMI: Индекс массы тела (вес в кг / (рост в м)^2).
        DiabetesPedigreeFunction: Показатель наследственного предрасположения к диабету.
        Age: Возраст (лет).

    Целевая переменная:
        Outcome: Наличие диабета у пациента (0 - нет диабета, 1 - есть диабет).

Каждая строка в наборе данных представляет собой данные о конкретном пациенте, включая значения указанных медицинских параметров и наличие или отсутствие диабета. Этот набор данных часто используется для задач классификации с использованием моделей машинного обучения, таких как логистическая регрессия.
