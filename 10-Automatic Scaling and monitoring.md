# Automatic Scaling and monitoring
## Elastic Load Balancing
- Jakaa app/verkkoliikenteen usealle kohteelle joko yhdelle avail zonelle tai useammalle.
### Application load balancer
- Toimii sovellustasolla ( OSI 7 )
- Reitittää liikennettä kohteille sisällön perusteella.
- HTTP/HTTPS-liikentelle
- TLS+SSL varmenteet päivitetty load balancerin avulla

### Network load balancer
- Network-tasolla (osi 4)
- Reitittää yhteydet IP-protokolla datan avulla
- Toimii hyvin TCP ja UDP-liikenteen load balancaamiseen.

### Classic Load Balancer
- Toimii niin app että verkko tasolla.
- Kuormanjako niin HTTP/HTTPS/TCP/SSL liikenteelle.

## Amazong CloudWatch
- Monitoroi: AWS-resursseja ja sovelluksia jotka pyörii AWS:ssä.
- Kerää ja seuraa: Joko yleisiä metriikoita tai muokattuja metriikoita.
- Hälyttää: Joko lähettää ilmoituksen tai tekee EC2-auto scaling toiminnon

## Amazon EC2 Auto Scaling
- Auttaa ylläpitämään sovelluksen saatavuutta
- Lisää automaattisesti tai poistaa EC2 instansseja, määriteltyjen ehtojen mukaan.
- Tunnistaa heikot instanssit sekä vanhentuneet sovellukset, ja uusii instanssit puolestasi.
- Skaalautuvuuden voi tehdä usealla tavalla: Manuaali,aikataulutettu, dynaaminen tai ennustamalla.
- SCALE OUT = LUO uuden instanssin
- SCALE IN = Poistaa instanssin (terminate)



