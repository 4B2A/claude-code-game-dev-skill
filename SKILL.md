---
name: game-dev
description: Yeni bir oyun geliştirmen, oyun mekaniği tasarlaman, UI/Juice eklemen veya mevcut bir oyun kodunu (Unity, Godot, Unreal, Pygame, Phaser, Three.js vb.) düzenlemen gerektiğinde (game development, game mechanics, shader, level design) bu yeteneğin tamamını oku ve uy.
---
# Game Dev Skill

**Kurallar:**
1. Her zaman oyun geliştirmeyi 3 Adıma böl. Her adım bittiğinde dur, kullanıcıya özet rapor ver ve onay almadan kesinlikle bir sonraki adıma geçme.
2. Kod yazmaya başlamadan önce kök dizinde `GAME_DEV_PROGRESS.md` dosyası var mı kontrol et; varsa önce onu oku ve kaldığın yerden devam et. Yoksa proje klasörünü (`.godot`, `Assets/`, `package.json`, `requirements.txt` vb.) incele, oyun motorunu tespit et ve bu dosyayı oluştur.
3. Karmaşık kod yazımı, kapsamlı hata analizi veya paralel işler gerektiğinde alt-ajanları (`Task` tool) başlat.
4. Alt-ajanları başlatırsan hepsini sen yönet. Kendini CEO, alt-ajanları ise farklı departmanlardaki uzmanlar gibi düşün. Görev verirken hangi oyun motorunun kullanıldığını, ilgili dosya yollarını ve sınırları ajanlara açıkça ilet.
5. Uzun projelerde bağlamı kaybetmemek için her adımın sonunda tamamlanan işleri, alınan kararları ve sıradaki hedefi `GAME_DEV_PROGRESS.md` dosyasına işle.

**Adımlar:**
* **İlk Adım (MVP):** Senden istenilen oyunu temel mekanikler, basit geometrik modeller (placeholder) ve temel animasyonlar ile çalışır bir MVP (Minimum Viable Product) haline getir.
* **İkinci Adım (Entegrasyon):** Kullanıcının klasöre eklediği Asset veya Asset Pack'leri incele, basit şekillerle değiştir ve oyunu tam entegre et.
* **Üçüncü Adım (Juice & UI):** Oyunun mekaniklerini yüksek hissiyatlı (kamera sarsıntısı, parçacık efektleri, hit-stop/vuruş duraksaması, ses efektleri) hale getir. Arayüzleri (UI) ise modern, animasyonlu (tween/geçiş efektli) ve estetik yap.

**Ek Notlar:**
1. Her zaman kodları temiz, modüler ve tespit ettiğin oyun motorunun standartlarına (Best Practices) uygun yaz. "Bitti" demeden önce kesinlikle Tester mantığıyla kodu analiz et ve mümkünse terminal üzerinden derleme/test komutlarını çalıştırarak doğrula.
2. Belirsiz kalan veya oyun tasarımını etkileyecek mekanikleri kafana göre uydurma, kullanıcıya sormaktan çekinme.
3. Yarım bırakılmış, `TODO` bırakılmış, hatalı veya spagetti (slop) kodlar kesinlikle yasak.
4. Aceleci ve düz UI yazma; her butonun, panelin ve menünün hover/click gibi görsel ve işitsel geri bildirimi olsun.

**Alt-Ajan Rolleri (`Task` Tool Kullanımı):**
* **Coder Agent:** Sadece belirlenen mekaniklerin temiz, modüler ve hatasız kodlarını yazar.
* **Tester Agent:** Yazılan kodları okur, mümkünse terminalden build/test alır; mantık hatalarını, edge-case'leri ve bug'ları bulup raporlar.
* **Juice Agent:** Sadece oynanış hissiyatına odaklanır; shader, kamera efektleri, partiküller ve modern UI animasyonlarını (tween) entegre eder.
