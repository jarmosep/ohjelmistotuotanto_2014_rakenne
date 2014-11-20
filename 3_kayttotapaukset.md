## Käyttötapaukset

### Loppukäyttäjät

Track-O-Polia on lisättyä todellisuutta hyödyntävä Wifi-pohjainen navigointisovellus, jonka avulla käyttäjät voivat mm. suunnistaa haluamiinsa luokkiin, etsiä tiettyä henkilökuntaan kuuluvaa henkilöä tai tarkistaa luokan saatavuuden. Jokaisella käyttäjällä on eri tavoitteet ja tarpeet, joten järjestelmän loppukäyttäjät määritelty seuraavasti:
- Opiskelijat
- Opettajat
- Muu koulun henkilökunta
- Vierailijat

Näiden käyttäjien lisäksi mobiilisovellusta käyttävät myös kehittäjät ja ylläpitäjät. Tästä syystä käyttötapaukset on jaoteltu kahteen osaan:
Käyttäjäpainoitteiset tapaukset. Yleisimmät tapaukset ovat:
- opastus haluttuun luokkaan älylaitteella (puhelin, tabletti)
- selvitys vapaiden luokkien lukumäärästä
- koulun henkilökunnan paikannus luokkakohtaisesti
- ohjelmistokohtaisen luokan / tietokoneen haku (esim. mistä löytyy 3DS Max, mistä Adobe InDesign?)

Kehittäjäpainoitteiset tapaukset. Tällaisia tapauksia ovat esimerkiksi:
- käyttäjien antamien palautteiden käsittely
- sovelluksen kehittäminen ja bugfixing
- järjestelmän ylläpito / käytön tuki

### Käyttötapauskaaviot

![Use case diagram example](http://users.metropolia.fi/~jarmosep/Kayttotapaukset1.png)
![Use case diagram example](http://users.metropolia.fi/~jarmosep/Kayttotapaukset2.png)


### Käyttötapausskenaariot

| Käyttötapaus                      	| Käyttäjä tarkastaa skannaamalla tietyn luokan tietokoneiden ohjelmistot                                                                                                                                                                                                                                                            	|
|-----------------------------------	|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| Alkutila                          	| 1. Käyttäjä on luokan ulkopuolella 2. Wifi-yhteys ja gyroskooppi ovat päällä 3. Puhelimen kamera toimii                                                                                                                                                                                                                            	|
| Tapahtumien normaali kulku        	| 1. Käyttäjä avaa,ohjelman älylaitteellaan 2. Käyttäjä valitsee,skannaustoiminnon 3. Käyttäjä suuntaa,älylaitteensa kameran haluamansa luokan oveen ja tunnukseen 4. Sovellus värjää,luokan oven vihreäksi – luokka on vapaa loppupäivän. 5. Lisätiedot luokasta avautuvat:,oppilaan hakema ohjelmisto löytyy luokan tietokoneilta. 	|
| Vikatilanteet                     	| 3a. Sovellus ei tunnista oven tunnusta (esim. tunnus on likaantunut) 3b. Käyttäjä on liian kaukana ovesta, tunnistusta ei voi tehdä 3c. Älylaite heiluu liikaa skannauksen yhteydessä, tunnistusta ei voi tehdä 3d. Ympäristössä on liian vähän valoa, tunnistusta ei voi tehdä                                                    	|
| Vaihtoehtoinen  tapahtumien kulku 	| 4a. Sovellus värjää luokan oven punaiseksi – luokka on varattulukujärjestyksen mukaan /  toisen henkilön toimesta                                                                                                                                                                                                                  	|
| Lopputila                         	|                                                                                                                                                                                                                                                                                                                                    	|


