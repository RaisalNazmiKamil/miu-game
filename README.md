# PETUALANGAN MIU

Kumpulan empat mini-game browser original tentang Miu, si kucing oren. Dibuat dengan HTML5 Canvas, CSS3, dan JavaScript vanilla, tanpa backend atau dependensi.

## Menjalankan

Buka `index.html` langsung di browser modern. Tidak memerlukan server, npm, atau instalasi.

## Permainan

- **Miu Adventure**: platformer satu level, kumpulkan ikan, injak Si Landak, dan capai bendera akhir.
- **Miu Endless Run**: lompati rintangan yang makin cepat sambil mengumpulkan ikan.
- **Miu Catch Fish**: tangkap ikan selama 60 detik dan hindari kaleng atau sepatu.
- **Miu Sky Jump**: lompat otomatis dari platform prosedural untuk mencapai tinggi maksimal.

## Kontrol

- Adventure: `A/D` atau panah kiri/kanan, `W`/panah atas/Spasi untuk lompat, `Shift` untuk berlari, `P` untuk jeda.
- Endless Run: Spasi, `W`, atau panah atas untuk lompat.
- Catch Fish dan Sky Jump: `A/D` atau panah kiri/kanan.

## Struktur

```text
index.html          Menu dan area Canvas
style.css           Antarmuka responsif pixel-art inspired
main.js             Lifecycle, input, audio, localStorage, HUD umum
games/              Logika terpisah untuk empat game
assets/miu.png      Sprite utama Miu
assets/backgrounds/ Ruang untuk gambar latar tambahan
assets/objects/     Ruang untuk objek tambahan
assets/sounds/      Ruang untuk audio tambahan
```

## Kustomisasi

- Ganti `assets/miu.png` dengan sprite Miu lain (gunakan PNG transparan, rasio gambar tetap dijaga).
- Tambahkan audio lokal ke `assets/sounds/` lalu sambungkan pada fungsi `Miu.tone` di `main.js`; efek bawaan dibuat melalui Web Audio API.
- Tambah level Adventure dengan memperluas array `plats`, `fish`, dan `enemies` di `games/adventure.js`.

Rekor, pengaturan suara, dan permainan yang dimainkan disimpan lokal di browser menggunakan `localStorage`.
