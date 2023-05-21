# Update Rule Provider OpenClash

Repository ini berisi pembaruan untuk rule provider pada aplikasi OpenClash. Rule provider digunakan untuk mengatur aturan lalu lintas jaringan.

## Cara Menggunakan

1. Buka aplikasi OpenClash.
2. Cari pengaturan rule provider atau aturan aplikasi.
3. Tambahkan URL rule provider yang ingin digunakan, contoh: 
```yaml
type: http
behavior: domain
url: "https://raw.githubusercontent.com/fyn170/open_clash/main/rule_provider/ads.yaml"
path: "./rule_provider/rules.yaml"
health-check:
  enable: true
  url: "http://www.gstatic.com/generate_204"
  interval: 3600
```
5. Simpan pengaturan dan pastikan aplikasi mengunduh aturan terbaru dari rule provider yang ditambahkan.

## Aturan yang Tersedia

Repository ini menyediakan beberapa rule provider yang dapat digunakan dengan OpenClash. Aturan-aturan ini berupa file YAML yang berisi daftar domain atau alamat IP untuk diblokir atau diizinkan.

Daftar rule provider yang tersedia dapat ditemukan di direktori `rule_provider`.


## Credits
- [fyn170](https://github.com/fyn170/open_clash)
- ChatGPT by OpenAI ([openai.com](https://chat.openai.com))
