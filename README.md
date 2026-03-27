# DATA-LEAGUE-26---Kay-p-Randevu-No-Show-Tahmini
DATA LEAGUE'26 yarışması için geliştirilmiş, CatBoost tabanlı Kayıp Randevu (No-Show) tahminleme modeli.


# DATA LEAGUE'26 - Kayıp Randevu (No-Show) Tahmini 

## Proje Açıklaması 
Bu proje, sağlık hizmetlerinde verimliliği düşüren en kritik sorunlardan biri olan "Kayıp Randevu (No-Show)" problemini çözmek amacıyla **GENESIS** takımı tarafından DATA LEAGUE'26 yarışması için geliştirilmiştir. Hastaların geçmiş randevu sicili, klinik yükü ve randevu alma süresi gibi faktörleri barındıran ilişkisel bir veri seti kullanılarak, hastaların randevularına gelmeme (`label_noshow`) olasılıkları CatBoost algoritması ile modellenmiştir. Proje, yarışmada 9. sıraya yerleşerek Sakarya'da düzenlenecek Büyük Final Datathonu'na katılmaya hak kazanmıştır.

## Veri Seti Yapısı 
Projede hastane senaryosuna ait ilişkisel veri dosyaları kullanılmıştır:
* `appointments_train.csv`: Model eğitimi için kullanılan ve `label_noshow` hedefini içeren randevu verileri.
* `appointments_test.csv`: Modelin tahmin üreteceği test randevu verileri.
* `patients.csv`: Hastalara ait demografik özellikler ve geçmiş sicil bilgileri.
* `clinics.csv`: Kliniklere ait kapasite, yoğunluk ve branş bilgileri.
* `sample_submission.csv`: Platforma yüklenecek tahmin sonuçlarının örnek şablonu.

## Kod ve Model Geliştirme 
* `cat.boost0-514987.jpynb` ve `5155506.ipynb`: Verilerin birleştirilmesi, keşifsel veri analizi (EDA), özellik mühendisliği (feature engineering) ve model eğitimini içeren Jupyter Notebook dosyalarıdır. 
* Projede yüksek performans ve hız sağlaması amacıyla ana makine öğrenmesi modeli olarak **CatBoost** algoritması tercih edilmiştir.

## Kullanılan Teknolojiler 
* Python
* Pandas & NumPy (Veri manipülasyonu ve analizi)
* CatBoost (Makine Öğrenmesi Modeli)
* Scikit-Learn
