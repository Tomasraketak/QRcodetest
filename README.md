# QR Security Demo

Edukativní demo stránka k prezentaci o AI bezpečnosti a **quishingu** (phishing přes QR kódy).

Návštěvník naskenuje QR kód a stránka mu okamžitě ukáže, co o něm zjistí jakákoli webová
stránka bez jeho povolení: veřejnou IP adresu a přibližnou polohu, operační systém,
prohlížeč, typ zařízení, displej, jazyk, časové pásmo, typ připojení, baterii a hardware.

- Jeden soubor `index.html`, bez frameworků, vše inline.
- Žádné cookies, localStorage, analytika, trackery ani backend.
- Jediné externí volání je `https://ipwho.is/` přímo z prohlížeče návštěvníka.
- Nic se neukládá ani neodesílá na server autora.

QR kód s odkazem na stránku je v `assets/qr.png` a `assets/qr.svg`.

## Nasazení

1. Pushněte repozitář na GitHub (větev `main`).
2. Zapněte GitHub Pages z větve `main`, složka `/` (root):
   ```sh
   gh api -X POST repos/<uživatel>/qr-security-demo/pages \
     -f "source[branch]=main" -f "source[path]=/"
   ```
3. Stránka poběží na `https://<uživatel>.github.io/qr-security-demo/`.
