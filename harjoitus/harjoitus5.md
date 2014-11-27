## Harjoitus 5: Käyttöliittymän suunnittelu

#### 1. Selitä seuraavat käsitteet:

  1. Näkymä (view)
    - määrittää käyttöliittymän ulkoasun ja tietojen näytön esityksen käyttöliittymässä.
  2. Wireframe
    - havainnollistava ja suuntaa antava luonnos käyttöliittymän tulevasta graafisesta näkymästä. Kuvataan toimintalogiikka.
  3. Mockup
    - voidaan tehdä yksityiskohtainen näkymä (wireframea hyödyntäen) lopullisesta käyttöliittymästä, mutta sillä ei ole toiminnallisuutta
  4. Prototyyppi
    - toimiva, aikainen julkaisu sovelluksesta. Kehysmalli.

#### 2. Käyttöliittymän näkymät (User interface, views), oma projektiaihe. Voi tehdä pienryhmissä. 

1. Miten käyttötapaukset ja käyttöliittymät voisi yhdistää toisiinsa vaatimusmäärittelydokumentaatiossa? Perustele
vastauksesi.
    - tapahtumien kulussa voidaan selostaa mitä sovelluksen käyttöliittymässä näkyy kussakin tilanteessa.
2. Listaa järjestelmän käyttöliittymän olennaisimmat näkymät
    - päävalikko, skannausnäkymä, luokan/opettajan hakunäkymä , navigointinäkymä
3. Kuvaile näkymät *sanallisesti*: mitä näkymällä tehdään ja mitä siinä näkyy. Pyri määrittelemään tässä näkymät
*toiminnallisesta näkökulmasta*, älä niinkään ajattele miltä ne näyttävät
    - päävalikosta päästään käsiksi sovelluksen kaikkiin toimintoihin. Päävalikosta päästään toimintoihin "Etsi luokka", "Etsi opettaja", "skannaa luokka", asetukset, suosikit, info.
    - skannausnäkymä: näytölle avautuu puhelimen kameran kuva. Näkymässä skannataan luokan tietoja ovessa olevan tunnuksen perusteella, saadaan selville esim. mitä ohjelmistoja luokassa on. Luokan ovi värjäytyy vihreäksi, mikäli se on vapaa. Punaiseksi, jos varattu. 
    - Luokan hakunäkymä: Hakukenttä, mihin syötetään luokan numero tai sanallinen tunnus (esim. Dolphin). Toisessa hakukentässä luokkia voi etsiä aineen perusteella, jolloin vaihtoehdot tulevat esiin numeerisessa järjestyksessä. Tämän jälkeen avautuu varmistusvalikko, missä kysytään aloitetaanko navigointi ja lisätäänkö suosikkeihin. 
    - Opettajan hakunäkymä: Hakukenttä, mihin syötetään opettajan nimi. Toisessa hakukentässä opettajaa voi hakea aineen perusteella. Tämän jälkeen avautuu kolmas hakukenttä, mihin syötetään oman ryhmän tunnus. Tällöin saadaan esille kaikki tietyn koulutusohjelman aineen opettajat. Tämän jälkeen avautuu varmistusvalikko, missä kysytään aloitetaanko navigointi ja lisätäänkö suosikkeihin. 
4. Määritä näkymien väliset siirtymät korkealla tasolla, mistä näkymästä pääsee minnekin? Millä tavoin visualisoisit tilasiirtymät?
    - päävalikosta siirrytään etsintänäkymään, josta edelleen navigointinäkymään.
    - päävalikosta voidaan siirtyä skannausnäkymään
    - navigointinäkymän tai skannausnäkymän varmistusvalikosta voidaan siirtyä suosikkilistoihin, sen jälkeen kun opettaja/luokka on lisätty suosikkeihin.
    - päävalikosta pääsee käsiksi suosikkilistoihin, infoon ja asetuksiin
    - info-valikosta käyttäjä pääsee lähettämään palautetta kehittäjille
5. Listaa jokaista näkymää kohti tieto siitä, millaista tietosisältöä tai data käyttöliittymässä näytetään.
    - päävalikko on staattinen ja näyttää kaikki ohjelmiston haarat
    - etsi luokka/opettaja-näkymässä haetaan tietokannasta tietoa. Ohjelma toimii synkronisesti ja tarjoaa eri hakuvaihtoehtoja käyttäjälle tämän kirjoittaessa esim. aineen nimeä, eli se etenee ns. "tahdistuksen mukaisesti".
    - navigointinäkymä hakee puhelimen kameran syötteen ja näyttää sen näytöllä. Puhelin katsoo paikkatietojen perusteella sijainnin ja piirtää kampuksen 3D-malliin pohjautuen opastusnuolia lattiaan.
    - skannausnäkymä hakee puhelimen kameran syötteen ja näyttää sen näytöllä. Kameran reagoidessa luokan oven RFID-tunnukseen, sovellus hakee Metropolian palvelimelta tiedon onko luokka vapaa tai varattu.

#### 3. Visualisoi listaamasi näkymät ja niihin liittyvät siirtymät

#### Päävalikko
  ![Paavalikko](http://users.metropolia.fi/~jarmosep/ohjelmistotuotanto/3.jpg)
  
#### Suosikit
  ![Suosikit](http://users.metropolia.fi/~jarmosep/ohjelmistotuotanto/2.jpg)

#### Navigointi
  ![navigointi luokkaan](http://users.metropolia.fi/~teemusuv/eteneminen.png)

#### Luokan skannaus
  ![luokan skannaus](http://users.metropolia.fi/~teemusuv/scan.png)
  ![luokan skannaus](http://users.metropolia.fi/~teemusuv/scanInfo.png)
  
**Palauta linkki projektinne tiedostoon (Github), mistä löytyvät vastaukset tehtäviin. Vaikka teitte työn ryhmätyönä, jokainen palauttaa linkin Tuubiin henkilökohtaisesti.**
