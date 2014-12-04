##  Järjestelmäarkkitehtuuri

![Arkkitehtuurikaavio](http://users.metropolia.fi/~jonioks/arkkitehtuuri.jpg)

### Mobiilisovellus

Track-o-poliaa käytetään pääasiassa mobiililaitteen kosketusnäyttöä hyödyntämällä. Fyysisiä näppäimiä ei tarvitse olla laitteessa ollenkaan.

Sovelluksen asentaessaan sovellus pyytää käyttäjältä lupaa käyttää laitteen WLAN-vastaanotinta sekä gyroskooppia. Näiden avulla pystytään koululla sijaitsevien WLAN-tukiasemien ja beaconien avulla tarkasti määrittämään käyttäjän sijainti rakennuksessa. Paikkatieto lähetetään palvelimelle prosessoitavaksi ja reitin laskemista varten.

Skannaamista varten sovellus avaa laitteen kameran ja etsii QR-tageja kameran etsimestä. QR-tagista saatu luokan tunnus lähetetään Metropolian palvelimille tilanvarausjärjestelmään varaustilanteen määrittämiseksi.

Käyttäjällä on myös mahdollisuus sovelluksen kautta lähettää palautetta kehittäjille

###Palvelinohjelmisto

Track-o-polia sovellus pyörii omalla palvelimellaan ja sisältää useita eri aliohjelmia, joille on määritelty omat tehtävänsä.

Paikkatietokanta pitää sisällään tiedon kaikkien WLAN-tukiasemien ja beaconien sijainneista, jotta käyttäjän saamien WLAN-signaalien perusteella voidaan laskea missä hän on. Tämä toimii koko navigaatiotoiminnon perustana. Tietokanta sisältää myös luokkien sijainnit, jotta käyttäjä voidaan opastaa oikeaan paikkaan. Paikkatietojen käsittelijä käsittelee käyttäjältä saatuja paikkatietoja ja vertaa käyttäjän nykyistä sijaintia luokan sijaintiin, johon käyttäjä haluaa. Käsittelijä laskee lyhyimmän mahdollisen reitin luokkaan ja kutsuu navigointiopasteiden renderöijää.

Navigointiopasteiden renderöijä piirtää puhelimen näytölle ruudulle opastenuolia käyttäjän opastamiseksi oikeaan luokkaan. Opasteet renderöijä saa navigointiopastekirjastosta, jossa säilytetään kaikki erilaiset opastemerkit.

Palvelinohjelmisto pitää yllä reaaliaikaista seurantaa opettajien sijainnista koulussa, jotta navigointi heidän luokseen onnistuu mahdollisimman nopeasti. Reaaliaikaisen seurannan rinnalla toimii opettajatietokanta, johon on tallennettuna jokaisen opettajan opettamat aineet, yhteystiedot ja työhuone.

Käyttäjän tallentamat suosikkiluokat tallenetaan puhelimen fyysiseen muistiin, mutta myös palvelimen suosikkitietokantaan. Täten suosikit eivät koskaan häviä vaikka sovellusta käytettäisiin toisella laitteella.

Metropolian palvelimiin pidetään yhteyttä yhteyssovelluksella, jolla saadaan tietoja luokkien varaustilanteista ja niissä olevista ohjelmistoista.

###Metropolian palvelimet

Metropolian palvelimilla sijaitsevat opiskelijapalvelut lukkarikone ja tilanvarausjärjestelmä ovat pääasialliset toiminnot, joita Track-o-polia käyttää hyväkseen. Lukkarikoneen kautta voidaan suoraan käynnistää navigointi haluttuun luokkaan yksinkertaisesti luokan tunnusta painamalla.

Tilanvarausjärjestelmästä haetaan skannaustoiminnolla saadulla luokan tunnuksella luokan varaustilanne sekä siellä olevat ohjelmistot.
