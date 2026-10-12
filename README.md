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

Stránka je statická, stačí ji servírovat přes GitHub Pages:

1. V repozitáři otevřete **Settings → Pages**.
2. V části **Build and deployment** zvolte **Source: Deploy from a branch**, vyberte větev
   s tímto souborem `index.html` a složku `/ (root)`, pak **Save**.
3. Po 1–2 minutách stránka poběží na `https://<uživatel>.github.io/<repozitář>/`
   (zde `https://tomasraketak.github.io/QRcodetest/`).
