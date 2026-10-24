# Niky's Kitchen – kniha projektu

Sem se zapisuje jen to, na čem jsme se v chatu **shodly**. Nápady, o kterých ještě nevíme, patří do části 💡 Nápady.
Poslední aktualizace: 2026-10-24

---

## 🎯 O projektu

* **Co to je:** web a blog o zdravém jídle a pečení + webová appka **Jídlo od A–Z**. Později obchod s digitálními produkty (e-booky, online kuchařka, kurzy).
* **Proč:** ulehčit lidem zdravé stravování – jasná odpověď na „co mám dnes jíst a kolik“, bez složitého počítání.
* **Pro koho:** ženy i muži 18+, kteří berou zdravý životní styl jako investici do budoucna, ale nemají moc času. Chtějí zhubnout, udržet formu, nebo nabrat svaly.
* **Jak mluvíme:** přátelsky, tykáme, jako kamarádka. Žádná falešná hodnocení ani zdravotní sliby.
* **Jak to do sebe zapadá:** web přivádí čtenáře (recepty, články) → appka jim pomáhá v praxi (kolik jíst, co uvařit, co koupit) → obchod nabídne plány, e-booky a kurzy, které jdou do hloubky.

---

## 🌐 Web

**Stav:** funkční základ, soukromý na GitHubu, zatím není online.

| Stránka | Co obsahuje | Stav |
|---|---|---|
| Domů | úvod s videem, záložky s recepty, výhody, pozvánka do appky, náhled galerie | ⚠️ chybí video, hodnocení „★ 5.0“ nejsou skutečná |
| Recepty → Slané | Koláč od Niky + 3 kategorie | ⚠️ kategorie bez receptů |
| Recepty → Sladké | 3 kategorie | ⚠️ zatím bez receptů |
| Recepty → Nápoje | 3 kategorie, článek o ginger shotu | ⚠️ recepty na ledovou kávu a okurkovou limonádu jsou napsané, ale nejsou vložené |
| Články | přehled článků, boční panel | ❌ ukazuje 3 vymyšlené články, skutečné tam chybí |
| Galerie | karusel podle kategorií | ⚠️ místo fotek zástupné texty |
| O mně | krátké představení | ✅ |

**Hotové články (složka `clanky/`):** Kolik toho vlastně sníst? (s kalkulačkou) · Když přijdeš domů unavená · Proč po některém jídle hned hladovíš · Trávení po tréninku · Letní ovoce a bylinky v nápojích · Kalkulačka příjmu

**Detail receptu:** `recepty/Kolac.html` je nejpropracovanější (suroviny, postup, fotky), ale nefunguje v něm přepočet porcí.

**Menu (platí pro všechny stránky):** Domů · Recepty ▾ (Slané, Sladké, Nápoje) · Články · Aplikace · Galerie · O mně

---

## 📱 Aplikace Jídlo od A–Z

**Stav:** hotová první verze, veřejně online: https://4613nikola-oss.github.io/jidlo-od-a-z/

**Co umí:**
* **Profil** – z věku, váhy, výšky, pohybu a cíle (hubnout / udržet / nabrat) spočítá denní příjem
* **Můj den** – rozdělí příjem na snídani, oběd, večeři a svačinu, navrhne recepty a počet porcí
* **Lednička** – podle toho, co máš doma, ukáže, co uvaříš a co chybí
* **Recepty** – slané, sladké, nápoje, s hledáním
* **Nákup** – nákupní seznam z receptů, celého dne nebo ledničky
* doporučí články podle cíle, pamatuje si údaje, jde přidat na plochu mobilu

**Omezení:** recepty (14) a kcal jsou zatím ukázkové.

---

## 🛒 Obchod (později)

* **Digitální produkty** – bez skladu a rozvozu: malý placený vstup (mini e-book, plán na 7 dní) → hlavní nabídka (online kuchařka, kurz vaření dopředu s online setkáními, e-book pro starší) → pro věrné (předplatné, komunita)
* Objednávky, platby a faktury přes FAPI (návrh)
* Krabičky s jídlem zatím odložené – moc práce

---

## ✅ Rozhodnutí

* **2026-09-24** – Appka se jmenuje **Jídlo od A–Z**, podtitul pro Google: „kalorická kalkulačka, jídelníček a recepty z ledničky“
* **2026-09-24** – Appka je čisté HTML/CSS/JS bez frameworku – jednoduché, běží všude
* **2026-09-26** – Appka je veřejná (GitHub Pages, Docker Hub) kvůli portfoliu. Web zůstává soukromý, dokud nebude hotový
* **2026-09-28** – Značka je **Niky's Kitchen**, „Koláč od Niky“ je jen název receptu
* **2026-09-28** – Tón: přátelský, tykání. Cílovka: ženy i muži 18+
* **2026-09-28** – Položka „Aplikace“ v menu vede zatím na živou appku, později bude appka přímo součástí webu
* **2026-09-30** – Chat slouží k brainstormingu a práci, dohody se zapisují sem do PROJEKT.md
* **2026-10-03** – **Celý web i appka budou česky i anglicky** (ne jen pro Prahu). Texty se od začátku píšou tak, aby šly snadno přeložit
* **2026-10-03** – **Jen dva jazyky** (čeština a angličtina). Další jazyky ne, zbytečně by zatížily web, blog, appku i e-shop
* **2026-10-03** – Appku starším lidem zvlášť nepřizpůsobujeme (často nemají chytrý telefon nebo appky neovládají). Pro ně spíš e-book (viz Nápady). Základní přístupnost platí pro všechny
* **2026-10-03** – **Obchod prodává digitální produkty**, ne vařená jídla (krabičky = moc práce, sklad, rozvoz). Krabičky odloženy
* **2026-10-03** – **Nejdřív malý placený produkt**, ne všechno zdarma – zdarma jen to, co přivádí lidi (blog, část receptů, základní kalkulačka)
* **2026-10-05** – **Sociální sítě spouštíme hned**: Instagram a Facebook teď, Pinterest až bude web online, TikTok později. Startovní balíček v `podklady/SOCIALNI-SITE.md`
* **2026-10-05** – **Nový web v Next.js** (mění rozhodnutí z 24. 9.): web, appka a obchod časem v jednom projektu `niky-web`, dvě jazykové verze, statický web na GitHub Pages. Starý web a appka běží dál, dokud nebude nový hotový
* **2026-10-05** – Postup po fázích: **Fáze 0** nastavení projektu → **Fáze 1** kostra a design webu → dál detaily. **Databáze a přihlášení až později**
* **2026-10-05** – Příkazy (instalace, buildy, testy) se spouštějí **jen v Dockeru**, nic se neinstaluje přímo do počítače. Práce probíhá ve fázích: nejdřív struktura, pak detaily, průběžná kontrola v prohlížeči
* **2026-10-24** – **Dvě větve na GitHubu:** `dev` = rozpracované (Claude tam nahrává průběžně), `main` = hotové a živé. Do `main` jde až na pokyn Niky („nahraj to“)
* **2026-10-24** – **Podklady jsou zálohované na GitHubu** v samostatném soukromém repozitáři `nikys-kitchen-projekt` (kniha projektu, pravidla, brainstorming, logo, maskot)
* **2026-10-03** – Design musí být **responzivní** (mobil, tablet, počítač)
* **2026-10-03** – Web má být **co nejpřívětivější pro co nejvíc lidí, nikoho nevynechat** (jazyk, zrak, věk, zdraví, peníze, čas, technika)
* **2026-10-03** – Vizuální podklady a brainstorming žijí v Miru a ve složce `podklady/`; průběžně se aktualizují podle dohod

---

## 📋 Úkoly

Seřazené podle doporučeného pořadí.

**Sociální sítě:**
* [ ] Vybrat název účtu a založit Instagram + stránku na Facebooku (Niky)
* [ ] Prvních 14 dní podle plánu v `podklady/SOCIALNI-SITE.md`

**Nový web v Next.js (`niky-web`):**
* [x] **Fáze 0:** nastavení projektu – instalace, Docker, struktura stránek, čeština a angličtina, barvy a písma, logo, prázdné stránky (2026-10-05)
* [x] **Fáze 1 (první verze):** 17 receptů (6 slaných, 5 sladkých, 6 nápojů) a 6 článků česky i anglicky, propojené mezi sebou; paleta šalvěj/med/terakota; Tečka na úvodu, v kartách, na 404 a v patičce; přepočet porcí; fotky ve WebP (2026-10-05)
* [ ] Doladit podle moodboardu ve Figmě
* [ ] Niky zkontroluje ukázkové recepty (množství, postup, kcal) a doplní kcal u Koláče, ledové kávy, limonády a ginger shotu
* [ ] Skutečné fotky místo AI ilustrací u Koláče
* [x] Repozitář na GitHubu `nikys-kitchen-web` (soukromý) – založen a nahrán (2026-10-24)
* [ ] SEO základ: mapa webu, data receptů pro Google, propojení CZ/EN
* [ ] Stránky: prohlášení o přístupnosti, ochrana soukromí
* [ ] Později: appka uvnitř webu, obchod (FAPI), databáze a přihlášení

**Starý web a appka:**

1. [ ] **Články:** na stránku Články dát skutečné články místo vymyšlených
2. [ ] **Recepty:** opravit useknutý recept, zprovoznit přepočet porcí, vložit ledovou kávu a okurkovou limonádu do Nápojů
3. [ ] **Domů:** vyřešit úvodní video (chybí) a nahradit nepravdivá hodnocení
4. [ ] **Rychlost:** zmenšit fotky (2–3,5 MB → WebP kolem 200 kB)
5. [ ] **Appka do webu:** vložit Jídlo od A–Z jako sekci webu
6. [ ] **Recepty s kcal:** u každého receptu kcal na porci → přenést do appky místo ukázkových
7. [ ] **Web online:** zveřejnit web (GitHub Pages)
8. [ ] **Newsletter a sociální sítě:** napojit, nebo zatím skrýt
9. [ ] **Anglická verze celého webu a appky** (texty připravovat na překlad už od teď)

**Hotovo:**
* [x] Appka upozorní, když se údaje neukládají (anonymní okno); v hlavičce značka Niky's Kitchen (2026-10-03)
* [x] Appka na GitHubu, v Dockeru a veřejně online (2026-09-26)
* [x] Web v Cursoru a na GitHubu, oprava chyby, která vypínala JavaScript (2026-09-26)
* [x] Web sjednocený: menu, název, tykání, chybějící styly (2026-09-28)

---

## 💡 Nápady (zatím nerozhodnuté)

* Týdenní jídelníček místo jednoho dne + nákupní seznam na týden (appka)
* Kcal štítek u každého receptu a přepočet „kolik z toho sníst“ na webu
* Jeden společný soubor receptů pro web, appku i e-shop
* Bílkoviny u receptů, pitný režim, filtr pro vegetariány (appka)
* Recepty s daty pro Google (čas, kcal přímo ve výsledcích hledání)
* **E-book pro starší a jejich blízké:** PDF i tisk, koupit v e-shopu nebo darovat (třeba rodičům). Časté potíže, jejich příčiny a jak řešit příčinu, ne jen následky; nemoci, které trápí starší lidi. Zdravotní obsah zkontroluje odborník. Mohl by být první placený produkt
* **Maskot značky** – vlastní postavička, která se objeví na webu, v appce, v obchodě i v GIFech na sítích (vítá, počítá, vaří, utěšuje při chybě, slaví). Koncepty: **Tečka** (sladká tečka se šalvějovým lístkem) a **Kastrolek**. Niky se líbí Tečka s nápadem, že se **promění v předmět** (talíř, koláč, vidlička…), lístek a oči zůstávají. Soubory v `podklady/maskot/`, náhled v Miru (rám 27)
* **Plán sociálních sítí a reklamy** (návrh v Miru, rámy 28 a 29): Instagram, Pinterest, Facebook, později TikTok, e-mail a nálepky Tečky na GIPHY; šablony karuselu a krátkého videa; reklama až s prvním placeným produktem, malý test 1–3 tis. Kč
* *(odloženo)* **Niky's krabičky** jako název e-shopu s krabičkami, tři varianty FIT / STANDARD / SVALY (= hubnout / udržet / nabrat), logo NK a heslo „Zdravě a chutně“
* **Štítná žláza:** lidé po jejím odstranění často řeší přibírání (v průměru asi +2 kg) – téma pro článek a pro upozornění v kalkulačce

---

## 🔗 Odkazy

* Podklady ve složce `podklady/`: `DASHBOARD.md` (rozcestník a stav), `BRAINSTORMING.md` (průzkum, věda, konkurence, návrhy), `SITEMAP.md`, `PERSONY.md`, `FLOW.md`
* Logo **Niky's krabičky** ve vektoru: `podklady/logo/` (logo-novy, logo-nalepka, logo-ikona-NK – SVG i PNG; logo-vektor-podle-originalu = věrná kopie)
* Vizuální mapy v Miru (myšlenková mapa, persony, sitemap, flow): https://miro.com/app/board/uXjVIpEXRLo=/

* Appka online: https://4613nikola-oss.github.io/jidlo-od-a-z/
* Kód appky: https://github.com/4613nikola-oss/jidlo-od-a-z
* Kód webu (soukromý): https://github.com/4613nikola-oss/nikys-kitchen
* Docker obraz: https://hub.docker.com/r/nikolapaluskova/jidlo-od-a-z
