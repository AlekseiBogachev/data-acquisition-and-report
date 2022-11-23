# data-acquisition-and-report
Пример собранных и обработанных экспериментальных данных с отчётом. 
Результат обработки сырых данных с измерительной установки пакетом [pydlts](https://github.com/AlekseiBogachev/pydlts).

## Структура репозитория
- **py** - Папка с ноутбуками из которых запускалась пакетная обработка данных и ноутбуком, в котором построены дополнительные графики для отчёта.
- **raw_data** - Сырые данные, полученные с измерительной установки.
- **datasets** - Результаты измерений в удобном для обработки виде (сырые данные из папки raw_data, прошедшие обработку 
  с помощью объекта `BatchDataReaderDLS82E` из модуля `pydlts.misc`).
- **models** - Данные с добавленными результатами моделирования и идентификации. Результат обработки содержимого папки
  datasets с помощью моноэкспоненциальной модели с показателем нелинейности-неэкспоненциальности (объект `SklSingleExpFrequencyScan` из модуля `pydlts.fsmodels`).
- **plots** - Сгенерированные графики
- **Отчёт** - Проект отчёта в LaTex.
    - **main.pdf** - [Отчёт в формате pdf](https://github.com/AlekseiBogachev/data-acquisition-and-report/blob/main/%D0%9E%D1%82%D1%87%D1%91%D1%82/main.pdf).
- **Рабочий_журнал** - Папка с рабочим журналом измерений.
