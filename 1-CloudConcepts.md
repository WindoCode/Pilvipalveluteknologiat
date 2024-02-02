# Luento 1: Cloud Concepts, muodostettu käsinkirjoitetuista muistiinpanoista. (Rocketbook)

## **Monisoinen arkkitehtuuri**
   - Moodle, toimii kolmen eri palvelimen kautta:
     - Tietokanta/palvelin (Asiakastiedot)
     - Sovelluspalvelin (Konfiguraatiot)
     - Verkkopalvelin (HTTP-pyynnöt)

## **AWS CAF = Cloud Adoption Framework**
   - Mitä Huomioitavaa, kun siirrytään pilveen esimerkiksi konesaleista.

## **Virtualisointi**
   - Hyper-V luo raudan päälle virtuaalisen tietokoneen, virtuaalisen verkkokortin yms.

## **AWS-palvelut**
- Laskenta, Verkko, Tallennus, Tietokannat
- Computing, Storage, Networking, Database

## Datakeskus infrastruktuuri:

- Cloud Platform, AWS
- Virtualization Platform, esim. Hyper-V on virtuaalialusta, joka mahdollistaa virtuaalisten tietokoneiden luomisen fyysisen laitteiston päälle.
- JBODs, Just a Bunch of Disks, tallennusratkaisu, jossa useat kiintolevyt yhdistetään yhdeksi suureksi tallennustilaksi.
- Physical Network, verkkokomponentit, kuten kytkimet, reitittimet ja kaapelit, jotka mahdollistavat tietoliikenteen datakeskuksessa.
- Datacenter, fyysinen paikka, jossa tietokoneiden ja palvelimien laitteisto sijaitsee. Näiden sijainnissa huomioidaan esim. sään ja maanjäristyksen riskit.

## AWS Regions

- Regions - EU North
- Availability zone - 3 datakeskusta esim. Ruotsissa
- Local Zone, pieni datakeskus, esim. Helsinki.

## **AWS Hyödyt**

- Keskittyminen omaan bisnekseen. 
- CAPEX vs. OPEX: Siirtyminen pääomakustannuksista (CAPEX) operatiivisiin kustannuksiin (OPEX). Onprem vs Cloud.
- Economics of scale: Taloudelliset hyödyt suurista mittakaavasta, tässä tapauksessa AWS:n hostaamat datakeskukset.
- Kapasiteetin hallinta: Ei tarvetta varautua palvelimien kapasiteetin arvailuun. 
- Palvelimien elastisuus: Lisää palvelimia asiakaspiikkeihin ja vähentää niitä, kun asiakkaat eivät käytä palvelimia.
- Globaali ulottuvuus: AWS toimii monilla alueilla maailmanlaajuisesti. Go global in seconds.

- Pets not cattle ajattelu esim. [Slater 2017](https://github.com/WindoCode/PalvelintenHallinta/blob/main/h2-karjaa.md)
- IAS-Infraa palveluna, IAC-Infraa koodina
- Kaikki lasketaan, automaattinen laskutus

## **Taloudelliset hyödyt**
- Pay as you go, maksat siitä, mitä käytät.
- Tier hinnoittelut
- Maksa heti-alennus
- Osta kpl-määrällisesti enemmän, maksa kpl-hinnassa vähemmän
- BYOL-lisenssit (Bring your own license)

## Pilvimuodot
- Private, fyysiset räkit varattu tietyille organisaatioille.
- Public, jaetaan yhteisesti muiden organisaatioiden kanssa.
- Hybrid, Onprem+Public/Private cloud. Infrastruktuurin yhteydet tärkeät tässä yhteydessä.
- Multi-Cloud, esim AWS+Azure. Siirrettävyys voi olla syy multi-cloudin käytölle + Lailliset velvoitteet, esim. pankeilla.

# Xaas
- SaaS, palvelun esim. sovelluksen osto. Sähköposti, VPN, raportointi-työkalu/sovellus.
- IaaS, laskenta, tallennustila, verkko. Asiakas vastaa esim. virtualisoinnista.
- PaaS, esim. alusta. Data+Sovellukset asiakkaan vastuulla
- Asiakas vastaa turvallisuudesta pilvessä/Alustassaan.




