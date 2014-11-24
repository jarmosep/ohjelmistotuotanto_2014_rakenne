## Harjoitus 5: K�ytt�liittym�n suunnittelu

#### 1. Selit� seuraavat k�sitteet:

  1. N�kym� (view)
    - m��ritt�� k�ytt�liittym�n ulkoasun ja tietojen n�yt�n esityksen k�ytt�liittym�ss�.
  2. Wireframe
    - havainnollistava ja suuntaa antava luonnos k�ytt�liittym�n tulevasta graafisesta n�kym�st�. Kuvataan toimintalogiikka.
  3. Mockup
    - voidaan tehd� yksityiskohtainen n�kym� (wireframea hy�dynt�en) lopullisesta k�ytt�liittym�st�, mutta sill� ei ole toiminnallisuutta
  4. Prototyyppi
    - toimiva, aikainen julkaisu sovelluksesta. Kehysmalli.

#### 2. K�ytt�liittym�n n�kym�t (User interface, views), oma projektiaihe. Voi tehd� pienryhmiss�. 

1. Miten k�ytt�tapaukset ja k�ytt�liittym�t voisi yhdist�� toisiinsa vaatimusm��rittelydokumentaatiossa? Perustele
vastauksesi.
    - tapahtumien kulussa voidaan selostaa mit� sovelluksen k�ytt�liittym�ss� n�kyy kussakin tilanteessa.
2. Listaa j�rjestelm�n k�ytt�liittym�n olennaisimmat n�kym�t
    - p��valikko, skannausn�kym�, luokan/opettajan hakun�kym� , navigointin�kym�
3. Kuvaile n�kym�t *sanallisesti*: mit� n�kym�ll� tehd��n ja mit� siin� n�kyy. Pyri m��rittelem��n t�ss� n�kym�t
*toiminnallisesta n�k�kulmasta*, �l� niink��n ajattele milt� ne n�ytt�v�t
    - p��valikosta p��st��n k�siksi sovelluksen kaikkiin toimintoihin. P��valikosta p��st��n toimintoihin "Etsi luokka", "Etsi opettaja", "skannaa luokka", asetukset, suosikit, info.
    - skannausn�kym�: n�yt�lle avautuu puhelimen kameran kuva. N�kym�ss� skannataan luokan tietoja ovessa olevan tunnuksen perusteella, saadaan selville esim. mit� ohjelmistoja luokassa on. Luokan ovi v�rj�ytyy vihre�ksi, mik�li se on vapaa. Punaiseksi, jos varattu. 
    - Luokan hakun�kym�: Hakukentt�, mihin sy�tet��n luokan numero tai sanallinen tunnus (esim. Dolphin). Toisessa hakukent�ss� luokkia voi etsi� aineen perusteella, jolloin vaihtoehdot tulevat esiin numeerisessa j�rjestyksess�. T�m�n j�lkeen avautuu varmistusvalikko, miss� kysyt��n aloitetaanko navigointi ja lis�t��nk� suosikkeihin. 
    - Opettajan hakun�kym�: Hakukentt�, mihin sy�tet��n opettajan nimi. Toisessa hakukent�ss� opettajaa voi hakea aineen perusteella. T�m�n j�lkeen avautuu kolmas hakukentt�, mihin sy�tet��n oman ryhm�n tunnus. T�ll�in saadaan esille kaikki tietyn koulutusohjelman aineen opettajat. T�m�n j�lkeen avautuu varmistusvalikko, miss� kysyt��n aloitetaanko navigointi ja lis�t��nk� suosikkeihin. 
4. M��rit� n�kymien v�liset siirtym�t korkealla tasolla, mist� n�kym�st� p��see minnekin? Mill� tavoin visualisoisit tilasiirtym�t?
    - p��valikosta siirryt��n etsint�n�kym��n, josta edelleen navigointin�kym��n.
    - p��valikosta voidaan siirty� skannausn�kym��n
    - navigointin�kym�n tai skannausn�kym�n varmistusvalikosta voidaan siirty� suosikkilistoihin, sen j�lkeen kun opettaja/luokka on lis�tty suosikkeihin.
    - p��valikosta p��see k�siksi suosikkilistoihin, infoon ja asetuksiin
    - info-valikosta k�ytt�j� p��see l�hett�m��n palautetta kehitt�jille
5. Listaa jokaista n�kym�� kohti tieto siit�, millaista tietosis�lt�� tai data k�ytt�liittym�ss� n�ytet��n.
    - p��valikko on staattinen ja n�ytt�� kaikki ohjelmiston haarat
    - etsi luokka/opettaja-n�kym�ss� haetaan tietokannasta tietoa. Ohjelma toimii synkronisesti ja tarjoaa eri hakuvaihtoehtoja k�ytt�j�lle t�m�n kirjoittaessa esim. aineen nime�, eli se etenee ns. "tahdistuksen mukaisesti".
    - navigointin�kym� hakee puhelimen kameran sy�tteen ja n�ytt�� sen n�yt�ll�. Puhelin katsoo paikkatietojen perusteella sijainnin ja piirt�� kampuksen 3D-malliin pohjautuen opastusnuolia lattiaan.
    - skannausn�kym� hakee puhelimen kameran sy�tteen ja n�ytt�� sen n�yt�ll�. Kameran reagoidessa luokan oven RFID-tunnukseen, sovellus hakee Metropolian palvelimelta tiedon onko luokka vapaa tai varattu.

#### 3. Visualisoi listaamasi n�kym�t ja niihin liittyv�t siirtym�t

#### P��valikko
  ![Paavalikko](http://users.metropolia.fi/~jarmosep/ohjelmistotuotanto/3.jpg)
  
#### Suosikit
  ![Suosikit](http://users.metropolia.fi/~jarmosep/ohjelmistotuotanto/2.jpg)

#### Navigointi
  ![navigointi](http://users.metropolia.fi/~jarmosep/ohjelmistotuotanto/1.jpg)

**Palauta linkki projektinne tiedostoon (Github), mist� l�ytyv�t vastaukset teht�viin. Vaikka teitte ty�n ryhm�ty�n�, jokainen palauttaa linkin Tuubiin henkil�kohtaisesti.**