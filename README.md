# tenisMaciTahmini
# ATP Tenis Maçı Sonucu Tahmini Projesi

Bu proje, ATP tenis maçları verilerini kullanarak maç sonuçlarını tahmin etmek için makine öğrenme tekniklerini uygular. Amaç, oyuncu özellikleri ve maç istatistiklerine dayalı olarak, bir tenis maçının kazananını tahmin etmektir.

## Proje Özeti

Proje, 2020-2024 yılları arasındaki ATP tenis maçlarına ait verileri kullanarak, dört farklı makine öğrenme modelini (Random Forest, XGBoost, SVM ve Karar Ağaçları) eğitir ve performanslarını karşılaştırır. 

Makine öğrenme modelleri, maç istatistikleri ve oyuncu özellikleri (yaş, boy, servis sayısı vb.) gibi veriler kullanılarak eğitilmiştir. Sonuçlar, doğruluk, precision, recall, F1 skoru ve ROC AUC gibi metrikler kullanılarak değerlendirilmiştir.

## Kullanılan Modeller

1. **Random Forest (RF)**  
   - Birden fazla karar ağacının birleşiminden oluşan bir model.
   - Modelin genelleme yeteneği güçlüdür ve overfitting'i engeller.

2. **XGBoost**  
   - Ağaç tabanlı öğrenme algoritmalarına dayalı güçlü bir model.
   - Hızlıdır ve büyük veri setlerinde yüksek performans gösterir.

3. **SVM (Support Vector Machine)**  
   - Veri setindeki örnekler arasında en iyi ayrım çizgisini bulmaya çalışan model.
   - İyi genelleme performansı sağlar.

4. **Karar Ağaçları**  
   - Veri setini dallara ayırarak kararlar alır.
   - Modelin nasıl çalıştığını anlamak ve yorumlamak kolaydır, ancak overfitting riski vardır.

## Veri Seti

Proje, [Huge Tennis Dataset](https://www.kaggle.com/datasets) adlı veri setini kullanır. Veri seti, oyuncu özellikleri ve maç sonuçları gibi bilgileri içeren yaklaşık 73247 satır ve 49 sütundan oluşmaktadır.

Öne çıkan özellikler:
- **winner_rank**: Kazanan oyuncunun sıralaması
- **loser_rank**: Kaybeden oyuncunun sıralaması
- **winner_age**: Kazanan oyuncunun yaşı
- **loser_age**: Kaybeden oyuncunun yaşı
- **surface**: Maçın oynandığı zemin (Hard, Clay, Grass vb.)
- **w_ace**: Kazanan oyuncunun kazandığı "ace" sayısı
- **l_ace**: Kaybeden oyuncunun kazandığı "ace" sayısı

## Proje Amaçları

- Farklı makine öğrenme modellerinin tenis maç sonuçları üzerindeki performanslarını karşılaştırmak.
- Verinin özelliklerini analiz etmek ve özellik mühendisliği uygulamak.
- Verinin ön işlenmesi ve temizlik adımlarını gerçekleştirmek.
- Model doğruluğunu artırmak için hiperparametre optimizasyonu uygulamak.

## Kullanım

Proje, Python ile yazılmıştır ve aşağıdaki kütüphaneleri kullanır:

- `scikit-learn`
- `pandas`
- `matplotlib`
- `seaborn`
- `xgboost`
- `shap`
