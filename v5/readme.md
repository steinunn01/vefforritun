# Vefforritun 1, 2025: Verkefni 5, CSS #3

## Markmið

- Útfæra skalanlegan vef.
- Nota grid til að stýra útliti.
- Útfæra „dark mode“ og „light mode“.

## Verkefni 2–6

Í verkefnum 2–6 munum við vinna áfram með sama verkefni og byggja ofan á það:

- [Verkefni 2](https://github.com/vefforritun/vef1-2025-v2) skilgreinir grunn HTML og síður.
- [Verkefni 3](https://github.com/vefforritun/vef1-2025-v3) bætir við grunn viðmóti.
- [Verkefni 4](https://github.com/vefforritun/vef1-2025-v4) setur upp skipulagðra útlit.
- [Verkefni 5](https://github.com/vefforritun/vef1-2025-v5) setur upp grind og gerir útlit skalanlegt (e. responsive).
- [Verkefni 6](https://github.com/vefforritun/vef1-2025-v6) setur upp tól til að hjálpa við skipulag og vinnu.

## Lýsing

Verkefnið er framhald af [verkefni 2](https://github.com/vefforritun/vef1-2025-v2), [verkefni 3](https://github.com/vefforritun/vef1-2025-v3) og [verkefni 4](https://github.com/vefforritun/vef1-2025-v4), nýtir það efni sem uppsett er í því, og fylgir þeirri verkefnalýsingu. Leyfilegt er að nota sýnilausnir: [sýnilausn að verkefni 2](https://github.com/vefforritun/vef1-2025-v2-synilausn), [sýnilausn að verkefni 3](https://github.com/vefforritun/vef1-2025-v3-synilausn) eða [sýnilausn að verkefni 4](https://github.com/vefforritun/vef1-2025-v4-synilausn) sem gefin verður út föstudaginn 19. september.

## Grunnur

Gefið er `styles.css` skjal með grunn að lausn og athugasemdum svipað og í verkefnum 3 og 4. Sama og gilti almennt þar gildir áfram.

Gefið er `grid.css` skjal með „grid overlay“ sem er vísað í í HTML skrám og sést á fyrirmyndum.

Nota skal skilgreind CSS custom properties sem gefin eru í `styles.css`, búið er að bæta við skilgreiningum frá verkefni 4.

## Útlit

Fyrirmyndir að útliti er í `fyrirmynd/` möppu. Öll skjáskot eru tekin í `450px`, `700px` og `1200px` breiðum Firefox vafra.

Lýsing á útliti er að mestu endurtekin úr verkefni 4 en merkt er þar sem eitthvað breytist sérstaklega út frá því.

### Grind

Nota skal CSS grid til að setja upp grunn skipulag síðunnar. Nota skal 12 dálka og `30px` bil á milli dálka (gutter). „Offset“ frá vinstri og hægri skal vera `20px`. Þessar stærðir eru gefnar í `styles.css` sem CSS custom properties.

### Skalanleiki

Gera þarf síðuna skalanlega og hugsa um að hún virki vel í öllum stærðum frá og með `400px`. Í sýnilausn og fyrirmynd eru brotpunktar:

- Frá og með `550px`.
- Frá og með `700px`.
- Frá og með `900px`.

### Dark mode

Í „dark mode“ skal nota litina, þeim snúið við m.v. almenna lýsingu.

- Svartan sem bakgrunnslit: `#000000`.
- Hvítan sem textalit: `#ffffff`.
- Accent lit sem `#660000`.
- Protection lit sem `rgba(255, 255, 255, 0.5)`.

Fyrirmyndir af útliti í „dark mode“ má sjá í `fyrirmynd/` möppu:

- [Forsíða í dark mode](./fyrirmynd/forsida-dark-1200x1000.png)
- [Um síða í dark mode](./fyrirmynd/um-dark-1200x1000.png)
- [Sýningarsíða í dark mode](./fyrirmynd/syningar-dark-1200x1000.png)
- [Skráningarsíða í dark mode](./fyrirmynd/skraning-dark-1200x1000.png)

### Meginmál

Meginmál fyllir út í skjá.

Allt efni á að vera að hámarki `1100px` breitt (var `900px`) og miðjað í vafra, auka pláss vinstra og hægra megin skal sjálfkrafa vera útdeilt.

### Valmynd

- Valmynd er föst efst á síðu og fylgir þegar skrunað (scroll) er.
- Valmynd skal ná yfir alla breidd skjásins.
- Leturgerð skal vera Atkinson Hyperlegible.
- Leturstærð skal vera 24px, skilgreint í `rem`.
- Efni í valmynd skal vera miðjað (centered). Breytt frá verkefni 3:
  - Hér skal ekki nota `inline-block` og `text-align` til að ná því fram.
  - Nota skal `flexbox` til að miðja textann.
- Þegar tengill í valmynd er valinn með því að nota tab (`active`) eða sveimað er yfir (`hover`) skal setja undirstrik undir viðkomandi tengil.
- Núverandi síða skal vera með undirlínu (og er ekki tengill).

Í minni skjástærðum skal leturstærð vera stærð meginmáls letur en stækka í leturstærð fyrir fyrirsagnir í stærri skjástærðum (ykkar ákvörðun nákvæmlega hvenær). Einnig skal eingöngu sýna „Um“ og „Skráning“ í minni skjástærðum, ekki „Um safnið“ og „Skráning á sýningu“.

### Haus síðu

Haus (header) síðu skal vera með heiti síðu miðjað og leturstærð 48px, skilgreint í `rem`.

### Fótur

Efni í fæti skal vera skipt í þrennt með bili á milli og:

- Bakgrunnur skal vera með litnum `#ff9999`.
- Bil frá efni skal vera á allar hliðar innan fætar eitt bil.
- Eitt bil skal vera undir hverri fyrirsögn og milli staða í „Hafa samband“.
- Nota skal `flexbox` til að ná þessu fram, ef ekki er pláss fyrir efni skal það fara í nýja línu (wrap).

### Takkar

Nota skal sama útlit á „tökkum“ á forsíðu og „Skráningarsíðu“. Athugið að þó um takka _útlit_ sé að ræða þá skal athuga hvaða element eiga við merkingarfræðilega.

- Bil innan takka (padding) skal vera bil á hliðum og hálft bil fyrir ofan og neðan.
- Takki skal vera með svartan bakgrunn (secondary litur) og hvítan texta (primary litur).
- Takki skal hafa 5px border radíus.
- Leturstærð skal vera sama og á meginmáli (`16px` í rem).

### Forsíða

- [Forsíða í `1200px`](./fyrirmynd/forsida-1200x1000.png)
- [Forsíða í `700px`](./fyrirmynd/forsida-700x900.png)
- [Forsíða í `450px`](./fyrirmynd/forsida-450x700.png)

Haus er öðruvísi á forsíðu:

- Allan skjá skal hylja með [bakgrunnsmynd](./myndir/background.jpg):
  - Lýsing á mynd: Stakur sófi snýr að vegg, á veggnum eru mjög mörg listaverk í allskonar römmum. Einnig sést í vegg hægra megin við sófann, á honum eru líka mörg listaverk.
  - [Frá Unsplash](https://unsplash.com/photos/brown-loveseat-surrounded-by-photo-frame-lot-VbI0LMaGMlg?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash) eftir [Mick Haupt](https://unsplash.com/@rocinante_11?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash).
- Þegar skrollað er niður síðu skal bakgrunnsmynd vera föst (fixed).
- Mynd skal birta frá (position) miðju hennar, ekki frá efra vinstra horni.
- Myndin skal hylja allt pláss (cover) og ekki endurtaka sig (repeat).
- Yfir mynd en undir efni (stilla með z-index) skal vera hálfgegnsætt lag sem gerir það að verkum að texti er læsilegur (annars er erfitt að lesa hvítan texta ofan á myndinni þar sem partur af henni er hvítur).
- Efni skal vera miðjað með flexbox en fyrsta fyrirsögn skal dregin ofan (neikvætt margin) um fjögur bil.

Eftir haus á síðu birtist efni í tveim kortum (cards) með fyrirsagnirnar „Núverandi sýningar“ og „Skráðu hópinn þinn á sýningu“:

- Efni og mynd skal skipta í tvennt þar sem efnið tekur 7 af 12 dálkum af breiddinni og myndin 5 af 12.
  - Í minni skjástærðum skal efnið taka alla breidd og myndin birtast yfir efni.
- Efni:
  - „Kicker“ er fyrir ofan fyrirsögn og er í hástöfum í minna letri, `12px` en skilgreint í `rem`, ekki skal breyta HTML og setja stafi í hástafi heldur nota CSS
  - Fyrirsögn þar fyrir neðan
  - Efni þar fyrir neðan og tekur allt auka pláss sem í boði er.
  - Neðst vinstra megin skal vera tengill með útliti takka.
- Myndir:
  - Oddatölu kort skulu hafa myndir hægra megin við efni, jafntölu vinstra megin.
  - Myndir skulu hafa `5px` border radíus.
- Til að útfæra þessar breytingar þarf að breyta HTML uppsetningu.

### Um síða

- [Um síða í `1200px`](./fyrirmynd/um-1200x1000.png)
- [Um síða í `700px`](./fyrirmynd/um-700x900.png)
- [Um síða í `450px`](./fyrirmynd/um-450x700.png)

Eftir fyrirsagnir skal ekki vera bil. Milli svæða skal vera eitt bil.

### Sýningarsíða

- [Sýningarsíða í `1200px`](./fyrirmynd/syningar-1200x1000.png)
- [Sýningarsíða í `700px`](./fyrirmynd/syningar-700x900.png)
- [Sýningarsíða í `450px`](./fyrirmynd/syningar-450x700.png)

- Fyrirsagnir skulu vera fyrir ofan töflu.
- Milli tafla skal vera eitt bil.
- Fyrirsagnir á töflum skulu vera feitletraðar.
- Allt efni í töflu skal vera vinstrijafnað.
- Önnur hver röð í töflunni skal hafa bakgrunnslitinn `#ff9999`.
- Í minni skjástærðum skal taflan taka alla breidd og vera skrunanleg til hliðar.

### Skráningarsíða

- [Skráningarsíða síða í `1200px`](./fyrirmynd/skraning-1200x1000.png)
- [Skráningarsíða síða í `700px`](./fyrirmynd/skraning-700x900.png)
- [Skráningarsíða síða í `450px`](./fyrirmynd/skraning-450x700.png)

- Nýtt frá verkefni 3:
  - Setja upp svæði þannig að þau séu tvö í röð.
  - Milli svæða skal vera eitt bil á milli bæði lóðrétt og lárétt.
  - „Bóka“ svæði skal vera sér í línu
- Fyrirsagnir svæða skulu vera 24px, skilgreint í `rem`.
- Allir reitir skulu vera að hámarki `450px` breiðir.
- Allir form reitir skulu hafa hálft bil vinstra og hægra megin, hafa hvítan bakgrunn (`#ffffff`) og `1px` svartan (`#000000`) border.
- Þar sem tjékkbox eru notuð skulu þau vera á undan texta.
- Takki til að senda skal hafa bakgrunnslitinn `#ff9999`.
- Í minni skjástærðum skal allt efni taka alla breidd.

## Takmarkanir

Leyfilegt er að nota allt CSS.

## Netlify

Setja skal upp verkefni á Netlify með því að hlaða upp skrám með „manual deploy“ _eða_ tengja GitHub repo. Einnig er leyfilegt að nota aðra hýsingu en heyrið í kennara.

## Mat

- 20% – Snyrtilega uppsett og gilt CSS.
- 30% – Skalanleg lausn sett upp skv. forskrift.
- 30% – Grind sett upp skv. forskrift.
- 20% – „Dark mode“ útfært skv. forskrift.

## Sett fyrir

Verkefni sett fyrir í fyrirlestri mánudaginn 15. september 2025.

## Skil

Skila skal í Canvas, seinasta lagi fyrir lok dags fimmtudaginn 18. september 2025.

Skilaboð skulu innihalda bæði:

- zip skrá með öllum skrám og möppum í lausn á verkefni (eða hlekkur á GitHub).
- slóð á verkefni keyrandi á Netlify, sett sem athugasemd við skil á Canvas.

Athugið að það er **ekki nóg** að eingöngu setja athugasemd, skila þarf verkefni sérstaklega. Verkefnum sem ekki er skilað fá ekki einkunn.

## Aðstoð

Leyfilegt er að ræða, og vinna saman að verkefni en **skrifið ykkar eigin lausn**. Ef tvær eða fleiri lausnir eru mjög líkar þarf að færa rök fyrir því, annars munu allir hlutaðeigandi hugsanlega fá 0 fyrir verkefnið.

Ekki er heimilt að nota stór mállíkön til að vinna verkefni í námskeiðinu, [sjá nánar um notkun](https://github.com/vefforritun/vef1-2024/blob/main/mallikon.md).

## Verkefni og einkunn

Sett verða fyrir tíu minni verkefni þar sem átta bestu gilda 5% hvert, samtals 40% af lokaeinkunn.

Sett verða fyrir tvö hópverkefni þar sem hvort um sig gildir 10%, samtals 20% af lokaeinkunn.

> Útgáfa 0.2

## Útgáfusaga

| Útgáfa | Lýsing                                      |
| ------ | ------------------------------------------- |
| 0.1    | Fyrsta útgáfa verkefnisins                  |
| 0.2    | Bæta við html skrám, styles.css og grid.css |
