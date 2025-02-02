# h3 Hello Web Server

## Testataan ping-komennolla, että osoite localhost vastaa.

ping localhost
![ping localhost -> Testataan, että osoite localhost vastaa.](https://github.com/mikacheese/linux-servers/blob/imagesh3/ping_localhost.png)

## Tutkitaan logista onnistunut sivun lataus

sudo tail -2 /var/log/apache2/other_vhosts_access.log
![katsotaan /var/log/apache2/other_vhosts_access.log tiedostosta onnistunut sivun lataus.](https://github.com/mikacheese/linux-servers/blob/imagesh3/Success_1.png)

1. domain name and port: hattu.example.com:80 (80 = http)
2. ip address: 127.0.0.1
3. date & time: 02/Feb/2025:17:50:23 +0200
4. Get sivuston pyyntö, 200 html status onnistunut, 1128 kohteen koko
5. pyytävän selaimen tiedot

## Sivuston luominen ja valmis html5-sivu

Kansion luonti sivustoa varten
![kansion luonti sivustoa varten](https://github.com/mikacheese/linux-servers/blob/imagesh3/www_sivu_kansio.png)

Uuden sivuston conf-tiedoston luonti
![uuden sivuston apache conf tiedoston luonti](https://github.com/mikacheese/linux-servers/blob/imagesh3/hattuexamplecomconf.png)

conf- tiedoston sisältö
![hattu.example.com conf-tiedoston sisältö](https://github.com/mikacheese/linux-servers/blob/imagesh3/sites_availbale.png)

sivuston aktivointi
![sivuston aktivoiminen](https://github.com/mikacheese/linux-servers/blob/imagesh3/a2ensite.png)

Apachen uudelleen käynnistäminen
![apache:n uudelleen käynnistäminen](https://github.com/mikacheese/linux-servers/blob/imagesh3/arestart.png)

hosts tiedoston editoiminen
![host tiedoston editointi](https://github.com/mikacheese/linux-servers/blob/imagesh3/nanohosts.png)

hattu.example.com tiedoston lisääminen hosts-tiedostoon, jotta sitä voi kutsua omalla osoitteella
![hattu.example.com lisääminen hosts tiedostoon, jotta sitä voi kutsua omalla osoitteella](https://github.com/mikacheese/linux-servers/blob/imagesh3/hosts.png)

index.html tiedoston tekeminen, joka on web-sivujen oletus aloitussivu
![hattu.example.com\index.html tiedoston tekeminen, joka on aloitussivu](https://github.com/mikacheese/linux-servers/blob/imagesh3/indexhtml.png)

Valmis hattu... sivu
![valmis sivu hattu...](https://github.com/mikacheese/linux-servers/blob/imagesh3/Hattu_1.png)

Valmis mika... sivu
![valmis sivu mika...](https://github.com/mikacheese/linux-servers/blob/imagesh3/mika.png)

## curl komento

curl komento
![curl-komento näyttää kohdesivun html rakenteen](https://github.com/mikacheese/linux-servers/blob/imagesh3/curl.png)


curl I komento
![curl_I komento näyttää sivuston pyynnön otsaketiedot](https://github.com/mikacheese/linux-servers/blob/imagesh3/curl_I.png)

1. pyynnön tyyppi ja status
2. päivämäärä
3. palvelin ja alusta
4. koska sivua on viimeksi muokattu
5.
6.
7. sisällön koko
8.
9. sisällön tyyppi

