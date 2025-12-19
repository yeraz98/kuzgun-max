# 🦅 Kuzgun-MAX (500 Thread Edition)

Bu araç, web sitesi performans testleri için geliştirilmiş, yüksek kapasiteli bir L7 test aracıdır.

## 🚀 Özellikler
- **500 İş Parçacığı:** Maksimum paket trafiği.
- **Otomatik Port:** 80 ve 443 tespiti.
- **Tor Entegrasyonu:** Otomatik gizlilik.

## 📥 Diğer Telefona Tek Komutla Kurulum
Yeni bir Termux'ta her şeyi saniyeler içinde kurmak için şu dev komutu kopyalayıp yapıştırın:

```bash
pkg install python git tor -y && git clone [https://github.com/yeraz98/kuzgun-max](https://github.com/yeraz98/kuzgun-max) && cd kuzgun-max && mv kuzgun.py ~ && echo -e 'tor > /dev/null 2>&1 &\nsaldir() { if nc -zw1 $1 443 2>/dev/null; then PORT=443; else PORT=80; fi; env -u LD_PRELOAD python3 ~/kuzgun.py $1 $PORT; }' >> ~/.bashrc && source ~/.bashrc




🛠 Kullanım
Kurulumdan sonra sadece şunu yazın:

saldir hedefsite.com




⚠️ Yasal Uyarı
​Sorumluluk kullanıcıya aittir.
