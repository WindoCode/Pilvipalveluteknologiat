Amazon EBS

- Blokki-tallennus EC-2 instanssien kassa. Blokki-tallennuksen muuttamisessa korvataan vain muttuvat blockit vs. objektitallennuksessa, jossa korvataan koko tiedosto.
- Automaattisesti kopioidaan AZ:lla.
- Nopeampi ja käyttää vähemmän kaistaa, mutta kalliimpi kuin objektitallennus.
- EBS tarjoaa snapshotit tallennustilasta, joilla voidaan DisasterRecovery-suojelua varten.
- Salakirjoitettu, ei lisäkuluja
- Voi muokata dynaamisesti kokoa ja eri tyyppiseksi tallennustilaksi.

Amazon S3
- Data tallennetaan objekteina.
- S3 ei ole kiinni tietyssä serverissä, vaan AWS faciliteetteissa.
- IAM jopa objekti-tasolla.
- Voi olla esim. kuvia,videoita,tekstitiedostoja.
- S3 kasvaa dynaamisesti, eikä sille tarvitse provisioida lisätilaa.
- Maksat siitä mitä käytät
- S3 yhditetään esim. AWS managment console, AWS CLI, AWS SDK:lla.
- S3 tukee esim. staattisen nettisivun tiedostojen ylläpitämistä.

AWS EFS

- Toimii parhaiten esim. big datan, data-analytiikan sekä kotikirjastona.
- Myös dynaaminen provisointi datalle, tuhannet EC2 instanssit voivat lukea EFS:ltä tietoa samaan aikaan.

AWS S3 Glacier
- Turvallinen, kestävä sekä matalahintainen tallennustila esimerkiksi datan arkistointia tai pitkän ajan varmuuskopioita varten.
- Datan saaminen Glacierista voi kestää jopa tunteja.
- Archive = Video,kuva tai tiedosto,jonka on tallentanut glacieriin
- Vault = Kaikki archivet yhden Vaultin sisällä.
- Jokaisella Vaultilla omat IAM-säännöt.
- Kolme vaihtoehtoa tietojen saantiin glacierista.
    - Expedited - 1-5min: kallein
    - Standard - 3-5 tuntia
    - Bulk - 5-12 tuntia
- Tieteelisten aineistojen arkistoinnit, Terveystiedot, oikeudelliset arkistoinnit.
- Glacieria voidaan käyttää S3:sen kanssa yhdessä, esim. tiedostojen elinajan kanssa. Esim. jos tiedostoa ei käytetä 3kk aikana, se siirretään glacieriin ja poistoon.
