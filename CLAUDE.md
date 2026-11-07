# CLAUDE.md

Živý dokument. Průběžně aktualizuj, udržuj krátký a přehledný.

## Projekt

* **Název:** Niky's Kitchen (web + blog). Součástí je appka **Jídlo od A–Z**. „Koláč od Niky“ je název receptu, ne značky.
* **Firma:** žádná – osobní projekt a portfolio. Později obchod s digitálními produkty (e-booky, online kuchařka, kurzy; prodej přes FAPI).
* **Popis:** web s recepty (slané, sladké, nápoje), články o výživě a webová appka, která spočítá denní příjem, rozdělí ho do jídel, najde recepty podle ledničky a vytvoří nákupní seznam.
* **Cíl / Vize:** ulehčit lidem zdravé stravování – žádné složité počítání, jasná odpověď na „co mám dnes jíst a kolik“. Web přivádí čtenáře, appka jim pomáhá v praxi, obchod později nabídne placené plány, e-booky a kurzy. Design vždy responzivní.
* **Cílová skupina:** ženy i muži 18+, kteří berou zdravý životní styl jako investici do budoucna, ale nemají moc času a nechtějí nic složitého. Chtějí zhubnout, udržet formu, nebo nabrat svaly. Často aktivní – sport, práce na nohou. Veřejný web.
* **Brand tón:** přátelský, **tykání**, jako rada od kamarádky. Jednoduše, bez odborného žargonu, motivačně, ne moralizující. Žádná nepravdivá tvrzení (falešná hodnocení, zdravotní sliby).
* **Jazyky UI:** celý web i appka česky (primární) a anglicky, později případně další. Texty psát jednoduše a odděleně od kódu, aby šly snadno přeložit. Web má být přívětivý pro co nejvíc lidí, nikoho nevynechat.

## Uživatel

* **Skill level:** mírně pokročilá – zná základy HTML/CSS. Technické věci vysvětluj jednoduše, rozhodnutí navrhuj s doporučením.
* Pracuje v Cursoru (dřív Sublime Text), Windows.

## Stack

* **Nový web (od 2026-10-05):** `niky-web/` – **Next.js 16** (App Router, JavaScript, bez Tailwindu), statický export (`output: "export"`) pro GitHub Pages. Jazyky přes `app/[lang]/` (cs, en), texty v `dictionaries/*.json`. Před psaním kódu čti dokumentaci v `node_modules/next/dist/docs/` (verze se liší od tréninkových dat, viz `niky-web/AGENTS.md`). Spouštění: `docker compose up -d` → http://localhost:3000/cs/
* **Next.js v Dockeru na Windows:** nové soubory dev server občas nezaregistruje → `docker compose restart web`. Obrázky z `public/` v `next/image` přes `asset()` z `lib/asset.js` (kvůli podsložce na hostingu)
* **Starý web a appka:** `nikys-kitchen/` a `jidlo-od-a-z/` – čisté HTML, CSS, JS (běží dál, dokud nebude nový web hotový)
* **Databáze (od 2026-11-07):** PostgreSQL 17 v `niky-web/docker-compose.yml` (+ Adminer na :8081, heslo v `.env`, vzor `.env.example`). Struktura `db/init/01-tabulky.sql`, obsah `db/init/02-data.sql` (nahraje se jen do prázdné databáze), záloha `docker compose exec db sh /db/zaloha.sh`. Web čte přes `lib/db.js` (balík `postgres` v4 – numeric vrací jako text) a `lib/content.js`. Při buildu na GitHubu běží dočasná databáze (služba v `nasazeni.yml`). Appka stahuje `api/appka.json` (pohled `appka_recepty`), záloha `js/data.js`
* **Zatím ne:** přihlášení (Auth.js), živá databáze na internetu (newsletter a obchod potřebují server – např. Supabase)
* **UI:** vlastní CSS, fonty Playfair Display (nadpisy) + Plus Jakarta Sans (text) z Google Fonts (v Next.js přes `next/font`)
* **Data:** recepty a články jen v databázi (web i appka). Uživatelská data appky v `localStorage`.
* **Hosting:** GitHub Pages – appka i nový web (`https://4613nikola-oss.github.io/nikys-kitchen-web/`, nasazuje `.github/workflows/nasazeni.yml` po pushi na `main`, basePath `/nikys-kitchen-web`). Všechny 4 repozitáře jsou veřejné (rozhodnutí Niky 2026-11-07)
* **Commity** se podepisují soukromým e-mailem GitHubu (`…@users.noreply.github.com`, nastaveno globálně)
* **Kontejnerizace:** Docker + nginx (appka), obraz `nikolapaluskova/jidlo-od-a-z` na Docker Hubu

## Pravidla

### Prostředí

* Komunikace v chatu: **česky**, odpovědi dělit podle částí (🌐 Web / 📱 Aplikace / 📄 CLAUDE.md)
* Kód (komentáře, commity): **česky**
* **Všechny příkazy spouštěj jen v Dockeru** (node, npm, npx, python, build, testy, převody souborů). Nic neinstaluj přímo do Windows. Mimo Docker jen `git` a samotný `docker`.
* Node.js ani `gh` na počítači nejsou. Kontrolu JS dělej přes Docker: `docker run --rm -v "<cesta>:/src:ro" node:22-alpine node --check /src/<soubor>.js`
* `docker.exe` není v PATH shellu → `C:\Program Files\Docker\Docker\resources\bin`
* Appka lokálně: ve složce appky `docker compose up -d` → http://localhost:8080 (HTML/CSS/JS se projeví po F5, `nginx.conf`/`Dockerfile` vyžadují `--build`)

### Git a GitHub

* Samostatné repozitáře: nový web, starý web, appka. Kořen `curzor_projekt` = repo **podkladů** (`nikys-kitchen-projekt`, VEŘEJNÝ: CLAUDE.md, PROJEKT.md, podklady/ – jen větev `main`, pushuj po každé změně)
* Větve: **`dev`** = práce, **`main`** = hotové/živé. Po každé hotové změně **commitni a pushni sám na `dev`** a řekni, co se změnilo (uživatelka nechce potvrzovat každý push)
* Do `main` slučuj `dev` jen na pokyn uživatelky („nahraj to“, „pusť to ven“) – `main` u appky = **živý web** na GitHub Pages (nasadí se do minuty)
* Commit zprávy česky, stručné a popisné
* Přihlášení ke GitHubu přes Git Credential Manager (účet `4613nikola-oss`)
* Veřejné zveřejnění (repo → public, Docker Hub push) jen se souhlasem uživatelky

### Testy

* Testovací framework zatím není. Po změně: kontrola syntaxe JS (viz výše) + ověř, že se stránky načtou (HTTP 200)
* Uživatelce vždy řekni, co jsi ověřil a co ne (např. že jsi stránky neproklikal v prohlížeči)

### Mazání

* Nic nemaž bez potvrzení – hlavně originál webu v `OneDrive\Desktop\nikys-kitchen`
* V appce musí mít mazací akce (nákupní seznam, lednička) potvrzení nebo možnost vrátit

### Bezpečnost

* Žádná hesla, tokeny ani osobní údaje v kódu – repozitáře jsou nebo budou veřejné
* Před zveřejněním repozitáře zkontroluj citlivé údaje
* Všechny repozitáře mají `.gitignore` pojistku (hesla, klíče, archivy, složka `soukrome/`). Před každým commitem zkontroluj, co se přidává
* Rizika zapisuj do `security_warnings.md` v kořeni příslušného projektu

### Grafika a UI

* **Primární:** `#3d5233` (tmavě zelená), hover `#2e3e26`
* **Pozadí:** `#f7f5f0` (krémová), karty `#ffffff`, okraje `#e3ded5`
* **Text:** `#2c2c2c`, tlumený `#6b6b6b`, zvýraznění hvězdiček `#f59e0b`
* **Font:** Playfair Display + Plus Jakarta Sans
* **Styl:** přírodní, útulný, „papírové“ karty, zaoblené rohy (~1rem), jemné stíny. Mobil first.

### Vyhledávání

* Pokud si nejsi jistý aktuální verzí, best practice nebo syntaxí, vyhledej na internetu

## Struktura projektu

```
D:\curzor_projekt\
├── CLAUDE.md                 # tento soubor – pravidla pro Clauda
├── PROJEKT.md                # kniha projektu – rozhodnutí, úkoly, nápady (pro uživatelku)
├── podklady\                 # návrhy a podklady (ne rozhodnutí – ta jsou v PROJEKT.md)
│   ├── DASHBOARD.md          #   rozcestník a stav projektu
│   ├── BRAINSTORMING.md      #   průzkum, věda se zdroji, konkurence, koncepty, kalkulačka
│   ├── SITEMAP.md, PERSONY.md, FLOW.md
├── niky-web\                 # 🆕 nový web v Next.js (git: 4613nikola-oss/nikys-kitchen-web, VEŘEJNÝ)
│   ├── app/[lang]/           #   stránky cs/en (recepty/[slug], clanky/[slug]…), layout.js = hlavička, patička, písma
│   ├── db/                   #   databáze: init/01-tabulky.sql, init/02-data.sql, zaloha.sh
│   ├── app/api/appka.json/   #   recepty pro appku (statický JSON z databáze)
│   ├── components/, dictionaries/, lib/ (db, content, i18n, asset), app/globals.css
│   ├── docs/ukazky/          #   screenshoty do README (WebP)
│   ├── assets/maskot/        #   Tečka – nálady a proměny (SVG)
│   └── docker-compose.yml    #   vývoj jen v Dockeru
├── jidlo-od-a-z\             # 📱 appka Jídlo od A–Z (git: 4613nikola-oss/jidlo-od-a-z, VEŘEJNÝ)
│   ├── index.html            #   jediná stránka appky (záložky Profil/Můj den/Lednička/Recepty/Nákup)
│   ├── css/app.css
│   ├── js/app.js             #   logika appky
│   ├── js/data.js            #   recepty + články (zatím ukázková data)
│   ├── manifest.json, ikona.svg   # PWA – přidání na plochu
│   └── Dockerfile, docker-compose.yml, nginx.conf
├── nikys-kitchen\            # 🌐 web a blog (git: 4613nikola-oss/nikys-kitchen, VEŘEJNÝ)
│   ├── index.html, slane.html, sladke.html, napoje.html, clanky.html, galerie.html, o-mne.html
│   ├── clanky/               #   jednotlivé články
│   ├── recepty/              #   detailní recepty
│   ├── css/style.css, js/main.js
│   ├── images/ (písma z Google Fonts)
└── jidlo-od-a-z.zip          # původní export appky (archiv, obsah je v jidlo-od-a-z\)
```

## Postup práce

* Ve fázích: nejdřív základní struktura, pak detaily
* Po každé fázi ukázat výsledek v prohlížeči a počkat na zpětnou vazbu; zadání se smí měnit za pochodu

## Omezení agenta

* Velké změny (nové sekce, přestavba webu) nejdřív krátce popiš a nech schválit
* Drobné opravy chyb dělej rovnou a oznam je

## Nuance projektu

* Odkazy v appce (`../slane.html`, `../clanky.html`) počítají s tím, že appka bude složka uvnitř webu
* Recepty v appce jsou ukázkové – skutečné kcal na porci doplní uživatelka, až budou recepty na webu
* Kalkulačka: Mifflin-St Jeor, jen pro dospělé 18+, příjem nikdy pod BMR, vždy uvést, že nejde o lékařskou radu
* Web – technické detaily k úkolům: úvodní video hledá `video/kulinarium.mp4` (neexistuje, k dispozici je `images/4. května 2026.mp4`, 36 MB); `kalkulacka.html` v kořeni je prázdný soubor (nikdo na něj neodkazuje); `recepty/ledova-kava.html` a `okurkova-limonada.html` jsou jen úryvky k vložení do `napoje.html`

## PROJEKT.md – rozhodnutí, úkoly, nápady

* **Rozhodnutí, úkoly, nápady a popis funkcí jsou v `PROJEKT.md`** (kniha projektu pro uživatelku). Sem je neduplikuj.
* Chat = brainstorming a práce. **Po každé dohodě v chatu hned aktualizuj `PROJEKT.md`** (a datum „Poslední aktualizace“) a řekni, co jsi tam zapsal.
* Zapisuj jen to, na čem se shodnete. Nerozhodnuté nápady → část 💡 Nápady. Hotové úkoly → odškrtni a přesuň do „Hotovo“.
* Piš ho pro uživatelku: srozumitelně, bez technických detailů (ty patří sem do Nuancí).

## Údržba tohoto souboru

* Aktualizuj po každé strukturální změně, novém pravidlu nebo rozhodnutí
* Maximální stručnost – detaily patří do kódu nebo README, ne sem
* Smaž zastaralé info, nepřidávej duplicity
