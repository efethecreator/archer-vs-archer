# Archer vs Archer

Bu küçük terminal oyunu can sıkıntısı ve tekrar etme amaçlı yapılmıştır, iki okçunun birbirleriyle karşılıklı olarak ok attığı ve sağlık/ok durumlarının takip edildiği basit bir Python simülasyonudur. Testler otomatik olarak çalıştırılır ve sonuçlar terminalde görüntülenir.

## Dosya Yapısı

- `main.py`: Okçu sınıfı ve temel oyun mekaniği.
- `test.py`: Farklı senaryoları test eden ve sonuçları raporlayan test dosyası.

## Kullanım

1. Python 3 yüklü olduğundan emin olun.
2. Proje klasöründe terminal açın.
3. Testleri çalıştırmak için şu komutu girin:

   ```
   python test.py
   ```

4. Sonuçlar terminalde görünecektir.

## Sınıf Özellikleri

### Archer Sınıfı

- `name`: Okçunun adı
- `health`: Sağlık puanı
- `num_arrows`: Ok sayısı

#### Metotlar

- `shoot(target)`: Hedefe ok atar, ok sayısını azaltır ve hedefin sağlığını düşürür.
- `take_hit()`: Okçu vurulduğunda sağlık puanını azaltır, sağlık sıfır olursa hata fırlatır.
- `get_status()`: Okçunun adını, sağlığını ve ok sayısını döndürür.
- `print_status()`: Okçunun mevcut durumunu ekrana yazdırır.

## Testler

Testler, farklı okçu kombinasyonları ve beklenen sonuçlar ile otomatik olarak çalışır. Hatalı durumlarda beklenen hata mesajları kontrol edilir.

