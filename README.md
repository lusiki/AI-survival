# Strojevi Koji Pišu Kod

**Od modela do agenata i primjene**

Sveobuhvatni pregled suvremene kodne inteligencije na hrvatskom jeziku. Tekst pokriva cijeli životni ciklus velikih jezičnih modela za kod — od arhitektura i pretreniranja, preko evaluacije i usklađivanja, do agenata, sigurnosti i primjene u stvarnom softverskom inženjerstvu.

## Čitanje

| Format | Poveznica |
|--------|-----------|
| **HTML** (preporučeno) | [Otvori online](https://lusiki.github.io/AI-survival/) |
| **PDF** | [Preuzmi PDF](docs/kodna_inteligencija.pdf) |

> Zamijenite `lusiki` s vašim GitHub korisničkim imenom nakon što omogućite GitHub Pages.

## Sadržaj

Tekst je organiziran u devet poglavlja.

1. **Uvod** &mdash; Četiri epohe razvoja softvera i motivacija za kodnu inteligenciju
2. **Temeljni modeli za kod** &mdash; Opći LLM-ovi, arhitekture (dense, MoE, rekurentni, difuzijski, hibridni), multimodalnost, ograničenja; specijalizirani zatvoreni i otvoreni modeli kroz četiri evolucijske faze
3. **Zadaci, mjerila i evaluacija** &mdash; Metrike (Pass@k, CodeBLEU, execution-based), zadaci na razini funkcije i repozitorija
4. **Usklađivanje** &mdash; Nadzirano fino ugađanje (SFT), hladni start i destilacija rezoniranja, višejezično i multimodalno generiranje, pojačano učenje (PPO, DPO, GRPO), RLVR
5. **Agenti za softversko inženjerstvo** &mdash; Agenti kroz životni ciklus (zahtjevi, razvoj, testiranje, održavanje), opći SWE agenti, tehnike treniranja, budući trendovi
6. **Kod za generalističke agente** &mdash; Protokoli interakcije (MCP, A2A), agentske sposobnosti (razmišljanje, djelovanje, pamćenje u kodu), sučelja okruženja
7. **Sigurnost** &mdash; Sigurnost pretreniranja i posttreniranja, crveni tim, strategije ublažavanja
8. **Recepti za treniranje** &mdash; Distribuirani okviri, smjernice za pretreniranje, SFT i RL
9. **Primjena** &mdash; IDE pomoćnici, oblak platforme, terminalni agenti, popravak koda, PR pregled

## Datoteke

| Datoteka | Opis |
|----------|------|
| [`kodna_inteligencija.qmd`](kodna_inteligencija.qmd) | Izvorni Quarto dokument (631 redaka) |
| [`references.bib`](references.bib) | BibTeX bibliografija s 28 referenci |
| [`docs/index.html`](docs/index.html) | Renderirani HTML za GitHub Pages |
| [`docs/kodna_inteligencija.pdf`](docs/kodna_inteligencija.pdf) | Renderirani PDF |
| [`source/chapters/`](source/chapters/) | Izvorni Word dokumenti po poglavljima (9 datoteka) |

## Struktura repozitorija

```
.
├── kodna_inteligencija.qmd    # Izvorni Quarto dokument
├── references.bib             # BibTeX bibliografija
├── docs/                      # Renderirani izlaz (GitHub Pages)
│   ├── index.html
│   ├── kodna_inteligencija.pdf
│   └── kodna_inteligencija_files/
├── source/
│   └── chapters/              # Izvorni Word dokumenti po poglavljima
├── .gitignore
└── README.md
```

## Lokalno renderiranje

Potreban je [Quarto](https://quarto.org/docs/get-started/) (≥ 1.4).

```bash
quarto render kodna_inteligencija.qmd --to html
quarto render kodna_inteligencija.qmd --to pdf
```

Za PDF izlaz potreban je LaTeX (TinyTeX se preporučuje).

```bash
quarto install tinytex
```

## GitHub Pages

Ovaj repozitorij koristi `docs/` mapu za GitHub Pages. Za aktiviranje:

1. Otvorite **Settings** → **Pages** u repozitoriju
2. Pod **Source** odaberite **Deploy from a branch**
3. Odaberite granu `main` i mapu `/docs`
4. Sačekajte minutu, stranica će biti dostupna na `https://lusiki.github.io/AI-survival/`

## Izvor

Tekst se temelji na preglednom radu *From Code Foundation Models to Agents and Applications: A Comprehensive Survey and Practical Guide to Code Intelligence* ([arXiv:2511.18538](https://arxiv.org/abs/2511.18538)), proširen i adaptiran u narativnom obrazovnom stilu na hrvatskom jeziku.

## Licencija

Sadržaj je namijenjen obrazovnoj upotrebi. Izvorni pregledni rad podliježe vlastitoj licenci.
