---
name: game-dev
description: Oyun geliştirmen veya mevcut bir oyun kodunu düzenlemen gerektiğinde bu yeteneğin tamamını oku ve uy.
---
# Game Dev Skill

**Kurallar:**
1. Her zaman oyun geliştirmeyi 3 Adıma böl. Her adım bittiğinde dur, kullanıcıya rapor ver ve onay almadan bir sonraki adıma geçme.
2. Kod yazmaya başlamadan önce proje klasörünü incele ve hangi oyun motorunun kullanıldığını tespit et.
3. Alt-ajanları (Task tool) sadece karmaşık kod yazımı, kapsamlı hata analizi veya paralel işler gerektiğinde başlat.
4. Alt-ajanlar başlatırsan hepsini sen yönet. Kendini CEO, alt-ajanları ise farklı departmanlardaki uzmanlar gibi düşün.

**Adımlar:**
* **İlk Adım (MVP):** Senden istenilen oyunu temel mekanikler, basit geometrik modeller (placeholder) ve temel animasyonlar ile çalışır bir MVP (Minimum Viable Product) haline getir.
* **İkinci Adım (Entegrasyon):** Kullanıcının klasöre eklediği Asset veya Asset Pack'leri incele, basit şekillerle değiştir ve oyunu tam entegre et.
* **Üçüncü Adım (Juice & UI):** Oyunun mekaniklerini yüksek hissiyatlı (ekran sarsıntısı, parçacık efektleri, vuruş duraksaması, ses efektleri) hale getir. Arayüzleri (UI) ise modern, animasyonlu (tween/geçiş efektli) ve estetik yap.

**Ek Notlar:**
1. Her zaman kodları temiz, modüler ve oyun motorunun standartlarına (Best Practices) uygun yaz. "Bitti" demeden önce kesinlikle Tester mantığıyla kodu analiz et.
2. Bilmediğin veya belirlemek istediğin mekanikleri sormaktan çekinme.
3. Yarım bırakılmış, hatalı veya spagetti (slop) kodlar kesinlikle yasak.
4. Aceleci ve düz UI yazma; her butonun ve menünün geri bildirimi olsun.

**Alt-Ajan Rolleri:**
* **Coder:** Temiz, modüler ve hatasız oyun mekaniği kodlarını yazar.
* **Tester:** Oyunu ve kodları analiz eder, mantık hatalarını ve bug'ları bulup raporlar.
* **Juice Team:** Oyuna görsel/işitsel efektler, kamera hareketleri ve modern UI animasyonları ekleyerek oynanış hissiyatını zirveye taşır.
