# RentAnalysis_Kaz
Проект представляет собой общий анализ рынка аренды жилья и обзор на рынок г. Алматы и г. Астаны по состоянию на 8 сентября 2024-года. Дополнительно рассматривается ситуация в регионах в разрезе по годам.

[ссылка на дашборд](https://public.tableau.com/app/profile/yersaiyn.yergazy/viz/RentStats_Kaz/sheet10)

### **Общая информация работы:**
В проекте данные будут из двух источников: из `krisha.kz` (для общего анализа текущего рынка) и из Бюро нац. статистики (для статистики прошлых лет). Отдельные благодарности `@andprov` за парсер.

Из `krisha.kz` данные были собраны за 08/09/24, когда "сезон студентов" еще не завершился. Собранные данные помещены в датасет и очищены. Для анализа рынка были учтены только квартиры на долгий срок и три вида квартир: однокомнатные, двухкомнатные и трехкомнатные квартиры соответственно. Больше брать не нужно, разница в ценах может быть существенным.

[Данные из бюро доступны по ссылке](https://stat.gov.kz/ru/industries/economy/prices/spreadsheets/?year=&name=19521&period=&type=).

### **Результаты:**

В результате анализа было выяснено, что в Астане в этот день сдавалось 412 однокомнатных, 748 двухкомнатных и 435 трехкомнатных квартир. А в Алматы сдавалось намного больше: 1109 однокомнатных, 2325 двухкомнатных и 1176 трехномнатных квартир.

Медианная цена для квартиры в Астане - 360 000 тенге, в Алматы - 300 000.

Чем больше комнат, тем меньше цена за кв. метр:
Цена на квадратный метр однокомнатной квартиры в Астане составил 5208 тг., а в Алматы на *28% больше* - 6667 тг. Квадратный метр трехкомнатной в Астане стоил 4396 тг., в Алматы 5608 тг.

В Астане средняя цена для

1-комнатной - ₸200 000.

2-комнатной - ₸300 000

3-комнатной - ₸450 000.

В Алматы средняя цена для

1-комнатной - ₸250 000.

2-комнатной - ₸380 000.

3-комнатной - ₸500 000.

Несмотря на значительный отрыв в количестве квартир в Алматы, там квартиры *дороже в среднем на 20%* чем в Астане. Возможно на цены в Алматы сказывается большое количество студентов в городе.

Для сравнения:
В 2023 году в Астане за квадратный метр просили в среднем 4815 тг., а в г. Алматы - 5549 тг. Это цены в среднем за год, без учета сезонности.


### **А как было в прошлых годах?**

Данные из stat.gov дают шанс взглянуть на состояние рынка с 2001 года по всей Республике:
1. Хаотичное формирование рынка аренды жилья до 2006-года;
2. Кризис 2008-года вероятно повлиял на снижение цены почти во всех городах;
3. Заметное подорожание видно в отрезке 2012-2013 годов - как отражение восстановления рынка после глобального кризиса. [Возврат инвесторского интереса и активизация на рынке жилья сопровождались восстановлением строительства после спада 2009 года.](https://colab.research.google.com/drive/1wQmtgpdE-12ikfFZY-XZr-V1B3cTr2XD#scrollTo=cDz1fjRdKUu7&line=42&uniqifier=1);
4. Снижение цен на сырье на мировых рынках и "отправление в свободное плавание" тенге в 2015 видимо не повлиял на рынок жилья;
5. В "ковидное" время наблюдаем подорожание;
6. А на мобилизацию в РФ в 2022-году рынок ответил резким подорожанием аренды жилья. Событие стало таким значимым, что спустя два года цены не сильно снизились.


### **Future Works:**

1. Автоматизировать парсинг и собирать данные 2 раза в месяц, для информативности

2. Проработка дизайна

3. Можно рассмотреть возможность добавления статистики строительства и ввода в эксплуатацию новых объектов, чтобы оценить, отвечают ли темпы строительства на спрос.
4. Также можно рассмотреть статистику доходов населения для понимания доступности жилья гражданину РК по годам.
