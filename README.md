# 🎯 CHIZ Game Hub

**FPS oyuncuları için yerel, ücretsiz ve profesyonel antrenman uygulaması.**

---

🚀 İndir • ✨ Özellikler • 🆕 Yenilikler • 💻 Kurulum • 🛠️ Teknolojiler

---

## 🎯 Nedir Bu?

**CHIZ Game Hub**, FPS oyuncuları için tasarlanmış, **tamamen yerel** ve **ücretsiz** bir antrenman uygulamasıdır. Aim becerilerini geliştirmekten sistem performansını analiz etmeye kadar her şey tek bir yerde.

Counter-Strike 1.6'dan bugüne FPS oyunları oynayan biri olarak (Valorant, CS2 gibi oyunlarda üst düzey), bu uygulamayı **hem kendim hem de benim gibi düşünen oyuncular için** geliştirdim.

> 💡 **%100 Yerel** — Hiçbir verin dışarı gitmez. İnternet gerekmez. Reklam yok, abonelik yok.

---

## ✨ Özellikler

### 🎯 Antrenman

- **16 Aim Modu** — Reaction, Flick, Click, Tracking, Precision, Gridshot, Microshot, Micro Flick, Switching, Strafing, Moving Grid, Track+Strafe, **Track+Click**, **Gridshot Plus**, **Double Aim**
- **🤖 AI Rakip Bot** — 5 zorluk seviyesi, adaptif mod
- **🤖 AI Antrenman Koçu** — Yerel LLM ile kişisel öneriler
- **📊 Isı Haritası** — Vuruşlarını görselleştir
- **🔥 Günlük Streak** — Seri antrenmanlarla motive ol
- **⏱️ Pomodoro** — 25 dk odak + 5 dk mola

### 📊 Analiz

- **📈 Gerçek FPS Ölçümü** — PresentMon ile doğru FPS, 1% low, bottleneck analizi
- **🖥️ Sistem Monitörü** — CPU, GPU, RAM, disk, fan, voltaj canlı takip
- **🧪 Stres Testi** — CPU, RAM, GPU, disk için kapsamlı testler
- **💾 Disk Sağlık** — SMART verileri, sıcaklık, sağlık skoru
- **🌐 Ağ Araçları** — Ping, Traceroute, DNS Testi, Hız Testi
- **📈 Haftalık/Aylık Rapor** — Detaylı antrenman analizi, mod bazlı performans grafikleri

### 🎨 Kişiselleştirme

- **13 Tema** — Dark, Midnight, Light, Nord, Dracula, Solarized, Tokyo Night, Gruvbox, Catppuccin, One Dark, **Cyberpunk**, **Rose Pine**, **GitHub Dark**
- **🎨 Özel Accent Rengi** — Kendi rengini seç
- **🌐 5 Dil** — Türkçe, İngilizce, Almanca, Rusça, İspanyolca
- **⏰ Otomatik Tema** — Saate göre gündüz/gece

### 🎮 Overlay'ler

- **Crosshair** — Click-through, tamamen özelleştirilebilir
- **Performance HUD** — CPU/RAM/GPU/Ping + oyun FPS'i
- **Saat**, **Timer**, **FPS Counter**
- **Çoklu Monitör** desteği

### 🏆 Diğer

- **36 Başarı** — İlerlemeni oyunlaştır (streak, mod, toplam skor bazlı)
- **Kullanıcı Profilleri** — Birden fazla hesap
- **Game Launcher** — Programlarını tek yerden başlat
- **Game Profiles** — Grup halinde başlat (Valorant + Discord + OBS)
- **Otomatik Güncelleme** — Yeni sürümler otomatik bildirilir

---

## 🆕 Yenilikler

### v1.2.0 — Yeni Modlar & Rapor Sistemi

**🎯 3 Yeni Aim Modu:**
- **Track+Click** — Hareket eden hedefe tıkla (Track + Click)
- **Gridshot Plus** — 5x5 grid üzerinde 40 hedef, daha zor
- **Double Aim** — Aynı anda iki hedefe sırayla vur

**🏆 15 Yeni Başarı (Toplam 36):**
- Streak bazlı: Alev Aldı, Haftalık Disiplin, Ay Boyu
- Mod bazlı: Takipçi, Takip Efsanesi, Mikro Kahraman, Flick Kralı, Çift Nişancı
- Toplam skor bazlı: Bin Vuruş, On Bin Vuruş
- Kusursuzluk: Kusursuz, Grid Ustası
- Zaman bazlı: Gece Kuşu, Erken Kuş
- Koleksiyoncu: Her Şeyi Denedim

**📈 Haftalık/Aylık Rapor Sayfası:**
- Detaylı antrenman analizi
- Mod bazlı performans grafikleri
- Son 30 günlük aktivite grafiği
- Otomatik zaman aralığı seçimi (Hafta/Ay/Tüm Zamanlar)

**🎨 3 Yeni Tema (Toplam 13):**
- **Cyberpunk** — Neon sarı/mavi, distopik hava
- **Rose Pine** — Yumuşak pembe/eflatun, göz dostu
- **GitHub Dark** — Klasik GitHub koyu teması

---

## 💻 Kurulum

### 🚀 Hızlı Kurulum (Önerilen)

1. **Releases sayfasından** son sürümü indir
2. `CHIZ_Game_Hub_Setup.exe` dosyasına **çift tıkla**
3. Windows **yönetici izni** isteyecek → **Evet** de
4. **İleri → İleri → Kur → Bitir**
5. Masaüstündeki **CHIZ Game Hub** kısayoluna çift tıkla

**Kurulum boyutu:** ~47 MB  
**Disk kullanımı:** ~150 MB (Ollama ile ~5 GB)

### 📋 Sistem Gereksinimleri

| | Minimum | Önerilen |
|---|---------|----------|
| **OS** | Windows 10 (64-bit) | Windows 11 |
| **RAM** | 4 GB | 8 GB+ |
| **Disk** | 150 MB | 5 GB (AI Koç için) |
| **CPU** | Herhangi bir modern CPU | 4+ çekirdek |

### 🔧 Kaynaktan Çalıştırma

```bash
# 1. Repoyu klonla
git clone https://github.com/Chiz121/chiz-game-hub.git
cd chiz-game-hub

# 2. Sanal ortam oluştur
python -m venv .venv
.venv\Scripts\activate

# 3. Bağımlılıkları yükle
pip install -r requirements.txt

# 4. Çalıştır
python main.py
chiz-game-hub/
├── main.py                 # Giriş noktası
├── chiz.spec               # PyInstaller yapılandırması
├── build.bat               # Build scripti
├── requirements.txt        # Bağımlılıklar
│
├── assets/                 # İkonlar, görseller
│   ├── app.ico
│   ├── logo.png
│   └── presentmon/         # PresentMon.exe
│
└── app/                    # Ana uygulama
    ├── main_window.py      # Ana pencere
    ├── config.py           # Sabitler
    ├── storage.py          # Veri yönetimi
    ├── theme.py            # Temalar (13 adet)
    ├── reports.py          # Rapor analiz motoru  ← 🆕
    ├── i18n.py             # Çoklu dil
    ├── updater.py          # Otomatik güncelleme
    ├── presentmon.py       # FPS ölçümü
    ├── ollama_installer.py # AI kurulumu
    ├── sounds.py           # Ses efektleri
    ├── streak.py           # Streak sistemi
    ├── achievements.py     # Başarılar (36 adet)
    ├── ai_bot.py           # AI rakip
    ├── ai_coach.py         # AI koç
    ├── stress_test.py      # Stres testi
    ├── diskinfo.py         # Disk bilgisi
    ├── netutil.py          # Ağ araçları
    ├── sysinfo.py          # Sistem bilgisi
    ├── benchmark.py        # Benchmark
    ├── hotkeys.py          # Kısayollar
    ├── discord_rpc.py      # Discord
    ├── launcher_core.py    # Program başlatma
    ├── screen_recorder.py  # Ekran kaydı
    │
    └── widgets/            # Arayüz bileşenleri
        ├── common.py
        ├── splash_screen.py
        ├── help_overlay.py
        ├── notification_center.py
        ├── aim_canvas.py   # Aim antrenman alanı (16 mod)
        ├── page_reports.py # Rapor sayfası  ← 🆕
        ├── ... (35+ dosya)
        └── page_*.py       # Sayfalar
        🛠️ Teknolojiler
Python 3.11+ — Ana dil

PySide6 (Qt6) — Arayüz

PyInstaller — Paketleme

PresentMon — FPS ölçümü

Ollama — Yerel LLM (AI Koç için)

psutil — Sistem bilgisi

GPUtil — GPU bilgisi
🤝 Katkıda Bulunma
Katkılarınızı bekliyoruz! 🎉

Fork'la

Feature branch oluştur (git checkout -b feature/yeni-ozellik)

Commit'le (git commit -m 'Yeni özellik eklendi')

Push'la (git push origin feature/yeni-ozellik)

Pull Request aç
🐛 Hata Bildirimi
Issues sayfasından bildirebilirsiniz.
📄 Lisans
Bu proje MIT Lisansı altında lisanslanmıştır. Detaylar için LICENSE dosyasına bakın.
💝 Teşekkürler
Intel — PresentMon için

Ollama — Yerel LLM için

Qt Project — PySide6 için

Ve sana — bu uygulamayı kullandığın için ❤️
⭐ Beğendin mi?
Bu projeyi faydalı bulduysan yıldız vermeyi unutma! ⭐
