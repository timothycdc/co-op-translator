<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "d238206c3503631e32774716d11d1868",
  "translation_date": "2025-05-07T14:15:23+00:00",
  "source_file": "getting_started/command-line-guide/translator-your-project.md",
  "language_code": "id"
}
-->
# Translate your project using Co-op Translator

**Co-op Translator** adalah alat command-line interface (CLI) yang membantu Anda menerjemahkan file markdown dan gambar dalam proyek Anda ke berbagai bahasa. Bagian ini menjelaskan cara menggunakan alat ini, mencakup berbagai opsi CLI, dan memberikan contoh untuk berbagai kasus penggunaan.

> [!NOTE]
> Untuk daftar lengkap perintah dan deskripsi detailnya, silakan lihat [Command reference](./command-reference.md).

---

## Contoh Skenario dan Perintah

Berikut beberapa kasus penggunaan umum untuk **Co-op Translator**, beserta perintah yang sesuai untuk dijalankan.

### 1. Terjemahan Dasar (Satu Bahasa)

Untuk menerjemahkan seluruh proyek Anda (file markdown dan gambar) ke satu bahasa, seperti Korea, gunakan perintah berikut:

```bash
translate -l "ko"
```

Perintah ini akan menerjemahkan semua file markdown dan gambar ke bahasa Korea, menambahkan terjemahan baru tanpa menghapus yang sudah ada.

> [!TIP]
>
> Ingin tahu kode bahasa apa saja yang tersedia di **Co-op Translator**? Kunjungi bagian [Supported Languages](https://github.com/Azure/co-op-translator#supported-languages) di repositori untuk informasi lebih lanjut.

#### Contoh pada Phi-3 CookBook

Di **Phi-3 CookBook**, saya menggunakan metode berikut untuk menambahkan terjemahan bahasa Korea pada file markdown dan gambar yang sudah ada.

```bash
(.venv) C:\Users\sms79\dev\Phi-3CookBook>translate -l"ko"
Translating images: 100%|███████████████████████████████████████████████████| 276/276 [1:09:56<00:00, 15.37s/it]
Translating markdown files: 100%|████████████████████████████████████████████████| 153/153 [1:43:07<00:00, 241.31s/it]
```

### 2. Menerjemahkan Beberapa Bahasa

Untuk menerjemahkan proyek Anda ke beberapa bahasa sekaligus (misalnya Spanyol, Prancis, dan Jerman), gunakan perintah ini:

```bash
translate -l "es fr de"
```

Perintah ini akan menerjemahkan proyek ke bahasa Spanyol, Prancis, dan Jerman, menambahkan terjemahan baru tanpa menimpa yang sudah ada.

#### Contoh pada Phi-3 CookBook

Di **Phi-3 CookBook**, setelah menarik perubahan terbaru untuk mencerminkan commit terkini, saya menggunakan metode berikut untuk menerjemahkan file markdown dan gambar yang baru ditambahkan.

```bash
(.venv) C:\Users\sms79\dev\Phi-3CookBook>translate -l"ko ja zh tw es fr" -a
Translating images: 100%|███████████████████████████████████████████████████| 273/273 [1:09:56<00:00, 15.37s/it]
Translating markdown files: 100%|████████████████████████████████████████████████| 6/6 [24:07<00:00, 241.31s/it]
```

> [!NOTE]
> Meskipun umumnya disarankan menerjemahkan satu bahasa sekaligus, dalam situasi seperti ini di mana perubahan spesifik perlu ditambahkan, menerjemahkan beberapa bahasa sekaligus bisa lebih efisien.

### 3. Memperbarui Terjemahan (Menghapus Terjemahan Lama)

Untuk memperbarui terjemahan yang sudah ada (yaitu menghapus terjemahan saat ini dan menggantinya dengan yang baru), gunakan opsi `-u`. Ini akan menghapus semua terjemahan lama untuk bahasa yang ditentukan dan menerjemahkannya ulang.

```bash
translate -l "ko" -u
```

Peringatan: Perintah ini akan meminta konfirmasi sebelum melanjutkan penghapusan terjemahan yang ada.

#### Contoh pada Phi-3 CookBook

Di **Phi-3 CookBook**, saya menggunakan metode berikut untuk memperbarui semua file terjemahan dalam bahasa Spanyol. Saya sarankan menggunakan metode ini saat ada perubahan signifikan pada konten asli di beberapa dokumen markdown. Jika hanya ada beberapa file terjemahan markdown yang perlu diperbarui, akan lebih efisien menghapus file tersebut secara manual lalu menggunakan metode `-a` untuk menambahkan terjemahan yang diperbarui.

```bash
(.venv) C:\Users\sms79\dev\Phi-3CookBook>translate -l "es" -u
Warning: The update command will delete all existing translations for 'es' and re-translate everything.
Do you want to continue? Type 'yes' to proceed: yes
Proceeding with update...
Translating images: 100%|████████████████████████████████████████████| 150/150 [43:46<00:00, 15.55s/it]
Translating markdown files: 100%|███████████████████████████████████| 95/95 [1:40:27<00:00, 125.62s/it]
```

### 5. Menerjemahkan Hanya Gambar

Untuk menerjemahkan hanya file gambar dalam proyek Anda, gunakan opsi `-img`:

```bash
translate -l "ko" -img
```

Perintah ini hanya akan menerjemahkan gambar ke bahasa Korea, tanpa memengaruhi file markdown.

### 6. Menerjemahkan Hanya File Markdown

Untuk menerjemahkan hanya file markdown dalam proyek Anda, gunakan opsi `-md`:

```bash
translate -l "ko" -md
```

### 7. Memeriksa Kesalahan pada File Terjemahan

Jika Anda ingin memeriksa file terjemahan untuk kesalahan dan mencoba ulang penerjemahan jika perlu, gunakan opsi `-chk`:

```bash
translate -l "ko" -chk
```

Perintah ini akan memindai file markdown terjemahan dan mencoba ulang penerjemahan untuk file yang bermasalah.

#### Contoh pada Phi-3 CookBook

Di **Phi-3 CookBook**, saya menggunakan metode berikut untuk memeriksa kesalahan terjemahan pada file bahasa Korea dan secara otomatis mencoba ulang penerjemahan untuk file yang ditemukan masalah.

```bash
(.venv) C:\Users\sms79\dev\Phi-3CookBook>translate -l"ko" -chk 
Checking translated files for errors in ko...
Checking files for ko: 100%|██████████████████████████████████████████████████| 95/95 [00:01<00:00, 65.47file/s]
Retrying vsc-extension-quickstart.md for ko:   0%|                                     | 0/17 [00:00<?, ?file/s] 
```

Opsi ini memeriksa kesalahan terjemahan. Saat ini, jika perbedaan jumlah pemisah baris antara file asli dan terjemahan lebih dari enam, file tersebut ditandai mengalami kesalahan terjemahan. Saya berencana meningkatkan kriteria ini agar lebih fleksibel di masa depan.

Misalnya, metode ini berguna untuk mendeteksi bagian yang hilang atau terjemahan yang rusak, dan secara otomatis mencoba ulang penerjemahan untuk file-file tersebut.

Namun, jika Anda sudah tahu file mana yang bermasalah, lebih efisien menghapus file tersebut secara manual lalu menggunakan opsi `-a` option to re-translate them.

### 8. Debug Mode

To enable detailed logging for troubleshooting, use the `-d`:

```bash
translate -l "ko" -d
```

Perintah ini menjalankan penerjemahan dalam mode debug, memberikan informasi log tambahan yang dapat membantu Anda mengidentifikasi masalah selama proses penerjemahan.

#### Contoh pada Phi-3 CookBook

Di **Phi-3 CookBook**, saya mengalami masalah di mana terjemahan dengan banyak tautan dalam file markdown menyebabkan kesalahan format, seperti terjemahan yang rusak dan pemisah baris yang diabaikan. Untuk mendiagnosis masalah ini, saya menggunakan opsi `-d` untuk melihat bagaimana proses penerjemahan berjalan.

```bash
(.venv) C:\Users\sms79\dev\Phi-3CookBook>translate -l "ko" -d
DEBUG:openai._base_client:Request options: {'method': 'post', 'url': '/chat/completions', 'headers': {'api-key': 'af04e0bea45747d8a7b8c131c1971044'}, 'files': None, 'json_data': {'messages': [{'role': 'user', 'content': "Translate the following text to ko. NEVER ADD ANY EXTRA CONTENT OUTSIDE THE TRANSLATION. TRANSLATE ONLY WHAT IS GIVEN TO YOU.. MAINTAIN MARKDOWN FORMAT\n\n# Phi-3 Cookbook: Hands-On Examples with Microsoft's Phi-3 Models [![Open and use the samples in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/microsoft/phi-3cookbook) [![Open in Dev Containers](https://img.shields.io/static/v1?style=for-the-badge&label=Dev%
...
```

### 9. Menerjemahkan Semua Bahasa

Jika Anda ingin menerjemahkan proyek ke semua bahasa yang didukung, gunakan kata kunci all.

> [!WARNING]
> Menerjemahkan semua bahasa sekaligus dapat memakan waktu cukup lama tergantung ukuran proyek. Misalnya, menerjemahkan **Phi-3 CookBook** ke bahasa Spanyol memakan waktu sekitar 2 jam. Mengingat skala tersebut, tidak praktis satu orang mengelola 20 bahasa. Disarankan untuk membagi pekerjaan ke beberapa kontributor, masing-masing mengelola satu atau dua bahasa, dan memperbarui terjemahan secara bertahap.

```bash
translate -l "all"
```

Perintah ini akan menerjemahkan proyek ke semua bahasa yang tersedia. Jika Anda melanjutkan, proses terjemahan mungkin memakan waktu cukup lama tergantung ukuran proyek.

> [!TIP]
>
> ### Menghapus File Terjemahan Secara Manual (Opsional)
> File terjemahan sekarang secara otomatis terdeteksi dan dibersihkan saat file sumber diperbarui.
>
> Namun, jika Anda ingin memperbarui terjemahan secara manual - misalnya, untuk mengulang file tertentu atau menimpa perilaku sistem - Anda bisa menggunakan perintah berikut untuk menghapus semua versi file tersebut di folder bahasa.
>
> ### Di Windows:
> 1. **Menggunakan Command Prompt**:
>    - Buka Command Prompt.
>    - Arahkan ke folder tempat file berada menggunakan perintah `cd`.
>    - Gunakan perintah berikut untuk menghapus file:
>      ```
>      del /s *filename*
>      ```
>      Opsi `/s` mencari juga di subdirektori.
>
> 2. **Menggunakan PowerShell**:
>    - Buka PowerShell.
>    - Jalankan perintah ini:
>      ```powershell
>      Get-ChildItem -Path "C:\YourPath" -Filter "*filename*" -Recurse | Remove-Item -Force
>      ```
>      Ganti `"C:\YourPath"` dengan path Anda.
>
> 3. Gunakan perintah `cd` dan `find` untuk menemukan file:
>     ```bash
>     find . -type f -name "*filename*" -delete
>     ```
> 4. Gunakan perintah `translate -l` untuk memperbarui perubahan file terbaru.

**Penafian**:  
Dokumen ini telah diterjemahkan menggunakan layanan terjemahan AI [Co-op Translator](https://github.com/Azure/co-op-translator). Meskipun kami berusaha untuk akurasi, harap diingat bahwa terjemahan otomatis mungkin mengandung kesalahan atau ketidakakuratan. Dokumen asli dalam bahasa aslinya harus dianggap sebagai sumber yang sahih. Untuk informasi yang penting, disarankan menggunakan terjemahan profesional oleh manusia. Kami tidak bertanggung jawab atas kesalahpahaman atau salah tafsir yang timbul dari penggunaan terjemahan ini.