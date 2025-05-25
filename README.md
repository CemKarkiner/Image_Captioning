# 🧠 Image Captioning with BLIP (Salesforce)

Bu proje, [Salesforce BLIP (Bootstrapping Language-Image Pre-training)](https://huggingface.co/Salesforce/blip-image-captioning-base) modelini kullanarak görseller için otomatik açıklama (caption) üretir. Eğitim verisi analizi, görselleştirme ve test görsellerine altyazı üretimi işlemleri bu notebook içerisinde adım adım uygulanmaktadır.

## 📁 Proje Yapısı

image_captioning_blip.ipynb # Ana Jupyter Notebook dosyası
train.csv # Eğitim veri dosyası
test.csv # Test veri dosyası
train_images/ # Eğitim görselleri klasörü
test/ # Test görselleri klasörü (alt klasörde .jpg formatında)
submission.csv # Üretilen caption'ların yer aldığı çıktı dosyası


## ⚙️ Kullanılan Teknolojiler

- Python 3.x
- [Hugging Face Transformers](https://huggingface.co/transformers/)
- PyTorch
- BLIP Image Captioning Model
- pandas, matplotlib, PIL

## 🚀 Kurulum ve Kullanım

### 1. Gerekli kütüphaneleri yükleyin


    pip install transformers torch pandas matplotlib pillow

### 2. Notebook'u çalıştırın

image_captioning_blip.ipynb dosyasını açarak aşağıdaki işlemleri gerçekleştirebilirsiniz:

  - Eğitim ve test verilerini yükleme

  - Eksik veri analizi

  - Örnek görsellerin gösterimi

  - BLIP modeli ile altyazı (caption) üretimi

  - submission.csv dosyasının kaydedilmesi

### 3. Test Caption'larını Üretin

Notebook, test setindeki her görsel için BLIP modeli kullanarak açıklamalar üretir ve submission.csv dosyasına kaydeder.

## 🖼️ Örnek Çıktı
image_id	caption
123.jpg	a man riding a bike on the road
456.jpg	a group of people at the beach

## 📌 Notlar
 Model, CPU'da da çalışır ancak GPU ile çok daha hızlı sonuç verir.
