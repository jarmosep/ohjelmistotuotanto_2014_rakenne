## Johdanto

Tämän projektin tarkoituksena on kehittää Metropolian Leppävaaran toimipisteelle lisättyä todellisuutta (augmented reality) hyödyntävä navigointipalvelu, jonka avulla opiskelijat pystyvät paikantamaan ja navigoimaan haluamiensa luokkien luokse tai tarkastamaan vapaan luokan saatavuuden. Palvelua käytetään kannettavissa älylaitteissa. Koska sovelluksessa käytetään lisättyä todellisuutta, navigointimenetelmänä hyödynnetään älylaitteiden kameroita. Ruudulla näkyy mm. 3D-grafiikkaa hyödyntäviä opastusnuolia ja metrilaskureita, jotka kertovat kohteen sijainnin ja ohjeistavat käyttäjää reaaliajassa. Sovellus vaatii älylaitteelta myös gyroskoopin ja wi-fi-yhteyden toimiakseen.

Vapaiden tai varattujen luokkien tarkastusta varten puhelimessa on myös toiminto, jossa luokan ovi/tunnus skannataan ja tieto luokan nykytilasta saadaan älylaitteen ruudulle. Järjestelmää pystytään hyödyntämään jo olemassa olevan Metropolian mobiilipalvelun Ihanan kanssa. Kun opiskelija hakee Ihanasta lukujärjestystään ja klikkaa jotain tiettyä kurssia, Track-O-Polia sovellus käynnistyy ja aloittaa ohjeistuksen. Ihana näyttää **mitä** informaatiota saadaan - Track-o-polia kertoo **miten** informaation luokse pääsee.  

Tässä vaatimusmäärittelyssä pyritään kuvaamaan mahdollisimman tarkasti, millaisia käyttötapauksia navigointipalvelulla on, sekä millaisen järjestelmäarkkitehtuurin ja käyttöliittymän kyseinen palvelu vaatisi.

Navigointipalvelua tarvitaan, koska suunnistaminen oppilaitoksessa on haastavaa varsinkin uusille opiskelijoille, mutta myös vanhoillekin. Opettajatkaan eivät aina ole varmoja onko jokin tietty luokka varattu opetusta varten.
