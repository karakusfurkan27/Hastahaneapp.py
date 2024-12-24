# Hastane Yönetim Sistemi

Bu proje, basit bir hastane yönetim sistemi uygulamasıdır. Tkinter kullanılarak geliştirilmiş bir grafiksel kullanıcı arayüzü (GUI) ile hasta, doktor ve randevu yönetimi yapılabilir. Veritabanı olarak SQLite kullanılmıştır.

## Özellikler

- **Hasta Ekleme**: Kullanıcı hasta adı, yaşı ve hastalığını girerek hasta ekleyebilir.
- **Hastaları Listeleme**: Sistemdeki tüm hastaların bilgileri listelenebilir.
- **Randevu Ekleme**: Hasta ID'si, doktor adı ve randevu tarihi girilerek randevu eklenebilir.
- **Doktor Ekleme**: Doktor adı ve uzmanlık alanı girilerek yeni bir doktor eklenebilir.
- **Doktorları Listeleme**: Sistemdeki tüm doktorların bilgileri listelenebilir.

## Kullanım

1. **Hasta Ekleme**: Hasta adı, yaşı ve hastalığı girerek hasta ekleme işlemi yapılabilir.
2. **Randevu Ekleme**: Var olan bir hastaya randevu eklemek için hasta ID'si, doktor adı ve randevu tarihi girilmelidir.
3. **Doktor Ekleme**: Yeni doktor eklemek için doktor adı ve uzmanlık alanı girilmelidir.
4. **Listeleme**: Sistemdeki hastalar ve doktorlar listelenebilir.

## Veritabanı Yapısı

Bu uygulama üç ana tabloyu kullanır:

1. **patients** (Hastalar):
   - `id`: Hasta ID'si (Birincil Anahtar)
   - `name`: Hasta Adı
   - `age`: Hasta Yaşı
   - `ailment`: Hasta Hastalığı

2. **appointments** (Randevular):
   - `id`: Randevu ID'si (Birincil Anahtar)
   - `patient_id`: Hasta ID'si (patients tablosuna yabancı anahtar)
   - `doctor_name`: Doktor Adı
   - `appointment_date`: Randevu Tarihi

3. **doctors** (Doktorlar):
   - `id`: Doktor ID'si (Birincil Anahtar)
   - `name`: Doktor Adı
   - `specialty`: Doktorun Uzmanlık Alanı

## Gereksinimler

- Python 3.x
- Tkinter (Python ile birlikte gelir)
- SQLite (Python ile birlikte gelir)

## Kurulum

1. Proje dosyasını indirin.
2. Python 3.x yüklü olduğundan emin olun.
3. Terminal veya komut satırında aşağıdaki komutları çalıştırarak programı başlatabilirsiniz:

```bash
python hospital_management_system.py
```

## Katkı

Katkıda bulunmak isterseniz, lütfen pull request (PR) oluşturun ve değişikliklerinizi açıklayın.
