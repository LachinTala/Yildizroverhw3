Veri Seti

Toplam: 652 görsel

Eğitim (Train): 456

Doğrulama (Valid): 131

Test: 65

Veri seti Roboflow platformundan alınmış ve STOP işaretinin farklı açılardan, ışık koşullarından ve durumlarından oluşan görselleri içermektedir.

Veri setinde ayrıca sahte (fake) ve vandalize edilmiş STOP işaretleri de bulunmaktadır.

Kullanılan Model

Model Tipi: Roboflow 3.0 Object Detection (Accurate)

Önceden eğitilmiş model (pre-trained) üzerinden transfer learning yapılmıştır.

Parametreler:

Epoch: ~300

Image Size: 640 px

Batch Size: Roboflow tarafından otomatik ayarlanmıştır

Optimizer: Varsayılan (Adam/SGD)

 Sonuçlar

mAP@50: %97.8

Precision: %93.9

Recall: %92.6

Sınıf bazında doğruluk:

Stop Sign → %99

Fake Stop Sign → %100

Vandalized Stop Sign → %95

Eğitim Grafikleri

Box Loss, Class Loss ve Object Loss değerleri eğitim boyunca düzenli olarak azalmıştır.

mAP değerleri hızlı şekilde yükselmiş ve %0.9 seviyelerinde sabitlenmiştir.

Test Örnekleri

Model, standart STOP işaretlerini yüksek doğrulukla tespit etmiştir.

Bazı testlerde sahte tabelalar da STOP işaretiyle karıştırılmıştır (ör. kırmızı sekizgen şekilli sahte işaret %97 güven ile etiketlenmiştir).

Örnek sonuç görselleri bu repoya eklenmiştir (/samples klasöründe).

Nasıl Çalıştırılır?

Bu proje Roboflow ortamında GUI üzerinden gerçekleştirilmiştir, dolayısıyla özel Python kodu bulunmamaktadır.
Modeli denemek için:

[Roboflow proje linki](MODEL_URL buraya eklenebilir) üzerinden model açılabilir.

“Upload Image or Video File” seçeneğiyle kendi görselleriniz üzerinde test yapabilirsiniz.

“Try on My Machine” seçeneğiyle modeli bilgisayarınızda da çalıştırabilirsiniz.

 Kaynaklar

Roboflow Documentation

YOLO Object Detection Models