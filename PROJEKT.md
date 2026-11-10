# Niky's Kitchen – kniha projektu

Sem se zapisuje jen to, na čem jsme se v chatu **shodly**. Nápady, o kterých ještě nevíme, patří do části 💡 Nápady.
Poslední aktualizace: 2026-11-10

---

## 🎯 O projektu

* **Co to je:** web a blog o zdravém jídle a pečení + webová appka **Jídlo od A–Z**. Později obchod s digitálními produkty (e-booky, online kuchařka, kurzy).
* **Proč:** ulehčit lidem zdravé stravování – jasná odpověď na „co mám dnes jíst a kolik“, bez složitého počítání.
* **Pro koho:** ženy i muži 18+, kteří berou zdravý životní styl jako investici do budoucna, ale nemají moc času. Chtějí zhubnout, udržet formu, nebo nabrat svaly.
* **Jak mluvíme:** přátelsky, tykáme, jako kamarádka. Žádná falešná hodnocení ani zdravotní sliby.
* **Jak to do sebe zapadá:** web přivádí čtenáře (recepty, články) → appka jim pomáhá v praxi (kolik jíst, co uvařit, co koupit) → obchod nabídne plány, e-booky a kurzy, které jdou do hloubky.

---

## 🌐 Web

**Nový web (Next.js) – online:** https://4613nikola-oss.github.io/nikys-kitchen-web/
* 17 receptů (slané, sladké, nápoje) a 6 článků, česky i anglicky, propojené mezi sebou
* recepty a články jsou v databázi, přepočet porcí, alergeny, maskot Tečka
* README na GitHubu se screenshoty, schématem a popisem, co projekt řeší

**Starý web (čisté HTML)** – běží dál jen jako archiv, dokud nový nepřevezme všechno:

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

**Recepty:** bere si je z databáze přes nový web (17 receptů). Když se nenačtou, použije záložní ukázkové recepty, takže funguje vždycky. Recepty bez kcal se do plánu dne nedávají.

---

## 🛒 Obchod (později)

* **Digitální produkty** – bez skladu a rozvozu: malý placený vstup (mini e-book, plán na 7 dní) → hlavní nabídka (online kuchařka, kurz vaření dopředu s online setkáními, e-book pro starší) → pro věrné (předplatné, komunita)
* Objednávky, platby a faktury přes FAPI (návrh) – platforma pro skutečný prodej ještě není rozhodnutá, musí být bez měsíčního poplatku
* Krabičky s jídlem zatím odložené – moc práce
* **Ukázkový obchod na Shopify** (do portfolia, nedá se v něm skutečně prodávat): vývojářský obchod 
ikys-krabicky.myshopify.com`, zdarma bez limitu. Ukázková data od Shopify smazána, zůstal Pondělní oběd (Fit / Standard / Svaly)

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
* **2026-10-25** – **Projekt je i portfolio pro práci**: má ukázat firmám, že Niky umí spravovat e-shop (platformu, analytiku, marketing). Nástroje vybíráme i podle toho, co firmy chtějí v inzerátech
* **2026-11-07** – **Jedna databáze pro web i appku** (PostgreSQL, běží v Dockeru). Recepty a články jsou uložené jen jednou, appka si je stahuje z webu. Když se nestáhnou, má záložní recepty a funguje dál
* **2026-10-25** – **Obchod bude přímo součástí webu**, ne samostatný web. Všechno na jednom místě (recepty, články, appka, obchod, newsletter) je pro lidi pohodlnější a ukazuje, že Niky umí dotáhnout celý projekt
* **2026-10-25** – **Všechno zdarma natrvalo** – žádné měsíční poplatky ani placené zkušební verze, které po měsíci začnou stát peníze
* **2026-10-25** – **Nový web bude veřejný** (repozitář i stránka na GitHub Pages, zdarma). Veřejná zůstává i appka. ~~Soukromé zůstávají podklady a starý web~~ – změněno 7. 11., všechno je veřejné (písma ze starého webu nahrazena)
* **2026-11-08** – **Postup po fázích A–E:** A opravy webu a appky → B vzhled (3 varianty pozadí, Tečka překreslená do stylu loga, vlastní ikonky, mikroanimace) → C nová appka uvnitř webu (plán den/týden/měsíc, profil s průvodcem, filtry, oblíbené, nákup na týden) → D přihlášení (avatar, historie, newsletter) → E komunita (hodnocení, sekce Od babičky)
* **2026-11-08** – **Kcal u receptů spočítané orientačně** z množství surovin (Koláč 520, ledová káva 100, limonáda 30, ginger shot 40 kcal na porci). Niky je může upravit v Admineru
* **2026-11-08** – **Ceny produktů** (podle průzkumu trhu a plánu „zdarma přivede → malá placená věc → větší nabídka“): Startovací knížka zdarma za e-mail, Týdenní plán 99 Kč, e-book Jeden základ, tři varianty 249 Kč, e-book pro starší 249 Kč, Kurz vaření dopředu 990 Kč (zaváděcí 690 Kč), Online kuchařka 129 Kč/měsíc. Krabičky v Shopify: Fit 149, Standard 159, Svaly 179 Kč za oběd
* **2026-11-08** – **Na webu jsou v obchodě všechny produkty** s obálkou, cenou, popisem a ukázkou zdarma (u plánu celý den ze skutečných receptů + PDF). Zatím „připravujeme“
* **2026-11-08** – **Ukázkový Shopify obchod má 3 typy zboží:** krabičky, digitální produkty a merch s Tečkou (magnetky, kolíčky, nálepky, sklenice na kaši, krabička na jídlo, taška). Merch jen v Shopify, ne na webu
* **2026-11-07** – **Všechny repozitáře jsou veřejné** (rozhodla Niky): nový web, appka, starý web i podklady. Hesla a soukromé soubory hlídá pojistka `.gitignore`
* **2026-11-07** – **Shopify vývojářský obchod jde do portfolia** (zdarma, bez placených aplikací). Učení „jednou Claude, podruhé Niky“: Claude udělá jednu věc, Niky tu další sama v administraci, Claude zkontroluje
* **2026-11-07** – **Persony mají přesný věk** (Petra 35, Tomáš 27, Jana 38, Kája 21, Martin 54, Pavel 41, Emma 31) a profilové fotky (Niky je doplňuje v Miru)
* **2026-11-10** – **Obchod bez štítku „Připravujeme“.** Místo „Koupit“ je u produktů formulář „Mám zájem“ (e-mail), protože produkty zatím nejsou napsané a není platební brána. Prodávat se bude až s hotovými produkty, platbou a živnostenským listem
* **2026-11-10** – **Dva kurzy:** online Kurz vaření dopředu (690 Kč, zaváděcí) a **Kurz vaření naživo** (1 290 Kč za osobu, 3 hodiny, max. 8 lidí). Oba mají místo obálky ilustraci (lektorka online / skupina vaří s lektorkou). Startovací knížka je jen v boxu s newsletterem, ne dvakrát
* **2026-11-10** – **Newsletter a „Mám zájem“ přes Make → Google tabulka** (zdarma). E-maily se ukládají do tabulky v Google účtu Niky (ne RDCUK). Rozesílat zatím z Gmailu, později třeba MailerLite
* **2026-11-10** – **Recepty se zobrazují na 1 porci**, aby to sedělo s „kcal na porci“. Tlačítky +/− se přepočítají
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
* [x] SEO základ: mapa webu, data receptů pro Google (čas, kcal, suroviny), propojení CZ/EN, náhledy při sdílení (2026-11-09)
* [x] Stránky: prohlášení o přístupnosti, ochrana soukromí, odkazy v patičce (2026-11-09)
* [x] Recept jde vytisknout nebo uložit jako PDF (2026-11-09)
* [ ] Doplnit kontakt na ochranu soukromí a přístupnost (e-mail značky) – newsletter už běží, takže co nejdřív
* [ ] **Niky:** v Make potvrdit připojení svého Google účtu (odkaz v chatu 10. 11.) → Claude dokončí zápis do tabulky
* [ ] **Niky:** v nastavení Hugging Face povolit generování obrázků → Claude vytvoří fotky ke 16 receptům
* [ ] Fáze B – nový vzhled: Niky vybere pozadí A–F, pak se přenese na web i do appky (nová Tečka, ikonky, avatary, karta, animace 3 a 4)
* [ ] Napsat Startovací knížku (dárek za newsletter) – Claude ji může poskládat z receptů v databázi do PDF
* [ ] Až bude web online s novými stránkami: přidat ho do Google Search Console a odeslat mapu webu (sitemap.xml)
* [ ] Před spuštěním newsletteru nebo obchodu nechat ochranu soukromí zkontrolovat (nejde o právní radu)
* [x] **Databáze:** recepty a články jsou v jedné databázi, web i appka si je berou odtud; připravené tabulky pro newsletter a obchod (2026-11-07)
* [x] Kcal u Koláče, ledové kávy, limonády a ginger shotu – spočítané orientačně (2026-11-08)

**Fáze A – opravy (2026-11-08):**
* [x] Web: filtry receptů (kategorie, štítky, bez alergenu), hledání s překlepy a nabídkou podobných, „Načíst další“, kcal i při změně porcí, alergeny žlutě s trojúhelníkem, varianty jako karty po dnech
* [x] Appka: celá karta klikací, kontrastní tlačítka, chytré hledání, odkaz zpět na web, tipy na obchod
* [ ] Niky: fotky jídel podle připraveného promptu, příběh pro O mně, recepty od babičky
* [ ] Později: appka uvnitř webu, obchod, přihlášení, databáze na internetu pro newsletter a objednávky

**Shopify – ukázkový obchod do portfolia** (úkoly i návody jsou v E-commerce akademii, modul 16):
* [x] Smazat 17 ukázkových produktů od Shopify, opravit překlep „obět“ → „oběd“ (2026-11-07)
* [ ] Přejmenovat obchod (doporučení: **Niky's Kitchen**), měna CZK, země Česko, časové pásmo Praha – Niky v Nastavení
* [x] Digitální produkty (6) a merch (6) s obrázky, ceny krabiček, digitální bez dopravy (2026-11-08)
* [ ] Obědy úterý až pátek (Niky sama podle pondělního vzoru)
* [ ] Kolekce, slevový kód VITEJ10, testovací objednávka a její vyřízení
* [ ] Téma obchodu na GitHub (repozitář `nikys-kitchen-shopify`)
* [ ] Case study do portfolia (web, appka, databáze, Shopify)

**Persony a výzkum:**
* [x] Přesný věk u všech person (Miro i PERSONY.md) a místo na fotky v Miru (2026-11-07)
* [ ] Niky doplní fotky person v Miru (Upload → hledání obrázků, Unsplash zdarma)

**Starý web a appka:**

1. [ ] **Články:** na stránku Články dát skutečné články místo vymyšlených
2. [ ] **Recepty:** opravit useknutý recept, zprovoznit přepočet porcí, vložit ledovou kávu a okurkovou limonádu do Nápojů
3. [ ] **Domů:** vyřešit úvodní video (chybí) a nahradit nepravdivá hodnocení
4. [ ] **Rychlost:** zmenšit fotky (2–3,5 MB → WebP kolem 200 kB)
5. [ ] **Appka do webu:** vložit Jídlo od A–Z jako sekci webu
6. [ ] **Recepty s kcal:** u každého receptu kcal na porci → přenést do appky místo ukázkových
7. [x] **Web online:** hotovo – online je nový web (2026-11-07)
8. [x] **Newsletter:** formulář na webu v obchodě, ukládá do Google tabulky přes Make (2026-11-10). Sociální sítě zatím ne
9. [ ] **Anglická verze celého webu a appky** (texty připravovat na překlad už od teď)

**Hotovo:**
* [x] **Nový web je online** na https://4613nikola-oss.github.io/nikys-kitchen-web/ (zdarma přes GitHub Pages); appka si z něj bere recepty z databáze (2026-11-07)
* [x] Zabezpečení GitHubu: pojistka proti nahrání hesel ve všech repozitářích, u veřejné appky zapnutá ochrana Secret Protection + Push protection, podklady zálohované v soukromém repozitáři (2026-10-24)
* [x] Appka upozorní, když se údaje neukládají (anonymní okno); v hlavičce značka Niky's Kitchen (2026-10-03)
* [x] Appka na GitHubu, v Dockeru a veřejně online (2026-09-26)
* [x] Web v Cursoru a na GitHubu, oprava chyby, která vypínala JavaScript (2026-09-26)
* [x] Web sjednocený: menu, název, tykání, chybějící styly (2026-09-28)

---

## 💡 Nápady (zatím nerozhodnuté)

* Týdenní jídelníček místo jednoho dne + nákupní seznam na týden (appka)
* Kcal štítek u každého receptu a přepočet „kolik z toho sníst“ na webu
* ~~Jeden společný soubor receptů pro web, appku i e-shop~~ → hotovo jako databáze (2026-11-07)
* **Merch pro skutečný obchod** (sklenice, tašky s Tečkou) – až budou fanoušci; fyzické zboží = sklad, balení, rozbité sklo, poštovné
* **Cenové schody:** zdarma (recepty, články, appka, newsletter) → dárek za newsletter (startovací knížka 7 receptů + sleva 10 %) → malý placený produkt (týdenní plán PDF) → větší nabídka (e-kuchařka, kurz, prémiová appka). Newsletter jednou za 14 dní
* **Dotazník** k ověření person (Google Forms, 8–10 otázek)
* **Jedna výrazná barva navíc** do palety (šafránová / citrusová žlutá) jen na ~10 % plochy: štítky, sladká tečka, jedno hlavní tlačítko
* **Případová studie (case study)** projektu do portfolia: problém → výzkum → rozhodnutí → design → výsledek se screenshoty → co ses naučila
* Na skutečný prodej bude potřeba **živnostenský list**
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

* **Nový web online:** https://4613nikola-oss.github.io/nikys-kitchen-web/ · kód: https://github.com/4613nikola-oss/nikys-kitchen-web
* Appka online: https://4613nikola-oss.github.io/jidlo-od-a-z/
* Kód appky: https://github.com/4613nikola-oss/jidlo-od-a-z
* Kód starého webu: https://github.com/4613nikola-oss/nikys-kitchen
* Podklady na GitHubu: https://github.com/4613nikola-oss/nikys-kitchen-projekt
* Shopify ukázkový obchod: https://admin.shopify.com/store/nikys-krabicky
* E-commerce akademie (modul 16 Shopify): https://claude.ai/artifact/LMsffmgAa9jSQo5jL4Ugpm
* Zápisek „Databáze pro Niky's Kitchen“ v Notionu: https://app.notion.com/p/4118e89419e08160afb9e772c22b1c57
* Docker obraz: https://hub.docker.com/r/nikolapaluskova/jidlo-od-a-z
