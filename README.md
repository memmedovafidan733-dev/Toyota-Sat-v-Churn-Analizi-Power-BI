# Toyota-Satış-və-Churn-Analizi-Power-BI
Toyota avtomobil şirkətinin müvafiq qitələr üzrə stok səviyyələri, satış dinamikası, müştəri itkisi (Churn) göstəriciləri üzrə təhlili.

# Xülasə
Bu layihə Toyota korporasiyasının 4 region üzrə (Avropa, Asiya, Amerika, Okeaniya) 2019-2022-ci il aralığındakı 4 illik satış, stok, satış mərkəzləri, şəhərlərin coğrafi koordinatları kimi datasetləri üzərindən analizi əhatə edir.


## Layihənin məqsədi
* Müvafiq regionlar üzrə satış dinamikası, stok səviyyələri, müştəri itkisi(Churn) və satışın illik/aylıq artım göstəriciləri üzrə interaktiv dashboardların, xəritə vizualının qurulması ilə qərarverməyə dəstək.

### Layihədə istifadə edilən texniki alətlər
    Power BI   •   Microsoft Excel   •   Power Query 


### Qurulmuş data model
* **Fakt Cədvəlləri (Fact Tables):** 
  * `Toyota_sales` (Şəhərlər, tarixlər və SKU-lar üzrə satış əməliyyatları)
  * `Toyota_stock` (Tarix, SKU və satış mərkəzləri üzrə anbar stok qeydləri)
* **Ölçü Cədvəlləri (Dimension Tables):** 
  * `Calendar` (Time intelligence hesablamaları üçün DAX ilə yaradılmış təqvim cədvəli)
  * `Toyota_city` (Coğrafi iyerarxiya: Qitə, Ölkə, Şəhər, Satış mərkəzi)
  * `Toyota_sku` (Məhsul kataloqu: Maşın adı, Ban növü, Model kodu, Satış ili)    

Şəkil: Data modelin sxemi
  <img width="1919" height="984" alt="image" src="https://github.com/user-attachments/assets/d9f42acd-f99d-4539-b1d2-52a80f382d0d" />

### Dashboard səhifələri
1. "Asiya qitəsi üzrə Xəritə" -
2. "Okeaniya qitəsi üzrə Stok Analizi" -
3. "Amerika qitəsi üzrə Churn Analizi" -
4. "Avropa qitəsi üzrə Satış Analizi" - 


### Layihədə icra edilən proseslər
* Power Query: 
* İstifadə edilən DAX-lar: ;
* Conditional formatting: Outlier məlumatlarının şərti formatlama ilə vizuallaşdırılması.


   
