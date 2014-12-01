## Vaatimukset 


### Funktionaaliset vaatimukset
  
| Toiminto | Kuvaus |
|----------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ohjelman käynnistys | Ohjelma käynnistetään älylaitteelta Track-O-Polian kuvaketta painamalla. |
| Tietojen haku palvelimelta | Sovelluksen tulee hakea Metropolian palvemelta lukujärjestyksen tiedot ja aikataulut |
| Toiminnon valinta | Käyttäjän on voitava valita pääikkunasta eri toimintoja. Painiketta painamalla pitää tapahtua sitä kuvaava toiminto: Etsi luokka -> luokan etsintä näkymä avautuu |
| Luokan oven skannaus | Sovelluksen pitää aktivoida kamera ja siirtyä QR-tunnuksia tunnistavaan skannaustoimintoon. |
| Tietojen hakeminen | Sovelluksella pitää pystyä hakemaan luokkia ja opettajia nimen tai tunnuksen perusteella |
| Paikkatietojen tallennus | Sovelluksella pitää pystyä tallentaa kosketuksesta haluttu sijainti/opettaja tietokantaan. |
| Aloita navigointi | Sovelluksen pitää aktivoida kamera ja käynnistää navigointi |
| Päämäärään saapuminen | Sovelluksen pitää ilmoittaa päämäärään saapumisesta |
| Asetusten muutaminen | Sovelluksen tulee muistaa käyttäjän valitsemat asetukset |


### Ei-funktionaaliset vaatimukset

| Toiminto          | Kuvaus                                                                                                                                                                  | Toteutus                                                                                                                                                                                                                                                              |
|-------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Helppokäyttöisyys | - sovelluksen käyttöliittymän tulee olla helppokäyttöinen <br> - käyttöliittymän tulee olla nopeasti opittava                                                           | - perinteiset älylaitteen "gesturet" <br> - selkeät painikkeet ja värikontrastit <br>  - selkeät siirtymät eri näkymien välillä <br> - universaalit graafiset elementit <br> - riittävästi tilaa graafisten elementtien välissä <br> - itsekuvaavat toimintojen nimet |
| Suorituskyky      | - sovelluksen toimintojen ja tietokannan tulee latautua nopeasti <br> - vasteaika on oltava lyhyt, varsinkin navigointinäkymässä <br> - energiatehokkuus: akun kesto    | - mahdollisimman paljon laskentaa totetutetaan palvelimella <br> - kevyt, tehokas ja virheetön koodi <br> - tiedostojen koot pidettävä mahdollisimman alhaisina <br>                                                                                                  |
| Skaalautuvuus     | - sovelluksen tulee näyttää kaikilla laitteilla samalta <br> - sovelluksella voi olla monta yhtäaikaista käyttäjää                                                      | - käyttöliittymästä tehdään näytön resoluution mukaan skaalautuva <br> - järjestelmäarkkitehtuurin komponentit pystyvät käsittelemään useita yhtäaikaisia palvelupyyntöjä vasteajasta tinkimättä                                                                      |
| Siirrettävyys     | - sovelluksen tulee toimia samalla tavalla kaikilla älylaitteilla, Androidilla ja iOS:lla <br> - sovellus voidaan siirtää uuteen arkkitehtuuriin siedettävällä hinnalla | - arkkitehtuurista tehdään yksinkertainen ja sovellettava <br> - lähdekoodista tehdään Swift:lle ja Javalle helposti muokattava <br> - määritellään mahdolliset uudet alustat ja versiot (esim. Windows Phone) ja kustannusarviot                                     |
| Ylläpidettävyys   | - sovelluksen ylläpidettävyyden tulee olla helppoa ja johdonmukaista                                                                                                    | - koodia tulee kommentoida ja sisennyksiä tulee käyttää <br> - yleiset koodin nimeämiskäytännöt <br> - sovellus lähettää virheilmoitukset automaattisesti ylläpidolle                                                                                                 |


  * Esim käytettävyyteen, tietoturvaan, tehokkuuteen, skaalautuvuuteen, hintaan ja prosessimalliin liittyvät vaatimukset
* **Muista esittää vaatimukset jäljitettävässä muodossa, yksiselitteisesti**
* Keskeinen tapa (erityisesti ei-funktionaalisiin vaatimuksiin) yksiselitteisille kuvauksille on vaatimusten **mitattavuus** (software metrics)
