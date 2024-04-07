# GPTInternetGratis


> Menjalankan aplikasi www.perplexity.ai sepenuhnya GRATIS, LOKAL, PRIVAT, dan TIDAK MEMERLUKAN GPU pada setiap komputer.


> [!IMPORTANT]  
> Jika Anda tidak dapat menggunakan proyek ini secara normal, kemungkinan besar disebabkan oleh masalah koneksi internet atau IP Anda, Anda memerlukan koneksi internet gratis untuk menggunakan proyek ini secara normal.
> 
## Apa itu GPTInternetGratis
GPTInternetGratis adalah agregator pencarian & pembangkit jawaban sepenuhnya gratis, privat, dan berjalan secara lokal menggunakan LLM, Tanpa Memerlukan GPU. Pengguna dapat bertanya dan sistem akan menggunakan searxng untuk melakukan pencarian multi mesin dan menggabungkan hasil pencarian ke ChatGPT3.5 LLM dan menghasilkan jawaban berdasarkan hasil pencarian. Seluruh proses berjalan secara lokal dan Tidak Memerlukan GPU atau kunci API OpenAI atau Google.

## Features 

- 🈚️ Benar-benar GRATIS (tidak perlu kunci API apa pun)
- 💻 Benar-benar LOKAL (tidak perlu GPU, setiap komputer dapat menjalankannya)
- 🔐 Benar-benar PRIVAT (semua hal berjalan secara lokal)
- 👻 Berjalan TANPA Perangkat LLM (TIDAK MEMERLUKAN GPU!)
- 🤩 Menggunakan Free ChatGPT3.5 API (TIDAK MEMERLUKAN kunci API! Terima kasih kepada OpenAI)
- 🚀 Cepat dan mudah diimplementasikan dengan Docker Compose
- 🌐 Antarmuka ramah Web dan Mobile, memungkinkan akses mudah dari setiap perangkat (Terima kasih ChatGPT-Next-Web)

## Bagaimana Cara Kerjanya?

1. Sistem mendapatkan pertanyaan input pengguna di ChatGPT-Next-Web (berjalan secara lokal), dan memanggil searxng (berjalan secara lokal) untuk melakukan pencarian di berbagai mesin pencari.
2. Mengumpulkan konten tautan hasil pencarian dan meneruskannya ke ChatGPT3.5 (menggunakan OpenAI ChatGPT3.5, melalui FreeGPT35 yang berjalan secara lokal), meminta ChatGPT3.5 untuk menjawab pertanyaan pengguna berdasarkan konten ini sebagai referensi.
3. Mengalirkan jawaban ke Antarmuka Obrolan ChatGPT-Next-Web.

## Status 

Proyek ini masih dalam tahap awal. Harap bersiap untuk beberapa bug.


### Jalankan rilis terbaru

```bash
git clone https://github.com/nashsu/FreeAskInternet.git
cd ./FreeAskInternet
docker-compose up -d 
```
🎉 Sekarang Anda seharusnya dapat membuka antarmuka web di http://localhost:3000. Tidak ada yang lain yang terpapar secara default.

### Cara Memperbarui ke yang Terbaru

```bash
cd ./FreeAskInternet
git pull
docker compose rm backend
docker image rm nashsu/free_ask_internet
docker-compose up -d
```

## Credits
- ChatGPT-Next-Web : [https://github.com/ChatGPTNextWeb/ChatGPT-Next-Web](https://github.com/ChatGPTNextWeb/ChatGPT-Next-Web)
- FreeGPT35: [https://github.com/missuo/FreeGPT35](https://github.com/missuo/FreeGPT35)
- searxng: [https://github.com/searxng/searxng](https://github.com/searxng/searxng)

## License
Apache-2.0 license

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=nashsu/FreeAskInternet&type=Date)](https://star-history.com/#nashsu/FreeAskInternet&Date)
