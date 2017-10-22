# Ylläpito (Maintenance)
Kuvauksen kirjoitti: Juuso Minkkilä K1756

## Lyhyt kuvaus ylläpidosta
Ohjelmiston ylläpito on sen julkaisun jälkeistä muokkaamista muun muassa vikojen korjaamiseksi tai ohjelmiston ominaisuuksien parantamiseksi.
Se on oleellinen osa ohjelmiston elinkaarta, ja voidaan jakaa neljään eri kategoriaan (ISO/IEC 14764):

 * Korjaava ylläpito - keskittyy ohjelmistossa ilmenneiden ongelmien korjaamiseen
 * Ennaltaehkäisevä ylläpito - keskittyy yleensä ohjelmiston luotettavuuden tai huollettavuuden parantamiseen, tarkoituksena estää mahdollisia tulevia ongelmia
 * Mukauttava ylläpito - ohjelmiston muokkaamista sen saattamiseksi yhteensopivaksi sen ympäristössä tapahtuneisiin muutoksiin
 * Täydellistävä ylläpito - ohjelmiston muuta muokkaamista sen elinkaaren pidentämiseksi, kuten käytettävyyden parantamista tai uusien käyttäjävaatimusten mukaisten ominaisuuksien lisäämistä

Toisin kuin usein luullaan, suurin osa ylläpidosta ei liity vikojen korjaamiseen. Sen osuus on usein noin 20%. Yllätyksenä voi myös tulla ylläpidon hinta, joka yksinään on yleensä noin 50% suurempi, kuin muiden ohjelmiston elinkaaren osien hinnan summa. Tämän vuoksi on tärkeää, että ohjelmiston ylläpitosuunnitelmaa aletaan tehdä jo hyvissä ajoin ohjelmiston kehitysvaiheessa. Tämän tulisi sisältää muun muassa budjettiarvio, ylläpidosta vastuussa olevat tahot, sekä selite siitä, kuinka käyttäjät voivat ilmoittaa vioista.

## Ylläpitoprosesseja
Tässä on joitakin esimerkkejä ylläpitoprosesseista.

 1. **Implementaatioprosessi** alkaa jo ennen ohjelmiston julkaisua. Tähän sisältyvät esimerkiksi ohjelmiston suoritusympäristön esivalmistelu, heti julkaisun jälkeinen konfigurointi, sekä ennen julkaisua tunnistettuihin ongelmiin varautuminen.
 2. **Ongelmien ja muutosten analysointia** aletaan suorittaa, kun vastuu ohjelmistosta on siirtynyt siitä vastaavalle ylläpitoryhmälle. Ryhmän kuuluu validoida, dokumentoida, ja mahdollisesti ratkaista kaikki sille raportoidut ongelmat.
 3. **Tarvittavien muutosten implementoinnin harkinta ja hyväksyntä** tapahtuu, kun jotain osaa ohjelmistosta halutaan muuttaa. Ensin on harkittava, kuinka muutos implementoidaan, jonka jälkeen on tarkistettava, tarjosiko muutos tarvittavan ratkaisun.
 4. **Migraatio** on harvinainen ylläpitoprosessi, joka suoritetaan jos esimerkiksi joudutaan siirtymään yhdestä käyttöympäristöstä toiseen.
 5. Ohjelmiston elinkaaren lopussa voidaan suorittaa sen **käytöstä poistaminen** (retirement)

## Uudelleensuunnittelu
Uudelleensuunnittelu on paljon resursseja kuluttava ohjelmiston ylläpitoprosessi, joka on kuitenkin varsin tärkeää sen ajantasaisuuden kannalta. Yleensä uudelleensuunnittelu koostuu kolmesta tärkeästä aliprosessista: takaisinmallintamisesta, uudelleenjärjestämisestä, sekä eteenpäinmallintaminen.

 * **Takaisinmallintamisessa** periaatteessa tehdään speksit olemassaolevan ohjelmiston pohjalta. Tarkoituksena on ymmärtää, kuinka ohjelmisto on suunniteltu sen lähdekoodin pohjalta.
 * **Uudelleenjärjestämisessä** nimensä mukaisesti uudelleenjärjestellään ohjelmaa. Käytännössä tämä tarkoittaa lähdekoodin ja ohjelman käyttämän datan uudelleenjärjestelyä sen toiminnallisuutta muuttamatta. Tämän tarkoituksena on usein parantaa ohjelmiston ylläpidettävyyttä ja luotettavuutta, esimerkiksi virhealttiita ohjelmakomponentteja muuttamalla. Tarvittaessa voidaan koodin uudelleenjärjejämisessä käyttää eri ohjelmointikieltä, kuin mitä alkuperäisessä ohjelmistossa on käytetty.
 * **Eteenpäinmallintamisessa** tuotetaan "valmis" tuote takaisinmallintamisen ja uudellenjärjestämisen pohjalta.

## Tiivistelmä

 * Muotoja: korjaava, ennaltaehkäisevä, mukauttava & täydellistävä
 * Alkaa jo ennen kuin ohjelmisto julkaistaan
 * Tähänkin löytyy standardi (ISO/IEC 14764:2006)

## Lähteitä liittyen aiheeseen
https://en.wikipedia.org/wiki/Software_maintenance

https://www.tutorialspoint.com/software_engineering/software_maintenance_overview.htm

https://fi.wikipedia.org/wiki/Ohjelmistotuotanto#Yll.C3.A4pito

Hyvä diasarja aiheesta: http://www.mit.jyu.fi/opetus/kurssit/jot/2006/luennot/yllapito.pdf

Uusin virallinen standardipaperi (ISO/IEC 14764:2006), maksaa noin 138€: https://www.iso.org/standard/39064.html

Vanhentunut IEEE standardipaperi: http://www.cs.uah.edu/~rcoleman/CS499/CourseTopics/IEEE_Std_1219-1998.pdf

## Linkit muihin wikisivuihin

https://github.com/JAMKPROJ/TTOS1000-GT0/blob/master/vika.md

https://github.com/JAMKPROJ/TTOS1000-GT0/blob/master/vikaraportti.md

https://github.com/JAMKPROJ/TTOS1000-GT0/blob/master/suppport-person.md

https://github.com/JAMKPROJ/TTOS1000-GT0/blob/master/muutospyynto.md

https://github.com/JAMKPROJ/TTOS1000-GT0/blob/master/defectdatabase.md

https://github.com/JAMKPROJ/TTOS1000-GT0/blob/master/reverse-engineering.md
