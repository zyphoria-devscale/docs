# Domain

- Kita bisa pakai custom domain untuk project BE dan FE

## 1. Beli Domain
- Untuk domain bisa beli di website seperti [Namecheap](https://www.namecheap.com/), [Domainesia](https://www.domainesia.com/), dll

## 2. Register Domain ke Cloudflare DNS
- Masuk ke [Cloudflare](https://dash.cloudflare.com/)
- Lalu klik `+ Add`, pilih `Connect a domain`

![Clean-Shot-2025-06-02-at-18-14-40-2x](https://i.ibb.co/dwtKJJ5X/Clean-Shot-2025-06-02-at-18-14-40-2x.png)

## 3. Pilih Cloudflare Plan
- Pilih plan yang sesuai dengan kebutuhan

![Clean-Shot-2025-06-02-at-18-21-21-2x](https://i.ibb.co/tM5WwrtS/Clean-Shot-2025-06-02-at-18-21-21-2x.png)

## 4. DNS Record
- Selanjutnya akan masuk ke halaman DNS Record

![Clean-Shot-2025-06-02-at-18-22-17-2x](https://i.ibb.co/fdKm8Rsr/Clean-Shot-2025-06-02-at-18-22-17-2x.png)

- Masukkan dns record untuk root domain (cth: `milhamh.com`)
- IPv4 address mengarah ke IP server Front End / Back End. Silahkan cek vps / server FE dan BE untuk mendapatkan IP Address.

![Clean-Shot-2025-06-02-at-18-29-07-2x](https://i.ibb.co/0jYTGBFH/Clean-Shot-2025-06-02-at-18-29-07-2x.png)

- Masukkan dns record untuk www (cth: `www.milhamh.com`)
- IPv4 address mengarah ke IP server Front End / Back End. Silahkan cek vps / server FE dan BE untuk mendapatkan IP Address.

![Clean-Shot-2025-06-02-at-18-29-27-2x](https://i.ibb.co/VWW77ct4/Clean-Shot-2025-06-02-at-18-29-27-2x.png)

## 5. Register Nameserver

- Lalu register nameserver cloudflare ke domain provider
- Kalau cloud flare pakai nameserver

```
asa.ns.cloudflare.com
jaime.ns.cloudflare.com
```

![Clean-Shot-2025-06-02-at-18-30-00-2x](https://i.ibb.co/RG101X6r/Clean-Shot-2025-06-02-at-18-30-00-2x.png)

![Clean-Shot-2025-06-02-at-18-32-58-2x](https://i.ibb.co/p6N8LbV2/Clean-Shot-2025-06-02-at-18-32-58-2x.png)

- Tunggu beberapa saat (max: 24 jam), status domain akan active di cloudflare

![Clean-Shot-2025-06-02-at-18-34-57-2x](https://i.ibb.co/ymXgydzk/Clean-Shot-2025-06-02-at-18-34-57-2x.png)

## Note
- ini hanya sebagai contoh saja
- cloudflare tidak hanya memiliki layanan dns, tapi memiliki layanan untuk beli domain. jadi bisa cukup beli dan setting dns di cloudflare. 
- Platform yang lain juga sama seperti netlify, vercel, dll