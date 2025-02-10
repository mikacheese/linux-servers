# h4 Maailma Kuulee


## Valitaan VPS-palvelutarjoaja, rekisteröidytään asiakkaaksi ja luodaan palvelin


Valitsin Hetznerin palveluntarjoajaksi, koska tiesin sen entuudestaan hyväksi vaihtoehdoksi; rahalle paras vastine, Saksalainen yritys jolla datacenter Suomessa Tuusulassa.


Ensin tutkin eri vaihtoehtoja Hetznerin sivuilta ja valitsin tähän käyttötarkoitukseen mielestäni optimaalisimman.


![Valitaan palveluntarjoaja.](https://github.com/mikacheese/linux-servers/blob/imagesh4/1Hetzner.png)


Sitten suoritin rekisteröitymisen asiakkaaksi, tunnistauduin konservatiivisella Saksalaisella tavalla passin ja web-kameran kuvan avulla ja annoin muiden tietojeni ohella maksutiedot.


![Rekisteröityminen.](https://github.com/mikacheese/linux-servers/blob/imagesh4/2TilinLuonti.png)


Hetznerillä uuden palvelimen luonti tapahtuu aloittamalla uusi projekti.


![Palvelimen luonti.](https://github.com/mikacheese/linux-servers/blob/imagesh4/3UudenPalvelimenLuonti.png)


Sen jälkeen päästään luomaan varsinaista virtuaalipalvelita ja ensimmäinen tehtävä on valita datakeskuksen sijainti - Helsinki.


![Valitaan datakeskuksen sijainti.](https://github.com/mikacheese/linux-servers/blob/imagesh4/3DataKeskuksenSijainti.png)


Seuraavaksi valitaan asennettava käyttöjärjestelmä - Debian 12.


![Valitaan Käyttöjärjestelmä.](https://github.com/mikacheese/linux-servers/blob/imagesh4/5Kayttojarjestelma.png)


Valitaan palvelimen resurssit, joka samalla määrittää peruspaketin hinnan.


![Valitaan palvelimen resurssit.](https://github.com/mikacheese/linux-servers/blob/imagesh4/6Resurssit.png)


Valitaan IP_osoitteen tyyppi.


![Valitaan IP-osoitteen tyyppi.](https://github.com/mikacheese/linux-servers/blob/imagesh4/7IP_Osoite.png)


Käydään välillä luomassa omalla Linux-koneella ssh-key.


![ssh-keyn luonti.](https://github.com/mikacheese/linux-servers/blob/imagesh4/11shkeyluonti.png)


Otetaan julkinen ssh-key talteen palvelinta varten.


![Julkinen ssh-key.](https://github.com/mikacheese/linux-servers/blob/imagesh4/12Julkinenssh.png)


Lisätään julkinen ssh-key palvelimelle


![ssh-keyn lisääminen.](https://github.com/mikacheese/linux-servers/blob/imagesh4/8SSHKeynLisaaminen.png)


Annetaan palvelimella nimi, tarkistataan lopullinen hinta ja luodaan palvelin.


![Palvelimen nimi ja lopullinen hinta.](https://github.com/mikacheese/linux-servers/blob/imagesh4/8PalvelimenNimiHinta.png)


Nyt kun palvelin on valmis, nähdään sen IP-osoite.


![Palvelimen IP.](https://github.com/mikacheese/linux-servers/blob/imagesh4/10IP.png)


## Palvelimen käyttäminen etäyhteydellä.


Kirjaudutaan root-käyttäjänä palvelimella.


![Kirjautuminen root:na ssh:lla.](https://github.com/mikacheese/linux-servers/blob/imagesh4/14sshkirjautuminen.png)


Päivitetään repository.


![Repositoryn päivitys.](https://github.com/mikacheese/linux-servers/blob/imagesh4/repositorypaivitys.png)


Päivitetään järjestelmä.


![Päivitetään järjestelmä.](https://github.com/mikacheese/linux-servers/blob/imagesh4/paivitys1.png)


Avataan palomuurista portti 22 ssh yhteyttä varten.


![Portin 22 (ssh) avaaminen.](https://github.com/mikacheese/linux-servers/blob/imagesh4/15portti22.png)


Avataan palomuurista portti 80 http yhteyttä varten.


![Portin 80 (http) avaaminen.](https://github.com/mikacheese/linux-servers/blob/imagesh4/16portti80.png)


Käynnistetään palomuuri.


![Palomuurin käynnistys.](https://github.com/mikacheese/linux-servers/blob/imagesh4/palomuuri.png)


Lisätään normaalikäyttäjä.


![Käyttäjän lisääminen.](https://github.com/mikacheese/linux-servers/blob/imagesh4/kayttaja.png)


Lisätään äsken luotu käyttäjä sudo-ryhmään, jotta käyttäjä voi suorittaa pääkäyttjän tehtäviä.


![Käyttäjä sudo - ryhmään.](https://github.com/mikacheese/linux-servers/blob/imagesh4/kayttajasudo.png)


Kirjaudutaan palvelimelle äsken luodulla käyttäjällä.


![Kirjatuminen käyttäjänä ssh:lla.](https://github.com/mikacheese/linux-servers/blob/imagesh4/kirjautuminenml.png)


Muokataan vielä sudoers tiedostoa, että saadaan ajastettua päivitykset cron:lla.


![Sudoers-tiedoston muokkaus päivitysten automatisoinniksi cron:lla .](https://github.com/mikacheese/linux-servers/blob/imagesh4/sudoerstiedostonmuokkaus.png)


Sudoers tiedostoon lisätty rivi antaa oikeuden ajaa "sudo apt-get update" ja "sudo apt-get upgrade" komennot ilman salasanaa sudo ryhmään kuuluville.


![Sudoers-tiedostoon lisätty rivi.](https://github.com/mikacheese/linux-servers/blob/imagesh4/sudoers.png)


## Domainin hankkiminen.


Hankin domainin Zonerilta, koska heillä oli hyvä alennus .fi domainista ja entuudestaan tiesin Zonerin hyväksi ja luotettavaksi kotimaiseksi palveluntarjoajaksi.


Domainin hallinassa kävin tekemässä tarvittavat ohjaukset.


![Zoner DNS asetukset.](https://github.com/mikacheese/linux-servers/blob/imagesh4/DNS.png)


Valmista tuli http://mikacheese.fi .


![Valmis www-sivu http://mikacheese.fi ](https://github.com/mikacheese/linux-servers/blob/imagesh4/websivu.png)
