# Background Music

Taro file lagu di folder ini dengan nama:

- `everything-you-are.mp3` (utama), atau
- `everything-you-are.m4a` (fallback)

Kalo file-nya belum ada, tombol vinyl di pojok kiri bawah tetap muncul, tapi audio-nya ga bakal jalan (silently fail).

## Dari mana dapetin file-nya?

Lagu "Everything You Are" - Hindia bisa didapat dari:
- Beli/rip dari sumber legal (Spotify → convert via yt-dlp dari YouTube resmi, dsb)
- Cari file mp3 yang lo udah punya di iTunes/library

## Kompresi (opsional)

Biar loading cepet, compress dulu ke bitrate 128kbps:

```bash
ffmpeg -i input.mp3 -b:a 128k everything-you-are.mp3
```

Target size < 4 MB idealnya.
