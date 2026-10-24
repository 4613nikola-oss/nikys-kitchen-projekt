# Flow – jak uživatel prochází webem a appkou

Kroky, kterými lidé projdou. Pomáhá navrhnout obrazovky a nezapomenout na nic. **Návrhy, ne rozhodnutí.**
Vizuálně v Miru: rámy 4, 5, 6, 18, 24 a 25.

← zpět na [DASHBOARD](DASHBOARD.md)

---

## 0. Celek: web → appka → obchod (Miro rám 24)

```
Google · Instagram a Pinterest · doporučení
        │
        ▼
🌐 Web: recept nebo článek ◄────────────── „Recept do mého dne“
        │                                         │
        ├── „Kolik z toho sníst?“ ──► 📱 Appka zdarma (kalkulačka, Můj den)
        │                                         │
        └── „Chci víc receptů“ ──► ✉️ E-mail (odběr se souhlasem)
                                                  │
              „Chci plán na celý týden“ ◄─────────┤
                        │                         │ tip a nabídka
                        ▼                         ▼
              🛒 Malý produkt: plán na 7 dní (asi 99–199 Kč)
                        │  e-mail od Niky po pár dnech
                        ▼
              🛒 Hlavní produkt: online kuchařka, kurz, e-book
                        │                 └─ QR kód a odkazy zpět do appky
                        ▼
              💚 Věrní: předplatné, komunita ──► sdílí a doporučí dál ──► (zpět nahoru)
```

## 0b. Data a nástroje (Miro rám 25)

```
Pages CMS (Niky přidá recept formulářem)
        │
        ▼
Recepty v jednom souboru dat ──► Web · Appka · E-booky a plány (PDF)
                                   │
Appka: profil a plán zůstávají jen v prohlížeči uživatele (žádná databáze)
                                   │
Tlačítko „Koupit“ (web, appka) ──► FAPI: objednávka, platba, faktura
                                   ├──► e-mail zákazníkovi s produktem a fakturou
                                   └──► e-mailing s novinkami (jen se souhlasem; napojení ověřit)
Web a appka ──► měření návštěvnosti + Search Console ──► Niky vidí, co zlepšit
```

---

## 1. Z Googlu k prvnímu plánu (hlavní cesta – Petra)

```
Google: „rychlá zdravá večeře“
        │
        ▼
Detail receptu na webu ── vidí ⏱ čas, 🔥 kcal, 💪 bílkoviny, V kostce
        │
        ▼
„Kolik z toho mám sníst?“ ──► appka: Profil (jednoduchá kalkulačka, < 60 s)
        │
        ▼
Výsledek: tvůj příjem + talíř („~25 g bílkovin na jídlo“)
        │
        ▼
Můj den ── recept už je v něm, doplní se zbytek dne + 🍰 tečka
        │
        ▼
Nákupní seznam ──► nakoupí ──► uvaří ✓
```

**Cíl:** užitek hned první den (výzkum: rozhoduje první týden).

---

## 2. Onboarding appky (první spuštění)

```
Vítej ── „Spočítám, kolik potřebuješ. Ty si jen uvaříš.“
   │
   ▼
Profil: věk · výška · váha · pohlaví · práce · trénink · cíl
   │
   ├── bezpečnostní kontrola (viz flow 6) ──► případně laskavé vysvětlení
   │
   ▼
Alergie a omezení? (nepovinné, přeskočitelné)
   │
   ▼
Výsledek + „Chci vidět detail ▾“
   │
   ▼
Můj den – hotový návrh
```

---

## 3. Týden se základem na víc dní (Petra, Tomáš)

```
Neděle: Můj týden ── appka navrhne 2 základy na týden (společné suroviny)
   │
   ▼
Nákup na týden ── odhad ceny („asi 900 Kč“)
   │
   ▼
Vaření základů (2 hodiny)
   │
   ▼
Po–Pá: každý den jiná varianta (A sytá · B rostlinná · C rychlá)
   │        └── „snědla jsem ✓“ (odškrtnutí, žádné zapisování)
   │        └── „Vyměnit jídlo“ (stejné kcal)
   ▼
Konec týdne: 🍰 sladká tečka v plánu ── 🏅 razítko „Týden s radostí ✓“
```

---

## 4. Lednička → recept → nákup (Kája)

```
Lednička: zadá, co má doma (tvaroh, vejce, rajčata…)
   │
   ▼
„Uvaříš hned“ / „Chybí 1–2 věci“
   │
   ├── vybere recept ──► režim „vaříme“ ──► ✓ + 🏅 razítko
   │
   └── chybí věci ──► přidat do nákupu
```

---

## 5. Stavebnice talíře (Martin, kreativní typy)

```
Vyber bílkovinu (kuře, tofu, vejce, cizrna…)
   │
   ▼
Vyber přílohu (celozrnná rýže, brambory, quinoa…)
   │
   ▼
Vyber zeleninu (1–2 druhy)
   │
   ▼
Appka spočítá gramy podle tvého příjmu
   ½ zelenina · ¼ příloha · ¼ bílkoviny + tuk
   │
   ▼
Uložit jako recept / přidat do dne / „kup jako bowl“ (e-shop ⏳)
```

---

## 6. Bezpečnostní pojistky kalkulačky

```
Zadané údaje
   │
   ├── věk < 18 ──────────────► „Appka je pro dospělé.“ (nic nepočítá)
   ├── těhotenství / kojení ──► „Poraď se s lékařem nebo nutričním terapeutem.“
   ├── BMI < 18,5 + hubnout ──► laskavé vysvětlení, žádný deficit,
   │                            kontakt na Anabell
   ├── zdravotní omezení ─────► jen filtry receptů + „nejde o lékařskou radu“
   │
   ▼
Výpočet: příjem nikdy pod BMR · tuky min. 20 %
```

---

## 7. Obchod – digitální produkty ⏳

```
Článek / appka ── „Chceš plán na celý týden?“
   │
   ▼
Malý vstup (mini e-book, plán na 7 dní) ── formulář FAPI ── platba
   │
   ▼
E-mail s produktem a fakturou (FAPI pošle samo)
   │
   ▼
Za pár dní e-mail od Niky ── nabídka hlavního produktu (kuchařka, kurz)
```

---

## 8. Přístupnost – cesta se čtečkou (Pavel)

```
Tab ► „Přeskočit na obsah“
   │
   ▼
Nadpis receptu (h1) ► V kostce ► Alergeny ► Suroviny (seznam)
   │
   ▼
„Spustit režim vaříme“ (tlačítko s názvem)
   │
   ▼
Krok 1 z 6 ► Další krok (klávesa) ► … ► Hotovo
```

**Kontrola:** každou novou stránku projít jen klávesnicí.

---

## 9. Článek pro netrpělivé (Kája)

```
Karta článku: nadpis · „čtení na 2 min“
   │
   ▼
V kostce (3 body) ── stačí? konec ✓
   │
   ▼
„Chci vědět víc ▾“ ── celý text
   │
   ▼
Související recept / „vyzkoušej v appce“
```
