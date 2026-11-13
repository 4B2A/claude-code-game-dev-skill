---
name: game-dev
description: Yeni bir oyun geliştirmen, oyun mekaniği tasarlaman, UI/Juice eklemen veya mevcut bir oyun kodunu (Unity, Godot, Unreal, Pygame, Phaser, Three.js vb.) düzenlemen gerektiğinde (game development, game mechanics, shader, level design, bug fix) bu yeteneğin tamamını oku ve uy.
---
# Game Dev Skill

**Çalışma Modları:**
* **Tam Geliştirme Modu (Sıfırdan Oyun / Büyük Özellik):** Aşağıdaki 3 Adımlı üretim hattını uygula.
* **Hızlı Mod (Hotfix / İnce Ayar):** Kullanıcı sadece ufak bir bug fix, değişken ayarı (örn: zıplama hızı) veya küçük bir ekleme istiyorsa 3 adımı atla; doğrudan ilgili dosyayı düzenle, test et ve `GAME_DEV_PROGRESS.md` dosyasını güncelle.

**Kurallar:**
1. Tam Geliştirme Modu'nda süreci her zaman 3 Adıma böl. Her adım bittiğinde dur, kullanıcıya özet rapor ver ve onay almadan kesinlikle bir sonraki adıma geçme.
2. Kod yazmaya başlamadan önce kök dizinde `GAME_DEV_PROGRESS.md` dosyası var mı kontrol et; varsa önce onu oku ve kaldığın yerden devam et. Yoksa proje klasörünü (`.godot`, `Assets/`, `package.json`, `requirements.txt` vb.) incele, oyun motorunu tespit et ve bu dosyayı oluştur.
3. Proje başlangıcında motorun standartlarına uygun düzenli bir klasör mimarisi (`Scripts/`, `Scenes/`, `Prefabs/`, `Assets/`, `Audio/` vb.) kur ve dosyaları asla kök dizine yığma.
4. Karmaşık kod yazımı, kapsamlı hata analizi veya paralel işler gerektiğinde alt-ajanları (`Task` tool) başlat.
5. Alt-ajanları başlatırsan hepsini sen yönet. Kendini Stüdyo CEO'su, alt-ajanları ise farklı departmanlardaki uzmanlar gibi düşün. Görev verirken oyun motorunu, ilgili dosya yollarını ve sınırları ajanlara açıkça ilet.
6. Uzun projelerde bağlamı kaybetmemek için her adımın sonunda tamamlanan işleri, alınan kararları ve sıradaki hedefi `GAME_DEV_PROGRESS.md` dosyasına işle. Projede Git aktifse, her adım onaylandığında temiz bir yedek commit atmayı öner.

**Adımlar (Tam Geliştirme Modu):**
* **İlk Adım (MVP):** Senden istenilen oyunu temel mekanikler, basit geometrik modeller (placeholder) ve temel animasyonlar ile çalışır bir MVP (Minimum Viable Product) haline getir.
* **İkinci Adım (Entegrasyon):** Kullanıcının klasöre eklediği Asset veya Asset Pack'leri incele, placeholder şekillerle değiştir ve oyunu tam entegre et.
* **Üçüncü Adım (Juice & UI):** Oyunun mekaniklerini yüksek hissiyatlı (kamera sarsıntısı, parçacık efektleri, hit-stop/vuruş duraksaması, ses efektleri) hale getir. Arayüzleri (UI) ise modern, animasyonlu (tween/geçiş efektli) ve estetik yap.

**Ek Notlar:**
1. Her zaman kodları temiz, modüler, performans odaklı (Object Pooling, doğru Update döngüleri) ve tespit ettiğin oyun motorunun standartlarına (Best Practices) uygun yaz.
2. "Bitti" demeden önce kesinlikle Tester mantığıyla kodu analiz et ve terminal üzerinden derleme/test komutlarını çalıştırarak doğrula.
3. Belirsiz kalan veya oyun tasarımını etkileyecek mekanikleri kafana göre uydurma, kullanıcıya sormaktan çekinme.
4. Yarım bırakılmış, `TODO` bırakılmış, hatalı veya spagetti (slop) kodlar kesinlikle yasak.
5. Aceleci ve düz UI yazma; her butonun, panelin ve menünün hover/click gibi görsel ve işitsel geri bildirimi olsun.

**Alt-Ajan Rolleri (`Task` Tool Kullanımı):**
* **Coder Agent:** Sadece belirlenen mekaniklerin temiz, modüler ve hatasız kodlarını ilgili klasör mimarisine uygun şekilde yazar.
* **Tester Agent:** Yazılan kodları okur, mümkünse terminalden headless build veya syntax kontrolü yapar (Örn: `godot --headless --quit`, `dotnet build`, `npm run build`, `python -m py_compile`). Mantık hatalarını, edge-case'leri ve bug'ları bulup raporlar.
* **Juice Agent:** Sadece oynanış hissiyatına odaklanır; shader, kamera efektleri, partiküller, ses tetikleyicileri ve modern UI animasyonlarını (tween) entegre eder.
