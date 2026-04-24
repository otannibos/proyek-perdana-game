# PROJECT REQUIREMENT DOCUMENT (PRD)
## Fishing Survival: Skill & Level System

---

## 1. Ringkasan Produk
Game memancing berbasis web dengan fokus pada refleks, kontrol pemain, dan sistem level berbasis skill. Game dirancang sebagai arcade sederhana dengan tekanan waktu dan progression.

---

## 2. Tujuan Produk
### Tujuan Utama
- Memberikan gameplay cepat, menantang, dan adiktif

### Tujuan Teknis
- Melatih:
  - Animasi DOM
  - Game loop
  - Collision detection
  - State management

---

## 3. Target User
- Pelajar / pemula coding
- Casual gamer
- User dengan waktu bermain singkat (1–3 menit)

---

## 4. Core Gameplay Loop
1. Player klik → kail turun
2. Kail masuk air → splash
3. Player menggerakkan kail
4. Ikan bergerak dinamis
5. Player mencoba menangkap ikan
6. Skor bertambah jika berhasil
7. Ulangi hingga waktu habis

---

## 5. Core Mechanics
### Kontrol
- Klik: lempar kail
- Arrow kiri/kanan: gerakkan kail

### Sistem Ikan
- Bergerak kiri ↔ kanan
- Memantul di batas layar
- Spawn berkala
- Kecepatan meningkat sesuai level

### Collision
- Menggunakan bounding box
- Tabrakan = ikan tertangkap

### Sistem Waktu
- Waktu awal: 20 detik
- Berkurang tiap detik
- Game over saat waktu habis

### Sistem Skor
- +1 per ikan
- Tidak ada skor jika miss

---

## 6. Sistem Level
### Aturan
- 20 ikan → naik level
- Maks level: 5

### Distribusi Ikan
- Level 1: Gabus
- Level 2: Lele
- Level 3: Toman
- Level 4: Nila
- Level 5: Emas

### Scaling Difficulty
- Kecepatan ikan meningkat tiap level

### Reward
- +5 detik saat level up
- Reset skor ke 0

---

## 7. Visual & UI
### Elemen
- Background desa
- Air
- Kapal
- Kail
- Ikan
- Splash effect

### HUD
- Level
- Progress ikan
- Waktu
- Notifikasi (hit/miss/level up)

---

## 8. Animasi
- Kail: transition naik/turun
- Ikan: gerakan real-time
- Splash: efek cepat

---

## 9. Game State
- Idle
- Casting
- Aiming
- Catch Check
- Result
- Level Up
- Game Over

---

## 10. Edge Cases
- Spam klik
- Kail keluar layar
- Banyak ikan aktif
- Double collision

---

## 11. KPI
- Player mencapai minimal level 2
- Gameplay mudah dipahami
- Performa stabil
- Player replay minimal 2 kali

---

## 12. Teknologi
- HTML
- CSS
- JavaScript (Vanilla)

---

## 13. Future Development
### Gameplay
- Hitbox berbeda
- Rare fish
- Combo system

### Visual
- Sprite ikan
- Animasi air
- Sound effect

### Progression
- Upgrade alat
- Endless mode
- Boss fish

---

## 14. Risiko
- Terlalu sulit
- Repetitif
- Visual sederhana

---

## 15. Estimasi Development
- Core: 1–2 hari
- Animasi: 1 hari
- Level system: 1 hari
- Polishing: 1–2 hari

---

## Kesimpulan
Prototype game arcade berbasis skill dengan sistem progression sederhana namun scalable.