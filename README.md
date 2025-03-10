Проєкт на тему

                     "Аналіз впливу первинних джерел енергії на викиди CO2 та порівняння енергоефективності економіки України та світу."

Для проє'кту були використані наступні дані:
https://www.kaggle.com/datasets/lobosi/c02-emission-by-countrys-grouth-and-population/data

Він містить перелік важливих факторів, які впливають на викиди C02, включаючи виробництво та споживання кожного типу основного джерела енергії для кожної країни та її щорічний рейтинг забруднення.Також включає ВВП кожної країни, кількість населення, енергоємність на душу населення (особу) та енергоємність на одиницю ВВП. 
Джерело походження даних -  US Energy Information Administration 
https://www.eia.gov/international/data/world

 МЕТА ПРОЄКТУ :
•	оцінка впливу споживання різних типів первинних джерел енергії на рівень викидів СО2 та визначення частки відновлювальних джерел у 
  загальній структурі та визначити тенденції їх використання;
•	аналіз енергоефективності економіки України у порівнянні з економікою світу через показники енергоємності на душу населення та енергоємності на одиницю ВВП;
•	прогноз рівня викидів СO2, на основі показника, що найсильніше з ним корелює - споживання енергії.

 ОСНОВНІ ЕТАПМ ТА МЕТОДИ АНАЛІЗУ :
 
1. EXCEL:
  
Первинний аналіз даних за допомогою PIVOT TABLES та CONDITIONAL FORMATTING
•	Аналіз статистичних показників: кореляції та регресії з допомогою DATA ANALYSES:
•	Визначення кореляції між CO2 викидами та споживанням енергії, виробництвом енергії , ВВП, чисельністю жителів
•	побудова регресійної моделі для прогнозу викидів CO2 для України та світу

2. SQL (BigQuery): фільтрація та округлення вхідних даних
   
3. POWER BI:
   
a.cтворення окремої таблички _calc, у якій будуть збережені наступні міри:

•	енергоефективності на душу населення;
•	енергоефективності на одиницю ВВП окремо для України та для світу;
•	визначимо частку сумарних викидів CO2 України відносно сумарних світових;
•	долю ВВП України у світовому ВВП;
•	відсоток кількості жителів України в населенні світу.

b.створення дашборду в POWER BI, який містить наступні візуалізації:

•	фільтр основних показників відображення значень по країні (Україна/світ), з можливістю вибору лише одного із значень, для уникнення їх агрегації, що в даному випадку було б, некоректно, оскільки дані по Україні уже є частиною даних по світу;
•	картки з основними показниками, представленими у датасеті;
•	частка викидів по типу джерела енергії для України та світу;
•	матрицю споживання енергії та викидів CO2 по типу джерела енергії у відносному вимірі.
•	динаміка за період 2000-2019 рік вище розрахованих мір: % викидів, % ВВП, %населення, енергоємності на душу та одиницю ВВП (не змінюють значень при виборі Україна /світ, але співставляють їх одразу  на візуалізації)
•	частка викидів по типу джерела енергії для України та світу.

4. GOOGLE SLIDES – цілісна презентація проєкту з детальними висновками та рекомендаціями.
   
Проведений аналіз дозволяє оцінити стан енергоефективності економіки як України, так і світу, в цілому, що дозволяє визначити пріоритети у використанні джерел енергії із меншим продукуванням викидів CO2. 
Завдяки регресійній моделі, можна спрогнозувати рівень викидів CO2 , в залежності від обсягів їх споживання первинних джерел енергії.

ОТРИМАНІ ІНСАЙТИ:

Споживання енергії вугілля та природного газу в Україні протягом періоду суттєво скоротилось, а от відновлювана енергія використовувалась, на жаль, в мізерних кількостях. І тут варто розробляти заходи на державному рівні, переймаючи досвід країн, які змогли повністю перейти на такі джерела або суттєво збільшити % їх використання.
Показник енергоємності на душу населення в Україні вдвічі перевищував світовий на початку періоду, але станом на 2019р., суттєво зменшившись, практично досяг світового рівня.
Енергоємність ВВП  в Україні теж мала позитивну динаміку: показник знизився більше як у два рази:з 18,5 у 2000р. до 7,1 в 2019р.
Позитивною тенденцією є суттєве зменшення частки викидів CO2 України у сумарних світових викидах CO2 з 1.5% в 2000р. до 0,6% в 2019р. 
Вугілля є найбільшим емітентом CO2, на другому місті- нафта, на третьому - природній газ, тому варто поступово відмовлятись від їх споживання і знаходити шляхи переходу на відновлювані джерела енергії. 
