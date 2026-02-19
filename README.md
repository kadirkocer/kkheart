# kkheart

Static `index.html` sitesi Cloudflare Pages ile GitHub entegrasyonu kullanılarak deploy edilecek şekilde ayarlandı.

## Proje ayarı

- Cloudflare build command: `(boş bırak)`
- Build output directory: `.`
- Root directory: `/` (repo root)

Bu ayarlar için repoda `wrangler.toml` dosyası eklendi.

## Cloudflare Pages kurulumu

1. Cloudflare Dashboard -> `Workers & Pages` -> `Create application` -> `Pages` -> `Connect to Git`.
2. Bu GitHub reposunu seç.
3. Build ayarlarında:
   - Framework preset: `None`
   - Build command: boş
   - Build output directory: `.`
4. Deploy et.

## Custom domain

1. Pages projesi içinde `Custom domains` bölümüne gir.
2. `zeynep.kadirkocer.com` domainini ekle.
3. DNS Cloudflare zone içinde ise kayıt otomatik oluşur; değilse verilen CNAME hedefini DNS sağlayıcına ekle.
4. SSL aktif olduktan sonra site `https://zeynep.kadirkocer.com` üzerinden açılır.
