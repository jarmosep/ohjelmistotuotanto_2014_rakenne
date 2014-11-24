## Harjoitus 4 

### Johdanto
- Sähköisen lääkemääräyksen vaatimusmäärittely. Tämä dokumentti kuvaa sähköisen lääkemääräyksen 
toteuttamiseksi tarvittavan toiminnallisuuden siihen liittyvien tietojärjestelmien ja niiden käyttäjien 
osalta.
- Dokumentti on tarkoitettu ihmisille, ketkä haluavat tutustua sähköisen lääkemääräyksen vaatimusmäärittellyyn:
Alan ammattilaiset: Lääkärit, hoitajat.
- Projekti on valmis. eResepti-palvelu on otettu käyttöön 1.9.2014
- Dokumentti on luotu siksi, koska projekti on vaatinut yksityiskohtaisia vaatimusmäärittelyjä.
- Dokumentissa kuvataan potilastietojärjestelmän käyttötapauksia. Kukin käyttötapaus kuvaa, mitä käyttäjä ja 
potilastietojärjestelmä tekevät, jotta käyttäjä saa suoritettua jonkinitsenäisen, lyhyen ja 
kerralla suoritettavan toimenpiteen, joka tukee hänen muuta toimintaansa. Kuvaukset eivät 
määrittele tarkkoja teknisiä yksityiskohtia vaan toiminnallisentavoitteen, joka tulee saavuttaa. 
Käyttötapausten kuvaaman toiminnallisuuden voi toteuttaateknisesti monin eri tavoin. 

### Käyttötapaukset
- Käyttäjäryhmällä on oikeudet mm. kirjoittaa, korjata ja mitätöidä lääkemääräyksiä, mikäli he toimivat 
potilaan hoitavana lääkärinä. Määräykset voivat olla tarkoitettuja potilaalle tai lääkärille itselleen.
- Käyttötapauskaaviot esimerkkejä:
  * Ylläpitäjä: Muuta käyttäjän oikeuksia
  * Kaikki käyttäjät: Tunnista käyttäjä ja tarkasta valtuutus, kirjaudu ulos
  * Muu henkilökunta: Tee uusimispyyntö, hylkää tai palauta uusimispyyntö
  * Sairaanhoitaja: Hylkää tai palauta uusimispyyntö, tulosta potilasohje, tarkastele lääkemääräyksiä
  * Lääketietokanta: Korjaa lääkemääräyksiä
  * Reseptikeskus: Hae tietoja reseptikeskuksesta
- Käyttötapauksia on lukuisia, joista kaikkia ei tähän harjoitukseen kannata listata.
Lista on erittäin yksityiskohtainen.
- Varsinaisia käyttötapausskenaarioita tai tarinoita ei ole listattu

### Järjestelmän yleisrakenne

- Järjestelmän kuvaukseen on käytetty erilaisia kaaviotekniikoita:
	* käyttötapauskaavioita, jotka havainnollistavat mitä sovelluksella voi tehdä ja mikä toiminnallisuus
	on käytettävissä milläkin käyttäjäryhmällä
	* uml-luokkakaavioita, joilla havainnollistetaan eReseptin rakennetta
	* työnkulkukaavio, jolla näytetään projektin etenemistä
	
### Funktionaaliset ja ei-funktionaaliset vaatimukset

- Järjestelmän vaatimukset on esitetty taulukoina:
	* kaikki vaatimukset on kategorioitu, numeroitu ja niiden tärkeys on merkitty kirjainsymbolein
	* vaatimukset on kuvattu erittäin yksityiskohtaisesti ja yksiselitteisesti
	* vaatimuksissa on myös määritelty kohdistuuko se käyttäjään vai ohjelmistoon

### Miltä näyttää
- Käyttöliittymästä ei ole kuvia

### Prosessimalli
- EReseptin käyttöönotto toteutetaan vesiputousmallilla. Arvioitu kesto on n. 7kk.
- Kyseessä on vain pohja suunnitelmalle, joten mitään määriteltyä budjettia tai resursseja ei ole. EReseptin käyttöönotto suoritetaan paikallisella tasolla eikä kattavaa maanlaajuista suunnitelmaa ole saatavilla.'

- Riskianalyysissä on 8 kohtaa
- Projektinhallinta
	* Aikataulu (viivästykset)
	* Kustannukset (budjetti ylittyy)
	* Resurssit (osaamisen kohdistaminen väärin)
- Potilastietojärjestelmät
	* Bugit
- Tietoliikenne ja yhteiset palvelut, laitteet
	* Laitteet ja tietoliikenneyhteydet hankittava riittävän ajoissa (toimitusaika)
- Varmennepalvelut
- Toimintamallit ja prosessit
- Käyttöönotto ja tuotannonaikainen tuki
- Koulutus
- Viestintä	


### Johtopäätökset

- Mikä tekee hyvän dokumentin?
 * selkeä yleisilme / rakenne
 * johdonmukaisuus
 
 - Onko tämä sellainen? Miksi?
 * Dokumentti on tekstisisällöltään hyvä, mutta kaaviot ovat epäselviä
 * Kaikki kohdat on perusteellisesti selitetty
 * Yhtenäinen ulkoasu
 
 - Kaavioiden käyttö: laatu? määrä? hyöty? 
 * kaavioita on suhteellisen paljon
 * kaavioiden laatu melko huono, epäselviä ja monimutkaisia
 * kaaviot ovat hyödyllisiä, jos asiasta on valmiiksi jotain tietoa