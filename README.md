# Проект: Предподготовка данных для постоения модели для автоматической оценки уровня зарплаты на основании резюме
## ***Описание проекта***
Этот проект посвящён предобработке данных для дальнейшей разработки модели машинного обучения, предназначенной для автоматической оценки примерного уровня заработной платы на основе информации, указанной в резюме соискателей. В рамках проекта будет использоваться база данных резюме, выгруженная с сайта поиска вакансий hh.ru.
#### Проблематика
Многие соискатели не указывают желаемую заработную плату в своих резюме, что создаёт трудности для рекрутеров и работодателей в оценке реальной стоимости кандидата. Чтобы устранить эту проблему и улучшить процесс подбора персонала, компания HeadHunter стремится построить модель, которая сможет автоматически прогнозировать заработную плату, основываясь на данных, предоставленных соискателем в резюме.
## ***Структура проекта***

- [Project.ipunb](https://github.com/Dashaklen/HHproject/blob/master/Project.ipynb): Jupyter ноутбук с анализом данных и построением графиков.
- [Графики](https://github.com/Dashaklen/HHproject/tree/master/%D0%93%D1%80%D0%B0%D1%84%D0%B8%D0%BA%D0%B8): Папка с графиками
- [reqirements.txt](https://github.com/Dashaklen/HHproject/blob/master/requirements.txt): Зависимости
- [README.md](https://github.com/Dashaklen/Customer_churn_analysis_bank/blob/main/README.md): Описание проекта.'
- Данные, использованные в проекте можно скачать по ссылкам:
[ExchangeRates.csv](https://drive.google.com/file/d/1dd-ZY8YzLEPfJDi0Y8FdM7MULMYFagvW/view?usp=drive_link)
[hh_database.csv](https://drive.google.com/file/d/1E8Bd4E7gVdkrFmBH20rbVgS9-l31VCFq/view?usp=drive_link)
## Используемые библиотеки

В проекте использованы следующие библиотеки:

- pandas для обработки данных
- matplotlib, plotly и seaborn для построения графиков
- Другие необходимые библиотеки, указанные в файле requirements.txt

## Этапы анализа

1. Загрузка и предобработка данных:
   * Загрузка данных из файла.
   * Преобразование данных в удобный для анализа формат.
   * Очистка данных, обработка пропусков и выбросов.

3. Анализ данных:
   * Исследование распределений и взаимосвязей между различными признаками резюме и уровнем заработной платы.
   * Выявление ключевых факторов, влияющих на заработную плату.

4. Выводы и рекомендации:
   - Анализ результатов.
   - Формулирование выводов.

## Графики и визуализации

В проекте построены различные графики, которые наглядно демонстрируют взаимосвязи между переменными и ключевыми факторами. Некоторые из них:

[Гистограмма распределения возраста](https://github.com/Dashaklen/HHproject/blob/master/%D0%93%D1%80%D0%B0%D1%84%D0%B8%D0%BA%D0%B8/age_distribution.png)

[Гистограмма распределения ожидаемой заработной платы](https://github.com/Dashaklen/HHproject/blob/master/%D0%93%D1%80%D0%B0%D1%84%D0%B8%D0%BA%D0%B8/distribution_of_expected_salary.png)

[Распределение медианной зарплаты в зависимости от уровня образования](https://github.com/Dashaklen/HHproject/blob/master/%D0%93%D1%80%D0%B0%D1%84%D0%B8%D0%BA%D0%B8/median_salary_by_level_of_education.png)

[Зависимость опыта работы от возраста соискателя](https://github.com/Dashaklen/HHproject/blob/master/%D0%93%D1%80%D0%B0%D1%84%D0%B8%D0%BA%D0%B8/the_dependence_of_work_experience_on_age.png)
## Заключительные Выводы:
1. Возраст и Заработная Плата:

   * Растущий Уровень Заработной Платы с Возрастом: Соискатели с высшим образованием демонстрируют значительный рост заработной платы с возрастом, достигая пика к 50-60 годам. В младшем возрасте заработная плата ниже, но с возрастом растет значительно. Для людей с неполным высшим и средним образованием зависимость заработной платы от возраста менее выражена.
   * Аномалии в Возрасте: Возрастные значения, превышающие 65 лет, могут быть выбросами, так как в этом возрасте работа может быть физически трудной. Значение в 100 лет явно указывает на ошибку ввода данных.
2. Образование и Заработная Плата:

   * Высшее Образование: Соискатели с высшим образованием получают наивысшие зарплаты в любой возрастной группе, что указывает на высокий уровень профессиональной квалификации и, вероятно, на соответствующие рабочие позиции.
   * Среднее и Неполное Высшее Образование: Зарплаты у лиц с неполным высшим образованием и средним образованием значительно ниже, и разница заметна даже в молодом возрасте.
3. Географический Фактор:

   * Большие Города: Уровень ожидаемой зарплаты выше в крупных городах, особенно в Москве. Это связано с более высокими затратами на жизнь и более высокими требованиями к зарплатам в столицах.

4. Фактор Готовности к Переезду и Командировкам:
   * Среди соискателей, которые готовы к командировкам и тех, кто готов к переезду, нет различий в уровне ожидаемой зарплаты. Однако уровень ожидаемой зарплаты у тех, кто готов к командировкам и переезду, выше, чем у тех, кто не готов к этим условиям. При этом соискатели, не готовые к переезду, ожидают более высокую зарплату по сравнению с теми, кто не готов к командировкам.
5. Пол соискателя и уровень заработной платы:
   * У мужчин уровень заработной платы выше, чем у женщин.
6. График работы/занятость и заработанная плата:
   * Самый высокий уровень ожидаемой медианной зарплаты у соискателей, которые ищут работу на условиях полной занятости и проектной работы. Самые низкие требования к ЗП у тех, кто ищет стажировку.
Среди графиков работы самые высокие уровни ожидаемой зарплаты наблюдаются у сосикателей, которые ищут работу на полный день или удаленную работу.
## Установка и использование

1. Клонируйте репозиторий:
   git clone [https://github.com/Dashaklen/Customer_churn_analysis_bank.git](https://github.com/Dashaklen/HHproject)
2. Скачайте базы данных и добавьте их в папку проекта:
[ExchangeRates.csv](https://drive.google.com/file/d/1dd-ZY8YzLEPfJDi0Y8FdM7MULMYFagvW/view?usp=drive_link)
[hh_database.csv](https://drive.google.com/file/d/1E8Bd4E7gVdkrFmBH20rbVgS9-l31VCFq/view?usp=drive_link)
4. Установить необходимые библиотеки:
   pip install -r requirements.txt
5. Запустить Jupyter notebook для просмотра и запуска анализа.
