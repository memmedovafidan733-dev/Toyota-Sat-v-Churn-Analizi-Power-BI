# Toyota-Satış-və-Churn-Analizi-Power-BI
Toyota avtomobil şirkətinin müvafiq qitələr üzrə stok səviyyələri, satış dinamikası, müştəri itkisi (Churn) göstəriciləri üzrə təhlili.

# Xülasə
Bu layihə Toyota korporasiyasının 4 region üzrə (Avropa, Asiya, Amerika, Okeaniya) 2019-2022-ci il aralığındakı 4 illik satış, stok, satış mərkəzləri, şəhərlərin coğrafi koordinatları kimi datasetləri üzərindən analizi əhatə edir.


## Layihənin məqsədi
* Müvafiq regionlar üzrə satış dinamikası, stok səviyyələri, müştəri itkisi(Churn) və satışın illik/aylıq artım göstəriciləri üzrə interaktiv dashboardların, xəritə vizualının qurulması ilə qərarverməyə dəstək.

### Layihədə istifadə edilən texniki alətlər
    Power BI   •   Microsoft Excel   •   Power Query 


### Faylların strukturu(Excel workbook)


### Faylın strukturu(Power BI)
1.




### Qurulmuş data modelin sxemi
* Fakt cədvəlləri: 
 Toyota sales



* **Fakt Cədvəlləri (Fact Tables):** 
  * `Toyota_sales` (Şəhərlər, tarixlər və SKU-lar üzrə satış əməliyyatları)
  * `Toyota_stock` (Tarix, SKU və satış mərkəzləri üzrə anbar stok qeydləri)
* **Ölçü Cədvəlləri (Dimension Tables):** 
  * `Calendar` (Zaman intellekti hesablamaları üçün DAX ilə yaradılmış təqvim cədvəli)
  * `Toyota_city` (Coğrafi iyerarxiya: Qitə, Ölkə, Şəhər, Satış mərkəzi)
  * `Toyota_sku` (Məhsul kataloqu: Maşın adı, Ban növü, Model kodu, Satış ili)




### Layihədə icra edilən proseslər
* Power Query: Tarix sütununun Split Column vasitəsilə ayrılması;  
* Power Pivot: Göstəricilərin, reytinq kateqoriya bölgüsünün, növbəti həftəlik planın və endirim kampaniyalarının hesablanması üçün measures vasitəsilə data modelin qurulması;
* Pivot Table: Nəticələr üzrə ümumiləşdirilərək cədvəl hesabatların hazırlanması;
* İstifadə edilən funksiyalar: IF, AND, OR, MAX, MIN, CALCULATE, SUM, COUNT, SUMX, DISTINCT, SWITCH, DISTINCTCOUNT, ALL, QUARTILE.EXC, IQR metodu ilə outlier dəyərlərin tapılması;
* Conditional formatting: Outlier dəyərlərə malik sürücülərin məlumatlarının şərti formatlama ilə vizuallaşdırılması.


    Şəkil: Data modelin sxemi
  <img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/5a64dbab-33be-4c88-8d6d-caf45fdda7e8" />
