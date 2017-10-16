# Virtuaalikone

Kuvauksen kirjoitti: Anton Kiri, K3268

## Lyhyt kuvaus

Virtuaalikone on emuloitu tietokone joka toimii laitteiston pääkäyttöjärjestelmän päällä, jonkin virtualisointi rajapinnan kautta.
Virtuaalikone jakaa saman fyysisen laitteiston kuin pääkäyttöjärjestelmä, mutta käyttäytyy kuin se olisi erillinen laite.
Virtuaalikoneen ei välttämättä tarvitse olla yhteensopiva laitteiston kanssa ohjelmistopohjaisessa virtualisoinnissa, joka mahdollistaa eri käyttöjärjestelmien ajamisen samalla laitteistolla. Esim Windows ja Linux.

![Virtualisoinnin graafi](http://www.ni.com/cms/images/devzone/tut/HostedVirtualizationSmall_20090325191230.PNG)

### Muuta

Virtualisointiin käytetään usein ohjelmistoa, kuten VMware tai VirtualBox.
Myös laitteistopohjainen virtualisointi on mahdollista, mutta usein se ei tarjoa suorituskyky etua ohjelmistopohjaiseen virtualisointiin nähden.

## Esimerkkejä

Useat serverit hyödyntävät virtualisointia, koska se säästää fyysistä tilaa. Käytännössä tämä näkyy niin, että samalla fyysisellä serverillä voi olla NAS (Network Attached Storage) serveri ja useita eri palveluita pyörittäviä servereitä. 

## Lähteitä liittyen aiheeseen

![Laite vs ohjelmisto virtualisointi](https://www.vmware.com/pdf/asplos235_adams.pdf)
![Virtualisoinnin etuja](https://www.vmware.com/pdf/server_consolidation.pdf) 
