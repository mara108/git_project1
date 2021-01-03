# Приложение для поиска ключевых слов в тексте

Приложение реализует возможность найти ключевые слова в тексте, чтобы быстро понять о чем текст, без прочтения.
Пользователь может:
* скопировать нужный текст (например с веб. страницы) и вставить в окно (вместо текста по умолчанию)
* открыть текстовый файл, введя имя в поле "Имя файла" и нажав кнопку "Вставить текст из файла"
* нужно выбрать язык (русский/английский)
* задать нужное количество ключевых слов (кнопка "Задайте количество слов")
* и, наконец, нажать кнопку "Получить ключевые слова"
В окне в таблицу будут выведены ключевые слова текста, в порядке убывания значимости.
Для акцентирования значимости использована подсветка с убывающим тоном по мере падения значимости.
Одновременно ключевые слова подсветятся и в исходном тексте, чтобы их можно было легко увидеть.

Приложение состоит из двух частей:
- Пользовательский интерфейс (класс MyWidget)
- Алгоритм TextRank (класс TextRank4Keyword)
Задача извлечения ключевых слов заключается в автоматическом извлечении ряда значимых слов или фраз из заданного текста. Алгоритм TextRank заключается в использовании отношения между локальными словами (окно совместного использования) для сортировки последующих ключевых слов, непосредственно извлеченных из самого текста.ect1
