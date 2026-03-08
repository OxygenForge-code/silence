# SESSİZLİK 🔇

> **"Sesin senin düşmanın."**

Tarayıcı tabanlı, mikrofon kontrollü psikolojik korku deneyimi. 
Fısıldarsan duyar, bağırırsan koşar, sessizsen... bekler.

---

## 🎮 Oynanış

### Temel Mekanikler

| Eylem | Sonuç |
|-------|-------|
| **Sessizlik** (< 5dB) | Yaratık uzaklaşır/gezinir |
| **Fısıltı** (5-15dB) | Yavaş yaklaşır, meraklanır |
| **Normal Konuşma** (15-35dB) | Yönünü bulur, takibe başlar |
| **Bağırma** (35-60dB) | Koşarak yaklaşır |
| **Çığlık** (> 60dB) | Anında saldırı |

### Kontroller

- **Mouse**: Bakış açısı + El feneri
- **W / S**: İleri / Geri hareket
- **Kulaklık**: 🎧 **ZORUNLU**

---

## 🏗️ Teknik Mimarisi

### Ses Analizi Motoru

```javascript
// Ağırlıklı RMS hesaplama
// Düşük frekanslara ağırlık verir (insan sesi/inşaat)
const weight = 1 / (1 + frequencyIndex * 0.01);
