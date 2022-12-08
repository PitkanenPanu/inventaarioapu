# Inventaarioapu-2022, Vaatimusmäärittely

* Dokumentin versionumero 1.0

## Johdanto


Projektin tavoitteena on muokata ja tuottaa AppGyver sovellus, joka toimii inventaariotyökaluna toimeksiantajalle helpottamaan tapahtumiin tulevien bändien tuotteiden laskemisessa.

## Tavoitteet 

Projektin tavoitteena on kehittää helppokäyttöinen ja selkeä sovellus, joka tallentaa annettuja tietoja.

## Palveluun liittyvät haasteet

Haasteena on saada sovelluksesta mahdollisimman yksinkertainen, mutta kuitenkin toimeksiantajan toivomia toimintoja sisältävä. Olemme muutamaan kertaan arvioineet uudelleen kunkin toiminnallisuuden tarpeellisuutta ja mahdollista karsimista. 

## Kohderyhmä

Tapahtuma-alan työntekijät

## Sidosryhmät

opiskelijat -- Jamk
ohjaajat -- Jamk
toimeksiantaja -- Ext Ventures Oy
ulkopuoliset käyttäjät -- John Smith Rock Festivaalin merge vastaavat


## Palveluun liittyviä asiakaspolkuja

**asiakaspolku PlantUML-esimerkki tilakoneena**

*käyttäjän asiakaspolku Inventaarioapu-2022- sovelluksessa*

```plantuml
[*] --> Step1

Step1 : Käyttäjä avaa sovelluksen. 
Step2 : Käyttäjä kirjautuu sisään.
Step3 : Käyttäjä voi lisätä uusia bändejä tapahtumaan.
Step4 : Käyttäjä voi lisätä kullekin luomalleen bändille tuotteita. Joko koollisia tai yksittäiskappaleita.
Step5 : Käyttäjä voi lisätä tuotteelle hinnan.
Step6 : Käyttäjä voi myynnin jälkeen lisätä jäljelle jäävien tuotteiden määrän.
Step7 : Käyttäjä voi nähdä suoraan sovelluksesta täsmääkö myynnit ja kassa sovelluksen tietojen kanssa.
Step8 : Käyttäjä voi saada sovelluksesta raportin, joka sisältää: tuote, koko, tulleet, jäljellä, hinta, myytyjä, yhteissumma.

Step1 --> Step2
Step2 --> Step3
Step2 --> Step4
Step4 --> Step5
Step5 --> Step6
Step5 --> Step7
Step5 --> Step8
```


## Tärkeimmät toiminnallisuudet/ominaisuudet

Sovelluksen oleellisia toimintoja:

* Käyttäjä käyttää valmiiksi luotuja tunnuksia 
* Käyttäjä voi Lisätä inventaario tietoja sovellukseen
* Käyttäjä voi muokata inventaario tietoja
* Käyttäjä voi Lisätä muistiinpanoja/kommentteja inventaario tietoihin
* Käyttäjän lisäämät tiedot tallentuvat firebaseen



## Asiakkaan toivomat ominaisuudet

**Yleiset:**

- Todella selkeä käyttöjärjestelmä
- visuaalisesti käyttöjärjestelmä yksinkertainen ja helppo käyttää kiireisissä tilanteissa
- Tallentaa inventaario tietoja
- Sovellus on myös suunniteltu toimimaan Tabletin kanssa
- Bändi kohtaiset raportit katseltavissa myös tietokoneelta

**Toiminnot:**

- Lisää bändin tuomien tuotteiden lukumäärä ennen ja jälkeen
- Tallenta tiedot tietokantaan
- csv tiedostot

**Tietoturva:**

- tietoturvaan toivottua että data pysyisi Suomessa Yrityksen sisällä
- hyödynnettävien sovellusten keräämä datan tiedote
- selvitä palautejärjestelmän tietosuojaehdot


## Alustavat käyttäjätarinat

[Käyttäjätarinat](vaatimukset/käyttäjätarinat.md)

## Yleiset tekniset vaatimukset

[Tekniset vaatimukset](vaatimukset/tekniset_vaatimukset.md)

## Toiminnalliset vaatimukset (Functional Requirements)

[Toiminnalliset vaatimukset](vaatimukset/toiminnalliset_vaatimukset.md)

## Suorituskykyyn liittyvät vaatimukset

[Suorituskyvyn vaatimukset](vaatimukset/suorituskyvyn_vaatimukset.md)

## Tietoturvan vaatimukset

[Tietoturvan vaatimukset](vaatimukset/tietoturvan_vaatimukset.md)

## Saavutettavuuden vaatimukset

[Saavutettavuuden vaatimukset](vaatimukset/saavutettavuuden_vaatimukset.md)

## Toimeksiannon kannalta kesävänkehityksen vaatimukset

[Kestävänkehityksen vaatimukset](vaatimukset/kestavakehitys_vaatimukset.md)

## Palvelun tuotantoympäristö

Tuotanto tapahtuu AppGyver- palvelun tarjoamassa kehitysympäristössä. Tietokantana käytössä on Firebase.

## Standardit ja lähteet

| ID | Nimi | Linkki | Kuvaus |  
|:-:|:-:|:-:|:-:|
| REF1 | JHS 165 ICT | [JHS Suositukset - vaatimusmäärittelylle](http://www.jhs-suositukset.fi/c/document_library/get_file?uuid=b8118ad7-8ee4-459a-a12b-f56655e4ab9d&groupId=14) | Vaatimusmäärittelyn suositus |
| REF2 | ISO 9241-11  | [Käytettävyys](https://fi.wikipedia.org/wiki/K%C3%A4ytett%C3%A4vyys)  | Usability | 
| REF3 |  EN 301 549 | [Saavutettavuus](https://fi.wikipedia.org/wiki/Saavutettavuus) | Availability |
| REF4 |  GDPR | [GDPR Asetus](https://europa.eu/youreurope/business/dealing-with-customers/data-protection/data-protection-gdpr/index_fi.htm) | General_Data_Protection_Regulation |
