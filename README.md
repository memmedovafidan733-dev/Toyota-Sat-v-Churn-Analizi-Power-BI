# Toyota-Satış-və-Churn-Analizi-Power-BI
Toyota avtomobil şirkətinin müvafiq qitələr üzrə stok səviyyələri, satış dinamikası, müştəri itkisi (Churn) göstəriciləri üzrə təhlili.

# Xülasə
Bu layihə Toyota korporasiyasının 4 region üzrə (Avropa, Asiya, Amerika, Okeaniya) 2019-2022-ci il aralığındakı 4 illik satış, stok, satış mərkəzləri, şəhərlərin coğrafi koordinatları kimi datasetləri üzərindən analizi əhatə edir.


## Layihənin məqsədi
* Müvafiq regionlar üzrə satış dinamikası, stok səviyyələri, müştəri itkisi(Churn) və satışın illik/aylıq artım göstəriciləri üzrə interaktiv dashboardların, xəritə vizualının qurulması ilə qərarverməyə dəstək.


### Layihədə istifadə edilən texniki alətlər
    Power BI   •   Power Query Editor   •   Microsoft Excel


### Qurulmuş data model
* **Fakt/Əməliyyat Cədvəlləri (Fact Tables):** 
  * `Toyota_sales` (Şəhərlər, tarixlər və SKU-lar üzrə satış əməliyyatları)
  * `Toyota_stock` (Tarix, SKU və satış mərkəzləri üzrə anbar stok qeydləri)
* **Axtarış Cədvəlləri (Lookup Tables):** 
  * `Calendar` (Time intelligence hesablamaları üçün DAX ilə yaradılmış təqvim cədvəli)
  * `Toyota_city` (Coğrafi iyerarxiya: Qitə, Ölkə, Şəhər, Satış mərkəzi)
  * `Toyota_sku` (Məhsul kataloqu: Maşın adı, Ban növü, Model kodu, Satış ili)    

Şəkil: Data modelin sxemi
  <img width="1919" height="984" alt="image" src="https://github.com/user-attachments/assets/d9f42acd-f99d-4539-b1d2-52a80f382d0d" />


### Layihədə icra edilən proseslər
* Power Query Editor: "Toyota Database Sales.xlsx"  faylındakı 2019-2022-ci il aralığındakı satış cədvəli səhifələrinin Append queries as new vasitəsilə Toyota sales cədvəlində birləşdirilməsi; Remove top rows vasitəsilə çirkli datanın təmizlənməsi; 
* İstifadə edilən DAX-lar: CALCULATE, LASTDATE, SUM, DISTINCTCOUNT, IF, DATE, FILTER, COUNT, DATEADD, ISBLANK, DIVIDE, SAMEPERIODLASTYEAR,  MINX, MAXX, UNION, SELECTCOLUMNS, ADDCOLUMNS, SWITCH, FORMAT;
* İstifadə edilən vizuallar: Map, Card, Slicer, Clustered bar chart, Clustered column chart, Table, Matrix table; 
* Conditional formatting: Ötən aya görə satışın artım faizi, satışın ildən-ilə böyümə faizi kimi məlumatların şərti formatlama ilə fərqləndirilməsi.


### Dashboard səhifələri
* "Asiya qitəsi üzrə Xəritə"

<img width="1915" height="975" alt="image" src="https://github.com/user-attachments/assets/8bdad5ce-35ac-4e74-994c-cb42e3adc4da" />

    
* "Okeaniya qitəsi üzrə Stok Analizi"

<img width="1919" height="981" alt="image" src="https://github.com/user-attachments/assets/28a6e32e-64a2-4019-99b2-f8e83ab7aa6b" />

    
* "Amerika qitəsi üzrə Churn Analizi"

<img width="1919" height="975" alt="image" src="https://github.com/user-attachments/assets/1ea2b901-2c45-443e-b34c-50e299a78bdb" />

    
* "Avropa qitəsi üzrə Satış Analizi"

<img width="1919" height="978" alt="image" src="https://github.com/user-attachments/assets/c1b62508-b32f-478e-b941-3d9a16ed4caa" />

