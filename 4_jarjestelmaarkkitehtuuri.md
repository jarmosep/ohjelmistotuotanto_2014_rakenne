##  Järjestelmäarkkitehtuuri

![Arkkitehtuurikaavio](http://users.metropolia.fi/~jonioks/arkkitehtuuri.jpg)

### Mobiilisovellus

Track-o-poliaa käytetään pääasiassa mobiililaitteen kosketusnäyttö hyödyntämällä. Fyysisiä näppäimiä ei tarvitse olla laitteessa ollenkaan.

Sovelluksen asentaessaan sovellus pyytää käyttäjältä lupaa käyttää laitteen WLAN-vastaanotinta sekä gyroskooppia. Näiden avulla pystytään koululla sijaitsevien WLAN-tukiasemien ja beaconien avulla tarkasti määrittämään käyttäjän sijainti rakennuksessa. Paikkatieto lähetetään palvelimelle prosessoitavaksi ja reitin laskemista varten.

Skannaamista varten sovellus avaa laitteen kameran ja etsii QR-tageja kameran etsimestä. QR-tagista saatu luokan tunnus lähetetään Metropolian palvelimille tilanvarausjärjestelmään varaustilanteen määrittämiseksi.
