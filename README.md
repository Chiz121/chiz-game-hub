<!-- Logo ve Başlık -->
<div align="center">

<img src="https://raw.githubusercontent.com/Chiz121/chiz-game-hub/main/assets/logo.png" alt="CHIZ Game Hub" width="180" height="180">

# 🎯 CHIZ Game Hub

**FPS oyuncuları için yerel, ücretsiz ve profesyonel antrenman uygulaması.**

[![Windows](https://img.shields.io/badge/Windows-10%2F11-blue?style=for-the-badge&logo=windows)](https://www.microsoft.com/windows)
[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![PySide6](https://img.shields.io/badge/PySide6-Qt%206-green?style=for-the-badge&logo=qt)](https://doc.qt.io/qtforpython/)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)
[![Version](https://img.shields.io/badge/Version-1.1.0-orange?style=for-the-badge)](https://github.com/Chiz121/chiz-game-hub/releases/latest)
[![Download](https://img.shields.io/badge/İndir-Download-red?style=for-the-badge&logo=github)](https://github.com/Chiz121/chiz-game-hub/releases/latest)

---

[🚀 İndir](#-i̇ndirme) • [✨ Özellikler](#-özellikler) • [💻 Kurulum](#-kurulum) • [🛠️ Teknolojiler](#-kullanılan-teknolojiler)

</div>

---

## 🎯 Nedir Bu?

**CHIZ Game Hub**, FPS oyuncuları için tasarlanmış, **tamamen yerel** ve **ücretsiz** bir antrenman uygulamasıdır. Aim becerilerini geliştirmekten sistem performansını analiz etmeye kadar her şey tek bir yerde.

Counter-Strike 1.6'dan bugüne FPS oyunları oynayan biri olarak (Valorant, CS2 gibi oyunlarda üst düzey), bu uygulamayı **hem kendim hem de benim gibi düşünen oyuncular için** geliştirdim.

> 💡 **%100 Yerel** — Hiçbir verin dışarı gitmez. İnternet gerekmez. Reklam yok, abonelik yok.

---

## ✨ Özellikler

### 🎯 Antrenman
- **11 Aim Modu** — Reaction, Flick, Click, Tracking, Precision, Gridshot, Microshot, Micro Flick, Switching, Strafing, Moving Grid, Track+Strafe
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

### 🎨 Kişiselleştirme
- **7 Tema** — Dark, Midnight, Light, Nord, Dracula, Solarized, Tokyo Night
- **🎨 Özel Accent Rengi** — Kendi rengini seç
- **🌐 5 Dil** — Türkçe, İngilizce, Almanca, Rusça, İspanyolca
- **⏰ Otomatik Tema** — Saate göre gündüz/gece

### 🎮 Overlay'ler
- **Crosshair** — Click-through, tamamen özelleştirilebilir
- **Performance HUD** — CPU/RAM/GPU/Ping + oyun FPS'i
- **Saat**, **Timer**, **FPS Counter**
- **Çoklu Monitör** desteği

### 🏆 Diğer
- **22+ Başarı** — İlerlemeni oyunlaştır
- **Kullanıcı Profilleri** — Birden fazla hesap
- **Game Launcher** — Programlarını tek yerden başlat
- **Game Profiles** — Grup halinde başlat (Valorant + Discord + OBS)
- **Otomatik Güncelleme** — Yeni sürümler otomatik bildirilir

---

## 💻 Kurulum

### 🚀 Hızlı Kurulum (Önerilen)

1. **[Releases sayfasından](https://github.com/Chiz121/chiz-game-hub/releases/latest)** son sürümü indir
2. `CHIZ_Game_Hub_Setup.exe` dosyasına **çift tıkla**
3. Windows **yönetici izni** isteyecek → **Evet** de
4. **İleri → İleri → Kur → Bitir**
5. Masaüstündeki **CHIZ Game Hub** kısayoluna çift tıkla

**Kurulum boyutu:** ~47 MB
**Disk kullanımı:** ~150 MB (Ollama ile ~5 GB)

### 📋 Sistem Gereksinimleri

| | Minimum | Önerilen |
|---|---|---|
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
    ├── theme.py            # Temalar
    ├── i18n.py             # Çoklu dil
    ├── updater.py          # Otomatik güncelleme
    ├── presentmon.py       # FPS ölçümü
    ├── ollama_installer.py # AI kurulumu
    ├── sounds.py           # Ses efektleri
    ├── streak.py           # Streak sistemi
    ├── achievements.py     # Başarılar
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
    │
    └── widgets/            # Arayüz bileşenleri
        ├── common.py
        ├── splash_screen.py
        ├── help_overlay.py
        ├── notification_center.py
        ├── ... (30+ dosya)
        └── page_*.py       # Sayfalar
        🤝 Katkıda Bulunma
Katkılarınızı bekliyoruz! 🎉

Fork'la (https://github.com/Chiz121/chiz-game-hub/fork)

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

⬆ Başa Dön


