# Derin-Ogrenme-ile-Saglikli-ve-Sagliksiz-Retina-Optik-Disk-Goruntulerinin-Taninmasi
"https://www.kaggle.com/datasets/andrewmvd/retinal-disease-classification/data" 
Proje Başlığı: RFMiD Veri Seti ile Derin Öğrenme Tabanlı Retinal Hastalık Sınıflandırması: Çoklu Model Karşılaştırması

Proje Özeti: Bu proje, RFMiD (Retinal Fundus Multi-disease Image Dataset) veri setini kullanarak göz dibi (fundus) görüntülerinden "Hastalık Riski (Disease Risk)" tespitini otomatize etmeyi amaçlamaktadır.

Çalışmanın temel amacı, farklı derin öğrenme mimarilerinin biyomedikal görüntü sınıflandırma performanslarını kıyaslamak ve klinikte kullanılabilecek yüksek doğruluklu bir Erken Uyarı Sistemi prototipi geliştirmektir.

Kullanılan Modeller ve Metodoloji: Projede, "Özel Tasarım/Deneysel" modeller ile "Modern (SOTA)" mimariler karşılaştırmalı olarak analiz edilmiştir:

Temel ve Deneysel Yaklaşımlar:

Basic CNN (Baseline): Projenin başarım alt sınırını belirlemek için geliştirdiğimiz özel ardışık (sequential) model.

U-Net Classifier: Geleneksel olarak segmentasyon (bölütleme) için kullanılan U-Net mimarisi, bu projede özgün bir yaklaşımla modifiye edilerek sınıflandırma problemine uyarlanmış ve performans potansiyeli test edilmiştir.

Modern Mimariler (State-of-the-Art):

ResNet50: Derin ağlardaki öğrenme problemlerini çözen "Residual" yapısı sayesinde güçlü bir referans noktası olarak kullanılmıştır.

DenseNet121: Katmanlar arası yoğun veri akışı sağlayan yapısıyla yüksek doğruluk hedeflenmiştir.

ConvNeXt Tiny: Modern Transformer yapılarından esinlenen bu CNN modeli, çalışmamızda en yüksek performansı (%99+ ROC AUC) gösteren "Şampiyon Model" olmuştur.

Hedefler ve Sonuçlar:

Dengesiz veri setine (Imbalanced Dataset) rağmen modern mimarilerle 0.97 üzerinde F1-Score başarısı elde edilmiştir.

Segmentasyon ağlarının (U-Net) sınıflandırma görevindeki başarısı analiz edilmiştir.

Tıbbi tanıda kritik olan "Hastalığı Kaçırmama" (Yüksek Recall/ROC AUC) hedefine ulaşılmıştır.
