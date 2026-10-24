# Niky's Kitchen – velký brainstorming

Všechno z brainstormingu 2026-10-02 na jednom místě: průzkum, věda, konkurence, persony, mapa webu, appka, e-shop a rozbor kalkulační tabulky.
Spojuje všechny tři dnešní kola (průzkum trhu → psychika, zdraví, přístupnost → kalkulačka) do jednoho dokumentu.
**Tohle jsou návrhy a podklady, ne rozhodnutí.** Co spolu odsouhlasíme, se zapíše do `PROJEKT.md`.

---

## Obsah

1. [Proč to děláme](#1-proč-to-děláme)
2. [Myšlenková mapa projektu](#2-myšlenková-mapa-projektu)
3. [Průzkum trhu](#3-průzkum-trhu)
4. [Co říká věda](#4-co-říká-věda)
5. [Konkurence](#5-konkurence)
6. [V čem jsme jiní](#6-v-čem-jsme-jiní)
7. [Persony](#7-persony--pro-koho-to-děláme)
8. [Hlavní koncepty](#8-hlavní-koncepty)
9. [Kalkulačka](#9-kalkulačka--jak-počítat)
10. [Mapa webu](#10-mapa-webu-sitemap)
11. [Aplikace](#11-aplikace-jídlo-od-az)
12. [Web](#12-web-a-blog)
13. [E-shop](#13-e-shop)
14. [Přístupnost a angličtina](#14-přístupnost-a-angličtina)
15. [Motivace bez tlaku](#15-motivace-bez-tlaku)
16. [Kdo – co – proč](#16-kdo--co--proč)
17. [Zákony a rizika](#17-zákony-a-rizika)
18. [Návrh pořadí práce](#18-návrh-pořadí-práce)
19. [Otevřené otázky](#19-otevřené-otázky)
20. [Zdroje](#20-zdroje)

---

## 1. Proč to děláme

**Problém:** lidé chtějí jíst zdravě, ale:

* mají náročnou práci a **nemají čas ani energii** vařit každý den něco jiného,
* **nevědí, kolik** toho sníst a **jak poskládat talíř**,
* kalorické appky je **nebaví** – zapisování zabírá čas a po pár týdnech ho vzdají,
* zapisování v nich vyvolává **výčitky** („to jsem si neměla dát“), což není dobré pro psychiku a u části lidí to souvisí s poruchami příjmu potravy,
* mladší generace mají **problém s pozorností** – dlouhé články a složité appky je zahltí,
* lidé s **alergiemi a nemocemi** (cukrovka, vysoký tlak, celiakie) mají málo jednoduchých zdrojů,
* na **nevidomé** a **cizince** (angličtina v Praze) se obvykle zapomíná.

**Vize:** jasná odpověď na „co mám dnes jíst a kolik“ – bez zapisování, bez výčitek, s radostí.

**Proč na tom záleží:** zdravá strava a pohyb jsou klíčem ke zdravému životu. Ovlivňují obezitu, cukrovku, vysoký tlak i cholesterol – tedy i několik rizikových faktorů demence (viz [kap. 4](#4-co-říká-věda)).

---

## 2. Myšlenková mapa projektu

```
                                NIKY'S KITCHEN
                     „Jez s radostí, ne s výčitkami“
                                      │
        ┌─────────────────────────────┼──────────────────────────────┐
        │                             │                              │
     🌐 WEB                     📱 APPKA                        🛒 E-SHOP
  přivádí čtenáře            pomáhá v praxi                  hotová jídla
        │                    „Jídlo od A–Z“                         │
        ├─ Recepty               ├─ Profil + kalkulačka            ├─ Bowly
        │   └─ základ + 3        │   ├─ jednoduchá                  ├─ Krabičky
        │      varianty          │   └─ pokročilá (InBody)          ├─ Filtry: cíl,
        ├─ Články                ├─ Můj den / týden                 │   kcal, bílkoviny,
        │   └─ „V kostce“ +      ├─ Stavebnice talíře               │   alergeny, cena
        │      rozkliknutí       ├─ Lednička                        ├─ Stejné varianty
        ├─ Sladká tečka          ├─ Recepty + filtry                │   jako recepty
        ├─ Vaření dopředu        ├─ Nákupní seznam                  └─ Alergeny u
        │   („krabičky sám“)     ├─ Odškrtávání (ne zapisování)        produktu (zákon)
        ├─ Galerie, O mně        └─ Razítka a odměny
        └─ English: Czech
           ingredients explained
                                      │
        ┌─────────────────────────────┼──────────────────────────────┐
   ♿ PŘÍSTUPNOST             🩺 ZDRAVÍ A BEZPEČÍ              🎮 MOTIVACE
   čtečka, kontrast,         filtry: alergeny, cukrovka,       razítka, výzvy,
   klávesnice, režim         tlak, bezlepek, trávení;          1 změna týdně,
   „vaříme“                  nepočítat: těhotné, <18,          bez trestů
                             podváha → odborník
```

---

## 3. Průzkum trhu

### Česko – lidé a zdraví

| Fakt | Číslo | Zdroj |
|---|---|---|
| Nadváha nebo obezita | **64 %** dospělých | Deník.cz, SZÚ |
| Přibrali za poslední rok | víc než polovina lidí, průměrně o 3 kg | Deník.cz |
| Vysoký tlak (léčený) | **2,2 mil.** (20 % populace), až třetina dalších o něm neví | VZP, MZd |
| Cukrovka | **přes 1,1 mil.**, ročně přibývá asi 20 tisíc | ÚZIS |
| Celiakie | 0,4–0,5 % populace, většina nediagnostikovaná | Medicína pro praxi |
| Cizinci v Praze | **asi 25 %** obyvatel (konec 2024), skoro polovina z Ukrajiny | ČSÚ |
| Vyhozené jídlo | 37–57 kg na osobu a rok, nejvíc plýtvá generace Z | ČSÚ, iRozhlas |

### Trh s appkami a jídlem

| Fakt | Číslo | Co z toho plyne |
|---|---|---|
| Kalorické tabulky | ~1,5 mil. aktivních měsíčně, 7 mil. registrací, ale denně zapisuje jen **150–200 tis.** (2024) | lidé chtějí přehled, zapisování je nebaví |
| Odchod z kalorických appek | **65 % lidí skončí do 90 dnů**; důvody: zapisování zdržuje (34 %), chybí potraviny (28 %), nevidí výsledky (24 %) *(zdroj: firma s vlastní appkou)* | ⭐ hlavní příležitost – appka bez zapisování |
| První týden | kdo zapisuje 5+ dní v 1. týdnu, většinou vydrží | appka musí být užitečná hned |
| Krabičkové diety v ČR | trh ~750 mil. Kč ročně, ~30 firem, **289–500 Kč/den** (9–15 tis. měsíčně) | zájem o „jídlo na míru“ je, ale je drahé |
| NutritionPro | tržby 160 mil. Kč, algoritmus sestaví jídelníček na míru | konkurence v „na míru“ je silná |
| Svět | 175–200 mil. lidí používá kalorické appky; trh roste ~12–17 % ročně | obor roste |

---

## 4. Co říká věda

Jen ověřené zdroje (PubMed, WHO, odborné společnosti). Kde výzkum vyšel jinak, než by se nám hodilo, je to napsané.

### Zapisování jídla a psychika

* Studie na 493 vysokoškolácích: lidé, kteří si počítají kalorie v appce, mají víc starostí kolem jídla a víc se omezují. Autorky píšou, že některým lidem můžou appky víc uškodit než pomoct. *(Simpson & Mazzeo, 2017)*
* Ze 105 lidí s poruchou příjmu potravy používalo MyFitnessPal ~75 % a **73 % z nich mělo pocit, že appka k poruše přispěla**. *(Levinson a kol., 2017)*
* ⚠️ Obě studie ukazují souvislost, ne příčinu.
* → **Appka bez povinného zapisování.**

### Sladká tečka bez výčitek

* Studie na 54 tisících lidí: **přísná kontrola** („nikdy čokoládu“) souvisí s vyšší váhou a přejídáním; **flexibilní kontrola** („klidně, jen míň“) s nižší váhou, menším přejídáním a **úspěšnějším hubnutím**. *(Westenhoefer a kol., 1999; potvrzeno Timko & Perone, 2005)*
* Velikost tečky: **WHO doporučuje přidaný cukr pod 10 % denního příjmu** → tečka do ~10 % dne (u 2 000 kcal ~200 kcal).
* 💬 Formulace: „tečka je **součást plánu**“, ne „zasloužila sis to“ – aby nevzniklo „když nevydržím, nezasloužím si“.

### Odměny a hry v appce

* Přehled 36 studií (10 tisíc lidí, 2024): prvky hry přinesly navíc ~0,7 kg úbytku a o něco víc pohybu – **malý, ale skutečný efekt**. *(Nishi a kol., 2024)*
* Lidi nejvíc baví **překvapení, novinky, výzvy a přehledný design**; zájem časem klesá. *(Davis a kol., 2021)*
* → odměny jako bonus, **nikdy trest** za vynechaný den.

### Demence – poctivě

* Komise Lancet (2024): **14 ovlivnitelných rizikových faktorů**, jejich odstranění by mohlo oddálit nebo zabránit **téměř polovině případů**. Se stravou a pohybem souvisí: obezita, cukrovka, vysoký tlak, vysoký LDL cholesterol, málo pohybu, alkohol.
* ⚠️ Studie diety MIND (604 lidí, 3 roky) **nenašla rozdíl** oproti běžné zdravé stravě s mírně nižším příjmem – zlepšily se obě skupiny. *(Barnes a kol., NEJM 2023)*
* → sdělení „**zdravý životní styl jako celek**“, ne „jídlo proti demenci“ (a to ani nesmíme – viz [kap. 17](#17-zákony-a-rizika)).

### Bílkoviny

* Pro aktivní lidi, kteří chtějí nabrat nebo udržet svaly: **1,4–2,0 g na kg váhy denně**, na jedno jídlo 20–40 g, rozložit během dne. *(ISSN, Jäger a kol., 2017)*

### Jak poskládat talíř

* **Harvardský talíř:** ½ zelenina a ovoce, ¼ celozrnná příloha, ¼ bílkoviny, k tomu kvalitní tuk a voda.

### Krátce a jasně

* Princip „**postupného odkrývání**“: nejdřív to nejdůležitější, detail až na rozkliknutí. Pomáhá lidem, kteří se rychle zahltí.

---

## 5. Konkurence

| Kdo | Silné stránky | Slabiny = naše šance |
|---|---|---|
| **Kalorické tabulky** (CZ) | obrovská databáze, AI pozná jídlo z fotky, Premium 199 Kč/měs. | **deník** – řekne, co jsi snědla, ne co uvařit; nutí zapisovat |
| **Toprecepty.cz** (CZ) | 3 mil. lidí měsíčně, 77 tis. receptů | bez kalorií v kontextu, člověk se ztratí |
| **Fitrecepty** (CZ) | 500 tis. stažení, kniha | bez osobního příjmu, ledničky a plánu |
| **Jídelní plán** (CZ) | 6 490 receptů s hodnotami, týdenní plány od 180 Kč | hlavně pro **diabetiky**, zdravotní tón |
| **NutritionPro** a krabičky | jídelníček na míru algoritmem, 5 000 receptů | 10 tis.+ měsíčně, nenaučí vařit |
| **Eat This Much, Samsung Food, Yazio** (svět) | automatické plány, AI fotka ledničky | anglicky, neosobní, neznají tvaroh ani Lidl |
| **Mealime** (svět) | jednoduchý týdenní plánovač | **končí 21. 10. 2026** – samotný plánovač bez obsahu se neuživí |

**Poučení z Mealime:** samotný plánovač bez obsahu a komunity se neuživí → appka musí stát na webu s recepty a články (to máme).

**Mezera na trhu:** nikdo v Česku nespojuje **kolik jíst + co uvařit z toho, co mám + co koupit** – bez zapisování, česky, jako kamarádka.

---

## 6. V čem jsme jiní

**Hlavní sdělení (návrh):**

> **„Jez s radostí, ne s výčitkami.“**
> Spočítáme, kolik potřebuješ. Uvaříš jeden základ a každý den ho jinak dochutíš. A sladká tečka je součást plánu.

Další varianty: „Kalorie spočítám já. Ty si jen uvař.“ · „Plánuj, nezapisuj.“

| # | Čím se lišíme | Proč to funguje |
|---|---|---|
| 1 | **Bez zapisování, bez výčitek** – plánuješ dopředu, nezapisuješ zpětně | výzkum o psychice; hlavní důvod odchodu z appek |
| 2 | **Jeden základ, tři varianty** | lidé nemají čas vařit každý den jinak |
| 3 | **Sladká tečka v plánu** | flexibilní kontrola = lepší výsledky |
| 4 | **Stavebnice talíře** | lidé chtějí tvořit, ale nevědí kolik čeho |
| 5 | **Recepty + appka + e-shop propojené** | uvař si sám, nebo kup hotové – stejný základ |
| 6 | **Pro každého** | přístupnost, alergie, nemoci, angličtina |
| 7 | **Skutečný člověk – Niky** | důvěra, kterou velké portály nemají |
| 8 | **Poctivost** | žádné falešné hodnocení ani zdravotní sliby |
| 9 | **Lednička, ze které nic nevyhodíš** | Češi vyhodí 37–57 kg jídla ročně – šetří peníze i jídlo |

---

## 7. Persony – pro koho to děláme

Přesunuto do samostatného souboru 👉 [PERSONY.md](PERSONY.md) – 7 person (Petra ⭐, Tomáš, Jana, Kája, Martin, Pavel, Emma) a jak je ověřit.

Cesty, kterými persony procházejí webem a appkou 👉 [FLOW.md](FLOW.md).

---

## 8. Hlavní koncepty

### 🥣 Jeden základ, tři varianty

Uvaříš základ na 3–4 dny a každý den ho jinak doplníš. Příklad:

| | Co přidat | Pro koho |
|---|---|---|
| **Základ** | pečená zelenina + quinoa | všichni |
| **Varianta A – sytá** | + kuřecí maso | nabírání, víc bílkovin |
| **Varianta B – rostlinná** | + cizrna a tahini | bez masa |
| **Varianta C – rychlá** | + feta a vejce | hotové za 5 minut |

* V appce: kcal a bílkoviny u každé varianty, přepočet na tvůj příjem.
* V nákupním seznamu: základ jen jednou + doplňky.
* V e-shopu: stejné varianty jako hotové bowly.

### 🍰 Sladká tečka

* V týdenním menu na konci dne nebo týdne **malá tečka** – sladká nebo slaná.
* Velikost do ~10 % denního příjmu (doporučení WHO).
* Je **součást plánu** – žádné výčitky, žádné „zasloužit si“.
* Na webu vlastní rubrika „Sladká tečka“.

### 🍽️ Stavebnice talíře

* Podle Harvardského talíře: ½ zelenina, ¼ příloha, ¼ bílkoviny + tuk.
* Vybereš si bílkovinu, přílohu a zeleninu → appka řekne **gramy podle tvého příjmu**.
* Můžeš být kreativní a přitom víš, kolik čeho dát.
* V e-shopu jako „**slož si svůj bowl**“.

### 🥡 Krabičky za cenu nákupu (vaření dopředu)

* „V neděli 2 hodiny vaření = 5 obědů.“
* Týdenní plán vybírá recepty se **společnými surovinami** → méně nákupu, méně vyhozeného jídla.
* Odhad ceny nákupu: „tenhle týden asi 900 Kč“ – proti krabičkám za 2 500 Kč.

---

## 9. Kalkulačka – jak počítat

### Dvě úrovně

**🟢 Jednoduchá (výchozí, pro každého)**

* Vstup: věk, výška, váha, pohlaví, **práce** (sedavá / na nohou / fyzická), **trénink** (0 / 1–2× / 3–6× týdně), cíl.
* Cíle: **hubnout / udržet / zpevnit (rekompozice) / nabrat**.
* BMR: Mifflin-St Jeor (jako dnes).
* Výsledek: kcal + talíř („~25 g bílkovin na jídlo“) + „Chci vidět detail ▾“.

**🔵 Pokročilá (rozkliknutím „Znám své % tuku / mám InBody“)**

* Vstup navíc: % tuku nebo změřený BMR, úroveň (začátečník / mírně pokročilý / pokročilý).
* BMR: **Katch-McArdle** = 370 + 21,6 × beztuková hmota (shoduje se s InBody).
* Výsledek: bílkoviny, tuky, sacharidy, vláknina v gramech, rozdělené do jídel.

### Vzorce (z Nikiny tabulky, ověřeno přepočtem)

| Co | Vzorec | Příklad |
|---|---|---|
| Denní příjem | BMR × násobek aktivity × přebytek/deficit | 1 341 × 1,3 × 1,1 = **1 918 kcal** |
| Bílkoviny | beztuková hmota × 2,2 g | 45 × 2,2 = **99 g** (= 1,87 g/kg váhy ✅ ISSN) |
| Tuky | 20–35 % příjmu ÷ 9, nebo váha × 0,66–1,1 g | 43–75 g, zvoleno **60 g** |
| Sacharidy | (kcal − bílkoviny × 4 − tuky × 9) ÷ 4 | (1 918 − 396 − 540) ÷ 4 = **245 g** |
| Vláknina | 25 g na 200 g sacharidů (EFSA min. 25 g/den) | **~31 g** |

### Násobky aktivity (z tabulky)

| Práce + trénink 3–6× týdně | Příklad | Násobek |
|---|---|---|
| Sedavá | kancelář | 1,2–1,5 |
| Lehká | prodavač, venčení psa | 1,5–1,8 |
| Střední | servírka, tenis | 1,8–2,0 |
| Vysoká | stavba, turistika | 2,0–2,2 |

*Konkrétní hodnoty pro appku je potřeba vybrat (appka dnes používá 1,2–1,9 v jedné volbě).*

### Přebytek / deficit (z tabulky)

| Úroveň | Nabrat | Zpevnit | Hubnout | Hubnout (vyšší % tuku) |
|---|---|---|---|---|
| Začátečník | ~25 % | udržovací | ~20 % | 21–30 % |
| Mírně pokročilý | 15–20 % | udržovací | ~20 % | 21–30 % |
| Pokročilý | 10–15 % | ±5–10 % | ~20 % | 21–30 % |

⚠️ **Návrh zmírnit:** přebytek 10–15 %, deficit 15–20 %. Větší deficit jen jako vědomá volba s vysvětlením. Deficit 30 % při násobku 1,2 vychází pod BMR.

### Srovnání: appka dnes × Nikina tabulka

| | Appka dnes | Nikina tabulka |
|---|---|---|
| BMR | Mifflin-St Jeor (váha, výška, věk) | InBody / beztuková hmota (přesnější) |
| Aktivita | 1 volba (1,2–1,9) | práce + trénink (1,2–2,2) |
| Cíle | hubnout / udržet / nabrat | + rekompozice a úroveň zkušeností |
| Makroživiny | ❌ nepočítá | ✅ bílkoviny, tuky, sacharidy, vláknina |
| Hubnutí | deficit 15 %, nikdy pod BMR | deficit 20–30 % |
| Nabírání | přebytek 10 % | přebytek 10–25 % |

### Na co si dát pozor

* **% tuku většina lidí nezná** → v appce jen nepovinně, jinak se uživatel zasekne a odejde.
* **Velké deficity se srazí s pravidlem „nikdy pod BMR“** – např. 1,2 × 0,7 = 0,84 × BMR.
* **Přebytek 25 % u začátečníků** je hodně – u netrénovaných jde spíš do tuku.
* **Zdroje tabulky** (RP Strength, Jeff Nippard) jsou uznávaní trenéři, ne vědecké studie; čísla u bílkovin a tuků ale s výzkumem souhlasí.
* Bílkoviny podle beztukové hmoty: 2,2 g/kg LBM vychází u příkladu na 1,87 g/kg celkové váhy – v rozmezí ISSN.
* Tuky 20–35 % příjmu odpovídají oficiálnímu doporučenému rozmezí (Institute of Medicine).
* Překlep v tabulce „Loose Fat“ → „Lose Fat“ (do appky půjde česky).

### Bezpečnostní pravidla (platí vždy)

* příjem **nikdy pod BMR**,
* **žádný deficit při podváze** (BMI pod 18,5) – laskavé vysvětlení + kontakt na Anabell,
* tuky minimálně 20 % příjmu,
* vždy poznámka: nejde o lékařskou radu.

### Filtry místo výpočtu

* **14 alergenů EU** (lepek, mléko, vejce, ořechy, arašídy, sója, ryby, korýši, měkkýši, celer, hořčice, sezam, oxid siřičitý, vlčí bob)
* vegetarián / vegan, bez lepku, bez laktózy
* **vhodné při cukrovce** – víc vlákniny, celozrnné přílohy, bez přidaného cukru
* **méně soli** – při vysokém tlaku
* **šetrné k trávení** *(upřesnit – viz otevřené otázky)*

### Nepočítat → odborník

Těhotenství a kojení · pod 18 let · cukrovka 1. typu (inzulin) · nemoci ledvin · podváha · poruchy příjmu potravy.

---

## 10. Mapa webu (sitemap)

Přesunuto do samostatného souboru 👉 [SITEMAP.md](SITEMAP.md) – mapa webu, appky a e-shopu, šablony stránek a propojení.

---

## 11. Aplikace Jídlo od A–Z

### Co umí dnes ✅

Profil a výpočet příjmu · Můj den · Lednička · Recepty s hledáním · Nákupní seznam · doporučené články · přidání na plochu mobilu. Omezení: 14 ukázkových receptů a kcal.

### Mapa appky (návrh)

```
Jídlo od A–Z
│
├── 👤 Profil
│     ├── Jednoduchá kalkulačka (práce + trénink, 4 cíle)
│     ├── Pokročilá ▾ (% tuku / InBody, úroveň, makroživiny)
│     ├── Zdraví a alergie (filtry)
│     └── Bezpečnostní pojistky
│
├── 📅 Můj den / Můj týden
│     ├── snídaně · oběd · večeře · svačina · 🍰 tečka
│     ├── „Vyměnit jídlo“ (stejné kcal)
│     ├── odškrtávání „snědla jsem ✓“ (ne zapisování)
│     └── týden se základem na víc dní (společné suroviny)
│
├── 🍽️ Stavebnice talíře
│     vyber bílkovinu + přílohu + zeleninu → gramy podle příjmu
│
├── 🧊 Lednička
│     co mám doma → co uvařím, co chybí
│
├── 📖 Recepty
│     základ + 3 varianty · filtry · režim „vaříme“
│
├── 🛒 Nákup
│     seznam z dne / týdne / ledničky · odhad ceny · (později) „kup hotové“
│
└── 🏅 Razítka a výzvy
      kuchařka s razítky · 1 změna týdně · bonusový recept
```

### Funkce podle priority (návrh)

| Priorita | Funkce |
|---|---|
| 1 | Víc skutečných receptů (aspoň 40–60) s kcal a bílkovinami – **největší slabina dnes** |
| 2 | Kalkulačka: práce + trénink, cíl „zpevnit“, bílkoviny |
| 3 | Týdenní plán + základ na víc dní + tečka |
| 4 | Stavebnice talíře |
| 5 | Zdravotní filtry a alergeny |
| 6 | Pokročilá kalkulačka (InBody, makroživiny) |
| 7 | Odškrtávání, razítka, výzvy |
| 8 | „Vyměnit jídlo“, odhad ceny nákupu |
| 9 | Angličtina |

---

## 12. Web a blog

### Co zlepšit

* **Recepty** ve formátu základ + 3 varianty, s kcal a bílkovinami, přepočet porcí, tlačítko „Přidej do mého dne“.
* **Články** s rámečkem „V kostce“ a rozkliknutím; štítek „čtení na 2 min“.
* **Nové rubriky:** Sladká tečka · Jeden základ, tři varianty · Krabičky za cenu nákupu.
* **SEO:** data receptů pro Google (čas, kcal); články na konkrétní hledané dotazy („večeře do 500 kcal z tvarohu“).
* **Důvěra:** příběh Niky na stránce O mně; pryč s falešnými hodnoceními.
* **Rychlost:** zmenšit fotky (WebP).
* **Přístupnost:** viz kap. 14.

### Nápady na články (návrh)

* Proč nemusíš zapisovat každé sousto
* Sladká tečka: proč si ji klidně dát
* Jak poskládat talíř (bez vážení)
* Kolik bílkovin vlastně potřebuješ
* Neděle v kuchyni: 2 hodiny = 5 obědů
* Jídlo při cukrovce / vysokém tlaku – jednoduše (s upozorněním, že nejde o lékařskou radu)
* Zdravý životní styl a mozek – co říká výzkum (poctivě)
* Czech ingredients explained (EN)

---

## 13. E-shop

> ✅ **Aktualizace 2026-10-03:** místo vařených krabiček **digitální produkty** (malý placený vstup → online kuchařka, e-booky, kurzy s online setkáními). Krabičky odloženy. Níže je původní úvaha. Aktuální stav je v `PROJEKT.md` a v Miru (rám 22).

### Co nabízet

* **Bowly a krabičky** ve stejných variantách jako recepty (základ + A/B/C).
* „**Slož si svůj bowl**“ podle stavebnice talíře.
* Propojení s appkou: „krabičky přesně na tvůj příjem“.

### Filtry a informace u produktu

cíl · kcal · bílkoviny · alergeny · vege · bez lepku · vhodné při cukrovce · cena · složení · příprava

### Realita (poctivě)

* Vlastní kuchyně = hygiena, provozovna, rozvoz, velké náklady; konkurence (NutritionPro) je silná.
* **Návrh postupu:**
  1. nejdřív obsah zdarma („Krabičky za cenu nákupu“) – ověří zájem,
  2. pak případně **spolupráce s existující krabičkovou firmou** (provize),
  3. vlastní e-shop až s publikem.

### Povinnosti

* **Alergeny musí být uvedené přímo u produktu** i při prodeji přes internet (EU 1169/2011) – „na vyžádání“ nestačí.
* Přístupnost e-shopu (zákon 424/2023 Sb.) – malé firmy jsou výjimkou, ale doporučeno dodržet.

---

## 14. Přístupnost a angličtina

### ♿ Přístupnost

* Standard **WCAG 2.1 AA** (vyžaduje ho zákon 424/2023 Sb. pro e-shopy od 28. 6. 2025; malé firmy výjimkou – dodržíme stejně).
* Popisky fotek (alt texty), dostatečný kontrast, ovládání klávesnicí.
* Postup receptu jako číslovaný seznam, informace nikdy jen barvou.
* Zvětšitelné písmo, omezení animací pro citlivé lidi.
* **Režim „vaříme“** – velké písmo, krok za krokem.
* Rozkliknutí přes HTML prvek `<details>` – funguje s klávesnicí i čtečkou.
* Prohlášení o přístupnosti na webu.

### 🇬🇧 Angličtina

* ✅ **Rozhodnuto 2026-10-03:** celý web i appka česky i anglicky, ne jen výběr. Cíl: web pro co nejvíc lidí, nikoho nevynechat.
* Texty od začátku psát jednoduše (norma ISO 24495-1) a ukládat odděleně od kódu, aby šly snadno přeložit.
* Přepínač jazyka na každé stránce.
* Navíc „**Czech ingredients explained**“ (tvaroh, pohanka, kde koupit v Albertu / Lidlu) – mezera, kterou nikdo nedělá.
* Data: v Praze žije ~25 % cizinců (ČSÚ).
* ✅ **Rozhodnuto 2026-10-03:** jen dva jazyky, další by zbytečně zatížily web.

---

## 15. Motivace bez tlaku

* **Razítka do kuchařky** – za uvařený recept nebo splněný týden.
* **„Týden s radostí ✓“** → odemknutí bonusového receptu.
* **1 malá změna týdně** – „tento týden přidej zeleninu k obědu“.
* **Překvapení** – nový recept týdne, sezónní výzva.
* **Bez trestů:** žádné „ztratila jsi sérii“, žádné žebříčky vah.
* **První týden** je klíčový – appka musí pomoct hned 1. den.

---

## 16. Kdo – co – proč

| Kdo | Co | Proč |
|---|---|---|
| **Niky** | recepty, fotky, kcal na porci, články, příběh, rozhodnutí | je tvář projektu – důvěra a osobní tón |
| **Claude** | kód webu a appky, průzkum, kontrola zdrojů, přístupnost | technická práce a ověřování |
| **Nutriční terapeut/ka** *(návrh)* | kontrola kalkulačky, zdravotních filtrů a článků o nemocech | bezpečnost a důvěryhodnost |
| **Testeři z cílovky** *(návrh)* | vyzkoušet appku (Petra, Tomáš, Pavel se čtečkou…) | zjistit, co je matoucí |
| **Partnerská krabičková firma** *(později)* | výroba a rozvoz | e-shop bez vlastní kuchyně |

---

## 17. Zákony a rizika

### Zákony

| Předpis | Co znamená pro nás |
|---|---|
| **EU 1924/2006** (zdravotní tvrzení) | nesmíme psát, že jídlo předchází nemocem nebo je léčí („proti demenci“, „léčí cukrovku“) |
| **EU 1169/2011** (informace o potravinách) | alergeny u každého produktu v e-shopu |
| **Zákon 424/2023 Sb.** (přístupnost) | e-shopy přístupné podle WCAG 2.1 AA; malé firmy výjimkou |
| **Ochrana osobních údajů** | údaje o zdraví a váze jsou citlivé – dnes jsou jen v prohlížeči (localStorage), tak to zůstane, dokud nebude jasné řešení |

### Rizika a slabiny

* Na projektu pracuje jen Niky.
* Recepty jsou zatím ukázkové (14) – omezuje to všechno ostatní.
* Appka nemá účty – data se nepřenesou mezi mobilem a počítačem.
* Web zatím není online.
* Kalkulačka může ublížit lidem s poruchou příjmu potravy → bezpečnostní pojistky.
* Zdravotní filtry nesmí působit jako lékařská rada.

---

## 18. Návrh pořadí práce

1. **Recepty s kcal a bílkovinami** (základ + 3 varianty) – bez nich nefunguje nic dalšího.
2. **Web:** skutečné články s „V kostce“, oprava receptů, pryč falešná hodnocení, zmenšit fotky.
3. **Přístupnost** webu i appky.
4. **Web online.**
5. **Kalkulačka:** práce + trénink, cíl „zpevnit“, bílkoviny, bezpečnostní pojistky.
6. **Týdenní plán** se základem na víc dní a tečkou.
7. **Stavebnice talíře.**
8. **Zdravotní filtry a alergeny.**
9. **Pokročilá kalkulačka** (InBody, makroživiny).
10. **Razítka a výzvy.**
11. **Angličtina.**
12. **E-shop** – nejdřív ověřit zájem, pak spolupráce.

---

## 19. Otevřené otázky

1. Hlavní sdělení: „**Jez s radostí, ne s výčitkami**“, „Kalorie spočítám já. Ty si jen uvař.“, nebo „Plánuj, nezapisuj“?
2. Marketing postavit hlavně na **Petře**?
3. Tečka jako „**součást plánu**“ místo „zasloužila sis“?
4. Kalkulačka ve **dvou úrovních** (jednoduchá + pokročilá)?
5. Přidat cíl **„zpevnit“** (rekompozice)?
6. Přebytek a deficit **z tabulky**, nebo **zmírnit** (10–15 % / 15–20 %)?
7. Je kalkulační tabulka tvoje (nebo od trenéra), nebo ji můžeme citovat jako zdroj (RP Strength, Jeff Nippard)?
8. Co jsi myslela tou „**sliznicí**“ – žaludek (gastritida), nebo slinivka?
9. E-shop: nejdřív obsah „**Krabičky za cenu nákupu**“, pak spolupráce?
10. Zapojit **nutričního terapeuta** na kontrolu?
11. Souhlasíš s **pořadím práce** v kap. 18?

---

## 20. Zdroje

### Vědecké studie (PubMed)

* Simpson & Mazzeo (2017) – Calorie counting and fitness tracking technology: associations with eating disorder symptomatology. [DOI](https://doi.org/10.1016/j.eatbeh.2017.02.002)
* Levinson a kol. (2017) – My Fitness Pal calorie tracker usage in the eating disorders. [DOI](https://doi.org/10.1016/j.eatbeh.2017.08.003)
* Westenhoefer a kol. (1999) – Validation of the flexible and rigid control dimensions of dietary restraint. [DOI](https://doi.org/10.1002/(sici)1098-108x(199907)26:1<53::aid-eat7>3.0.co;2-n)
* Timko & Perone (2005) – Rigid and flexible control of eating behavior in a college population. [DOI](https://doi.org/10.1016/j.eatbeh.2004.09.002)
* Nishi a kol. (2024) – Digital health apps with or without gamification: meta-analysis. [DOI](https://doi.org/10.1016/j.eclinm.2024.102798)
* Davis a kol. (2021) – Gamified applications for secondary prevention. [DOI](https://doi.org/10.1111/jocn.15808)
* Livingston a kol. (2024) – Dementia prevention, intervention, and care: Lancet Commission. [DOI](https://doi.org/10.1016/S0140-6736(24)01296-0)
* Barnes a kol. (2023) – Trial of the MIND Diet, NEJM. [DOI](https://doi.org/10.1056/NEJMoa2302368)
* Jäger a kol. (2017) – ISSN Position Stand: protein and exercise. [DOI](https://doi.org/10.1186/s12970-017-0177-8)

### Česká data a zákony

* [Deník – 64 % Čechů s nadváhou](https://www.denik.cz/zdravotnictvi/obezita-cesi-pruzkum-lecba.html) · [SZÚ – nadváha](https://szu.gov.cz/aktuality/vice-nez-60-procent-cechu-ma-nadvahu-trpi-ji-az-ctvrtina-deti-obezita-zpusobuje-zavazne-zdravotni-komplikace/)
* [VZP – hypertenze](https://www.vzp.cz/o-nas/aktuality/hypertenze-tichy-nepritel-ktery-ohrozuje-zdravi-milionu-cechu) · [MZd – kardiovaskulární studie](https://mzd.gov.cz/wp-content/uploads/2025/01/Priloha-3_NKV_plan-souhrnna-analyticka-studie.pdf)
* [SZÚ – cukrovka](https://archiv.szu.cz/zhruba-milion-cechu-trpi-cukrovkou-a-nemocnych-neustale) · [Aktuálně – diabetici](https://zpravy.aktualne.cz/domaci/v-cesku-uz-je-pres-milion-diabetiku/r~e9ce707437ff11eda25a0cc47ab5f122/?lp=1)
* [Medicína pro praxi – celiakie](https://www.medicinapropraxi.cz/pdfs/med/2011/09/03.pdf)
* [ČSÚ – počet cizinců](https://csu.gov.cz/pocet-cizincu-demograficke-udalosti) · [Statistická ročenka Prahy 2025](https://csu.gov.cz/produkty/statisticka-rocenka-hl-m-prahy-2025)
* [ČSÚ – plýtvání v domácnostech](https://statistikaamy.csu.gov.cz/plytvani-potravinami-v-ceskych-domacnostech) · [iRozhlas – generace Z](https://www.irozhlas.cz/zivotni-styl/spolecnost/nejvic-se-na-plytvani-jidlem-podileji-domacnosti-nejhorsi-je-v-tom-generace-z_2406021343_pj)
* [NZIP – označování alergenů](https://www.nzip.cz/clanek/364-povinne-oznacovani-potravin-obsahujicich-alergeny) · [SZPI – alergeny](https://www.szpi.gov.cz/clanek/povinnost-provozovatelu-zarizeni-spolecneho-stravovani-poskytovat-informace-o-alergennich-slozkach.aspx)
* [Shop5 – zákon o přístupnosti](https://www.shop5.cz/clanek/faq-pristupnost-e-shopu-a-zakon-c-424-2023-sb-na-koho-se-skutecne-vztahuje/) · [Animato – EAA 2025](https://www.animato.cz/blog/eaa-2025)

### Trh a konkurence

* [Kalorické Tabulky – Wikipedie](https://cs.wikipedia.org/wiki/Kalorick%C3%A9_Tabulky_(aplikace)) · [Kalorické Tabulky Premium](https://www.kaloricketabulky.cz/user/premium/public)
* [Nutrola – proč lidé opouštějí appky](https://nutrola.app/en/blog/120k-first-app-churn-90-day-data-report-2026) · [Macrite](https://macrite.app/blog/why-80-percent-quit-calorie-tracking)
* [Forbes – NutritionPro](https://forbes.cz/krabicky-na-dracku-nutritionpro-trha-rekordy-a-jde-za-hranice/) · [Testado – krabičkové diety](https://www.testado.cz/nejlepsi-krabickova-dieta/) · [Ecoblog – ceny krabiček](https://ecoblog.cz/krabickova-dieta-ostrava)
* [Toprecepty – inzerce](https://www.toprecepty.cz/inzerce) · [Pixelmate – Fitrecepty](https://pixelmate.cz/reference-fitrecepty) · [Jídelní plán](https://www.jidelniplan.cz/)
* [MealThinker – srovnání plánovačů 2026](https://mealthinker.com/blog/best-ai-meal-planning-apps-2026) · [SummitPlate](https://www.summitplate.com/guides/best-ai-meal-planning-apps-2026) · [Grand View Research](https://www.grandviewresearch.com/industry-analysis/diet-nutrition-apps-market-report)
* [Harvard Health – zdravý talíř](https://content.health.harvard.edu/blog/the-harvard-healthy-eating-plate-or-what-does-a-healthy-plate-look-like)
* [Lancet – tisková zpráva (EurekAlert)](https://www.eurekalert.org/news-releases/1052982)

### Kalkulační tabulka

* Nikina tabulka podle [RP Strength](https://rpstrength.com) a [Jeff Nippard](https://jeffnippard.com) – praktická pravidla trenérů, čísla u bílkovin a tuků souhlasí s výzkumem.
