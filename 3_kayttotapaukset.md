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

Näissä kaavioissa käyttäjiin on vedetty yhteen opiskelijat, opettajat ja vierailijat. Toinen kaavio kuvaa kehittäjien yleisimpiä käyttötapauksia.

![Use case diagram example1](http://users.metropolia.fi/~jarmosep/kaytto1.png)
![Use case diagram example2](http://users.metropolia.fi/~jarmosep/kaytto2.png)


### Käyttötapausskenaariot

Näihin käyttötapausskenaarioihin on koottu taulukoittain kaikista yleisimmät tapaukset, joita käyttäjät tekevät.

| Käyttötapaus                      | Käyttäjä tarkastaa skannaamalla tietyn luokan tietokoneiden ohjelmistot                                                                                                                                                                                                                                                                                |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Alkutila                          | 1. Käyttäjä on luokan ulkopuolella <br> 2. Wifi-yhteys ja gyroskooppi ovat päällä <br>  3. Puhelimen kamera toimii                                                                                                                                                                                                                                     |
| Tapahtumien normaali kulku        | 1. Käyttäjä avaa ohjelman älylaitteellaan <br> 2. Käyttäjä valitsee skannaustoiminnon <br> 3. Käyttäjä suuntaa älylaitteensa kameran haluamansa luokan oveen ja tunnukseen <br> 4. Sovellus värjää luokan oven vihreäksi – luokka on vapaa loppupäivän. <br> 5. Lisätiedot luokasta avautuvat: oppilaan hakema ohjelmisto löytyy luokan tietokoneilta. |
| Vikatilanteet                     | 3a. Sovellus ei tunnista oven tunnusta (esim. tunnus on likaantunut) <br> 3b. Käyttäjä on liian kaukana ovesta, tunnistusta ei voi tehdä <br> 3c. Älylaite heiluu liikaa skannauksen yhteydessä, tunnistusta ei voi tehdä <br> 3d. Ympäristössä on liian vähän valoa, tunnistusta ei voi tehdä                                                         |
| Vaihtoehtoinen  tapahtumien kulku | 4a. Sovellus värjää luokan oven punaiseksi – luokka on varattu lukujärjestyksen mukaan /  toisen henkilön toimesta                                                                                                                                                                                                                                      |
| Lopputila                         | 1. Käyttäjä sulkee sovelluksen, menee luokkaan ja käyttää tietokonetta                                                                                                                                                                                                                                                                                 |


| Käyttötapaus                      | Käyttäjä navigoi luokkaan joka on vapaa                                                                                                                                                                                                                           |
|-----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Alkutila                          | 1. Wifi-yhteys ja gyroskooppi ovat päällä <br> 2. Puhelimen kamera toimii                                                                                                                                                                                         |
| Tapahtumien normaali kulku        | 1. Käyttäjä avaa ohjelman älylaitteellaan <br> 2. Käyttäjä valitsee ”etsi luokka”-toiminnon <br> 3. Käyttäjä syöttää luokan tunnuksen kenttään <br> 4. Käyttäjä aloittaa kameranavigoinnin <br> 5. Käyttäjä noudattaa suuntaohjeita <br> 6. Päämäärään saapuminen |
| Vikatilanteet                     | 4a. Rakennuksen mahdolliset aluekohtaiset kalibrointiongelmat – vääränlainen  navigointinäkymä <br> 6a. Luokka on varattu, tieto ei ole päivittynyt sovellukseen                                                                                                  |
| Vaihtoehtoinen  tapahtumien kulku | 4. Käyttäjä pysähtyy kesken navigoinnin tarkastamaan muita matkan varrella olevia  luokkia skannaustoiminnolla <br> 5. Vapaa luokka löytyy <br> 6. Päämäärään saapuminen                                                                                          |
| Lopputila                         | 1. Käyttäjä sulkee sovelluksen ja menee luokkaan                                                                                                                                                                                                                  |

| Käyttötapaus                      | Käyttäjä etsii tietyn aineen opettajaa, mutta ei muista nimeä                                                                                                                                                                                                                                                                                                                                                                                                 |
|-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Alkutila                          | 1. Opettaja on koulussa <br> 2. Wifi-yhteys ja gyroskooppi ovat päällä <br> 3. Puhelimen kamera toimii                                                                                                                                                                                                                                                                                                                                                        |
| Tapahtumien normaali kulku        | 1. Käyttäjä avaa ohjelman älylaitteellaan <br> 2. Käyttäjä valitsee ”etsi opettaja”-toiminnon <br> 3. Käyttäjä syöttää ”etsi aineen perusteella” kenttään haluamansa aineen <br> 4. Käyttäjä syöttää seuraavaan kenttään ryhmätunnuksensa <br> 5. Käyttäjä valitsee avautuvasta listasta ryhmäkohtaisten opettajansa <br> 6. Käyttäjä näkee, että opettaja on laboratoriotiloissa <br> 7. Käyttäjä aloittaa kameranavigoinnin laboratoriotiloihin <br> 8. Käyttäjä noudattaa suuntaohjeita <br> 9. Kohdehenkilön löytyminen |
| Vikatilanteet                     | 6a. Rakennuksen mahdolliset aluekohtaiset kalibrointiongelmat – vääränlainen navigointinäkymä                                                                                                                                                                                                                                                                                                                                                                 |
| Vaihtoehtoinen  tapahtumien kulku | 5. Opettaja on toimistossaan <br> 6. Käyttäjä aloittaa kameranavigoinnin toimistoon <br> 7. Käyttäjä noudattaa suuntaohjeita <br> 8. Kohdehenkilön löytyminen                                                                                                                                                                                                                                                                                                 |
| Lopputila                         | 1. Käyttäjä sulkee sovelluksen                                                                                                                                                                                                                                                                                                                                                                                                                                |


| Käyttötapaus                      | Käyttäjä lisää tietoja suosikkeihin                                                                                                                                                                                                                                                                                           |
|-----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Alkutila                          | 1. Wifi-yhteys on päällä                                                                                                                                                                                                                                                                                                      |
| Tapahtumien normaali kulku        | 1. Käyttäjä avaa ohjelman älylaitteellaan <br> 2. Käyttäjä valitsee ”suosikit”-toiminnon <br> 3. Käyttäjä valitsee avautuvasta ikkunasta plus-ikonin <br> 4. Käyttäjä syöttää opettajan nimen / luokan nimen kenttään <br> 5. Käyttäjä valitsee ”OK”                                                                          |
| Vikatilanteet                     | Ei ohjelmistokohtaisia vikatilanteita, mikäli alkutilanne ei järky                                                                                                                                                                                                                                                            |
| Vaihtoehtoinen  tapahtumien kulku | 2. Käyttäjä valitsee ”etsi opettaja” tai ”etsi luokka” toiminnon <br> 3. Käyttäjä syöttää haluamansa tunnuksen kenttään <br> 4. Käyttäjä ei aloita navigointia, painaa ”Lisää suosikkeihin”-ikonia <br> 5. Käyttäjä painaa ”OK” -varmistusnappia <br> 6. Käyttäjä palaa takaisin ohjelman pääikkunaan nuoli-ikonia painamalla |
| Lopputila                         | 1. Tietokantaa on muunneltu <br> 2. Käyttäjä sulkee sovelluksen                                                                                                                                                                                                                                                                   |
