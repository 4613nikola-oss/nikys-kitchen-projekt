# Sitemap – mapa webu, appky a e-shopu

Návrh struktury celého Niky's Kitchen. **Jsou to návrhy, ne rozhodnutí** – co odsouhlasíme, jde do `PROJEKT.md`.
Legenda: ✅ existuje · 🔧 existuje, potřebuje úpravu · 🆕 nové · ⏳ později

← zpět na [DASHBOARD](DASHBOARD.md)

---

## 1. Celkový přehled

```
                         NIKY'S KITCHEN
                               │
      ┌────────────────────────┼────────────────────────┐
   🌐 WEB                  📱 APPKA                 🛒 E-SHOP ⏳
   recepty, články,        Jídlo od A–Z             bowly a krabičky
   příběh Niky             (sekce webu)             (sekce webu)
      │                        │                        │
      └──── recept → „Přidej do mého dne“ → appka ──────┤
      └──── recept → „Kup hotové“ ──────────────────────┘
      └──── appka → nákupní seznam / „kup hotové“ ──────┘
```

---

## 2. Web

```
/  🏠 Domů 🔧
│   hlavní sdělení · recepty týdne · „Spočítej si příjem“ (appka) ·
│   Jeden základ, tři varianty · Sladká tečka · O Niky (krátce) · e-shop ⏳
│
├── /recepty/  🍲 Recepty
│   ├── slane.html ✅🔧        Slané
│   ├── sladke.html ✅🔧       Sladké
│   │   └── sladka-tecka 🆕    Sladká tečka (rubrika)
│   ├── napoje.html ✅🔧       Nápoje
│   ├── zaklad-a-varianty 🆕   Jeden základ, tři varianty
│   ├── vareni-dopredu 🆕      Krabičky za cenu nákupu
│   ├── filtry 🆕              alergeny · vege · bez lepku · bez laktózy ·
│   │                          vhodné při cukrovce · méně soli · čas · kcal
│   └── /recepty/<recept> 🔧   Detail receptu (viz níž)
│
├── clanky.html 🔧  📖 Články
│   ├── kategorie 🆕: hubnutí · svaly · psychika a jídlo · zdraví · rychlá kuchyně
│   └── /clanky/<clanek> 🔧   Detail článku (viz níž)
│
├── /aplikace/ 🔧  📱 Jídlo od A–Z (dnes samostatně, později součást webu)
│
├── /eshop/ ⏳  🛒 E-shop (viz kap. 4)
│
├── galerie.html 🔧  🖼️ Galerie
├── o-mne.html 🔧    👩‍🍳 O mně – příběh Niky, proč to dělá
├── pristupnost 🆕   ♿ Prohlášení o přístupnosti
├── upozorneni 🆕    ⚖️ Nejde o lékařskou radu · zásady soukromí
│
└── /en/ 🆕  🇬🇧 English – celý web i appka (přepínač CZ/EN na každé stránce)
    └── czech-ingredients  Czech ingredients explained (navíc)
```

### Šablona: detail receptu

1. Název, fotka (s popiskem pro čtečku), ⏱ čas · 🔥 kcal · 💪 bílkoviny
2. **V kostce** – 3 věty
3. Alergeny (ikony + text)
4. Suroviny – s přepočtem porcí
5. **Základ** + **Varianta A / B / C**
6. Postup – číslovaný seznam · tlačítko **režim „vaříme“**
7. Tlačítka: **Přidej do mého dne** (appka) · **Kup hotové** (e-shop ⏳)
8. Tip od Niky · podobné recepty

### Šablona: detail článku

1. Nadpis · štítek „čtení na X min“
2. **V kostce** – 3 body
3. **Chci vědět víc ▾** – celý text (HTML `<details>`)
4. Zdroje (u zdravotních témat povinně)
5. Upozornění, že nejde o lékařskou radu (zdravotní témata)
6. Související recepty / „vyzkoušej v appce“

---

## 3. Appka Jídlo od A–Z

```
Jídlo od A–Z
│
├── 👤 Profil ✅🔧
│   ├── Jednoduchá kalkulačka 🔧 (práce + trénink, 4 cíle vč. „zpevnit“)
│   ├── Pokročilá ▾ 🆕 (% tuku / InBody, úroveň, makroživiny)
│   ├── Zdraví a alergie 🆕 (filtry)
│   └── Bezpečnostní pojistky 🔧
│
├── 📅 Můj den ✅ → Můj týden 🆕
│   ├── snídaně · oběd · večeře · svačina · 🍰 tečka 🆕
│   ├── Vyměnit jídlo 🆕
│   ├── Odškrtávání „snědla jsem ✓“ 🆕
│   └── Týden se základem na víc dní 🆕
│
├── 🍽️ Stavebnice talíře 🆕
├── 🧊 Lednička ✅
├── 📖 Recepty ✅🔧 (varianty, filtry, režim „vaříme“)
├── 🛒 Nákup ✅🔧 (týden, odhad ceny, „kup hotové“ ⏳)
└── 🏅 Razítka a výzvy 🆕
```

---

## 4. Obchod – digitální produkty ⏳

✅ 2026-10-03: místo vařených krabiček digitální produkty (krabičky odloženy).

```
/obchod/
│
├── Malý vstup (asi 99–199 Kč, návrh)
│   mini e-book · plán na 7 dní (jeden základ, tři varianty, nákupní seznam)
│
├── Hlavní nabídka
│   ├── Online kuchařka s plány
│   ├── E-booky (i pro starší, PDF i tisk, jde darovat)
│   └── Kurz vaření dopředu se živými online setkáními
│
├── Pro věrné
│   předplatné nových plánů · komunita · workshopy
│
├── Detail produktu
│   co v něm je · pro koho · ukázka · cena · objednat (formulář FAPI)
│
└── Právní stránky
    obchodní podmínky · odstoupení od smlouvy u digitálního obsahu ·
    ochrana osobních údajů · prohlášení o přístupnosti
```

---

## 5. Hlavní propojení (odkazy mezi částmi)

| Odkud | Kam | Proč |
|---|---|---|
| Recept | Appka – Můj den | „Přidej do mého dne“ |
| Článek | Obchod – malý vstup | „Chceš plán na celý týden?“ |
| Článek | Recepty / appka | od teorie k praxi |
| Appka – Nákup | Obchod – plán na 7 dní | hotový týden s nákupním seznamem |
| Appka – Profil | Články | doporučené články podle cíle (už funguje) |
| Obchod – produkt | Recepty | ukázka zdarma |
