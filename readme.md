# Verkefni 2

Setja skal upp fjórar síður, aðgengilegar af internetinu:

1. Forsíða með tenglum á aðrar síður, titill: `Velkomin á veðurstöðina!`
2. Síða með skráningarformi, titill: `Skráðu þig í veðurstöðina`
3. Síða með töflu yfir veðurgögn: `Veðurgögn`
4. Síða með texta um veður: `Fróðleikur um veður`

Allar síður fyrir utan forsíðu skulu vera innan `pages/` möppu, sjá gefið efni.

## Forsíða

Inniheldur titil, valmynd og ekkert meira (nema þið viljið skrifa eitthvað um veðrið.)

## Valmynd

Allar síður skulu innihalda valmynd sem vísar á allar aðrar síður. Fyrir þá síðu sem er opin skal feitletra og fjarlægja tengil á hana. Athugið að allar síður fyrir utan forsíðu verða að vera undir `pages/` möppu.

Fyrir neðan efni á öðrum síðum en forsíðu er lárétt lína notuð til að aðskilja á milli efnis og valmyndar.

## Síða með skráningarformi

Form tekur við upplýsingum fyrir skráningu notanda í veðurklúbbinn og skal vera sett upp með aðgengi í huga.

Eftirfarandi skal biðja um í formi, hópað saman með `<fieldset>` og með viðeigandi `legend`:

* Veðuráhugi
  - Staðsetning, val úr lista þar sem listi eru póstnúmer á Íslandi, sýna skal bæði póstnúmer og stað, sjá `postnumer.txt`
  - Netfangi til að senda veðurupplýsingar á, textareitur sem krafist og innihald ætti að líta út eins og netfang
* Greiðsluupplýsingar
  - Kortategund, _radio_ val um `Visa`, `MasterCard`, `AMEX`
  - Kortanúmer, textareitur sem er krafist
  - Gildistími
    + Val úr mánuðum
    + Val úr árum, frá og með 2020 til og með 2030
  - `checkbox` val sem er sjálgefið valið með textanum „Senda kvittun.“
  - Athugasemd, textareitur sem bíður upp á fleiri en eina línu af texta
* Takki til að hreinsa form/byrja upp á nýtt sem á stendur „Byrja upp á nýtt“
* Takki til að senda form sem á stendur „Senda“

Þegar ýtt er á takka gerist ekki neitt, þ.e.a.s. engin kóði keyrir og gögn eru ekki send neitt.

Síðan skal hafa fyrirsögnina `Form`.

## Síða með töflu yfir veðurgögn

Birta skal töflu með fyrirsögn `Meðalhiti í Reykjavík frá 1949` þar sem gögn eru í `medalhiti.txt`. Birta skal gögn úr dálkum `t` sem geymir meðalhita, `tx` sem geymir meðalhámarskshita og `txx` sem geymir hæsta hiti sem mældist í mánuðinum/á árinu.

[Gögnin eru sótt frá Veðurstofu Íslands](https://www.vedur.is/vedur/vedurfar/medaltalstoflur/).

## Síða með texta um veður

Varpa skal texta í `vedur.md` yfir í HTML með því að [þýða viðeigandi Markdown skipanir](https://daringfireball.net/projects/markdown/syntax) yfir í HTML.

Fyrir neðan texta skal vera lína (`<hr>`) og eftirfarandi texti:

> Texti og myndir fengnar frá Veðurstofu Íslands.

og skal textinn tengja í `https://www.vedur.is/vedur/frodleikur/greinar/nr/2532`.

Vísað er í myndir undir img/. Laga þarf slóð á mynd á HTML skrá, ekki skal færa img/ möppu. Titill myndar í Markdown skjali skal birta fyrir neðan mynd, [sjá hvernig birting er á upprunalegu grein](https://www.vedur.is/vedur/frodleikur/greinar/nr/2532) (ekki þarf að láta mynd birtast til hliðar).

## Almennt

* Ekki er krafa um að stýra útliti neitt með CSS
* Allar síður skulu hafa fyrisögn og „beint í efni“ hlekk á eftir fyrirsögn, en á undan valmynd.
* Síður skulu nota `utf-8` stafasett.
* Hafa snyrtilega uppsettan kóða þar sem inndráttur er samræmdur.
* Nýta merkingarfræðilega viðeigandi element.
* Vera villulaus ef hún er prófuð með [HTML validator](https://validator.w3.org/).
* Vera án aðgengisvillna ef hún er prófuð með [aXe](https://www.deque.com/axe/), setjið upp viðbót í vafra.

## Heimasvæði

Setja skal síður upp á heimasvæði RHÍ, (http://rhi.hi.is/node/155) undir möppu `.public_html/vefforritun/verkefni1` svo verkefnið verði aðgengilegt á `https://notendur.hi.is/<notendanafn>/vefforritun/verkefni2` þar sem `<notendnafn>` er notendanafnið þitt (t.d. `osk`).

## Mat

* 20% – Snyrtilega uppsettur kóði með merkingarfræðilegum elementum fyrir hverja síðu
* 20% – Síður án villna frá HTML validator og WAVE validator
* 20% – Form uppsett eftir forskrift
* 20% – Tafla uppsett eftir forskrift
* 20% – Forsíða og textasíða uppsett eftir forskrift

## Sett fyrir

Verkefni sett fyrir í fyrirlestri mánudaginn 31. ágúst 2020.

## Skil

Skila skal í Canvas í seinasta lagi fyrir lok dags föstudaginn 11. september 2020.

Skilaboð skulu innihalda slóð á verkefni ásamt zip skjali með lausn.

## Einkunn

Sett verða fyrir tíu minni verkefni þar sem átta bestu gilda 5% hvert, samtals 40% af lokaeinkunn.

Sett verða fyrir tvö hópverkefni þar sem hvort um sig gildir 10%, samtals 20% af lokaeinkunn.

> Útgáfa 0.1

### Útgáfusaga

| Útgáfa | Lýsing                              |
|--------|-------------------------------------|
| 0.1    | Fyrsta útgáfa                       |
| 0.2    | Uppfæra skiladag, bæta við skjáskotum                       |