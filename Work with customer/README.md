В данном директории собраны файлы по проекту "Wine Quality".

Цель проекта:
Предсказать экспертную оценку качества вина, используя данные его физико-химического состава.

Установка:
Для выполнения проекта необходимо установить все пакеты из файла requirements.txt

Краткое описание проекта:
Работа включала несколько этапов:

- на этапе исследовательского анализа были установлены зависимости между целевой переменной и признаками; построена тепловая карта корреляции; выявлен дисбаланс классов в целевой переменной.

- на этапе подготовки данных произведена их предобработка: заполнены пропуски; перекодированы категориальные переменные; определена важность признаков для обучения модели; произведена работа по увеличению выборки в целях борьбы с дисбалансом классов.

- на этапе моделирования произведено обучение моделей, рассчитана скорость их обучения, время предсказания, а также оценка качества модели посредством расчёта score; определена модель, показавшая наилучший score; произведен перебор гиперпараметров.

- на этапе оценки качества работы модели осуществлено предсказание для тестовой выборки; вычислен score; построена матрица ошибок.

- на этапе развертывания произведено сохранение результатов предсказания в файл формата .csv

Вывод по работе:
Более высокое качество показала модель RandomForestClassifier, которая в более чем 84,6% случаев успешно предсказала экспертную оценку качества вина.  
Матрица ошибок показала, что модель предсказывает лучше всего классы 3, 8, 9 и 4. Вероятно, их признаки действительно лучше выражены и модель лучше обучилась на них.
В перспективе планируется обучение бустинговых моделей.
