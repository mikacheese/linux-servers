# h2 Komentaja Pingviini



## sudo apt-get update -> repositorien eli pakettilähteiden päivitys.  

![sudo apt-get update -> repositorien eli pakettilähteiden päivitys](https://github.com/mikacheese/linux-servers/blob/imagesh2/update.png)

## sudo apt-get upgrade -> ohjelmien päivitys  

![sudo apt-get upgrade -> ohjelmien päivitys](https://github.com/mikacheese/linux-servers/blob/imagesh2/update.png)

## clear -> comentorivin tyhjennys.  



## a) & b) sudo apt-get install bash-completion nano vim micro cowsay lshw -> ohjelmien asennus.  

![a) & b) sudo apt-get install bash-completion nano vim micro cowsay lshw -> ohjelmien asennus](https://github.com/mikacheese/linux-servers/blob/imagesh2/install.png)



## c) FHS.  

ls -> tiedostolistaus  

tree -> hakemistorakenteen puumainen listaus  

/ -> juurihakemisto (root...)  

/home/ -> kaikkien käyttäjien hakemistot  

/home/joku/ -> joku nimisen henkilön kotihakemisto  

![Hakemistoissaliikkumista](https://github.com/mikacheese/linux-servers/blob/imagesh2/Hakemistoissaliikkumista.png)

/etc/ -> järjestelmän asetukset yms  

![/etc/ -> järjestelmän asetukset yms](https://github.com/mikacheese/linux-servers/blob/imagesh2/etc_sourceslist.png)

/media/ -> siirrettävät mediat  

![/media/ siirrettävät mediat](https://github.com/mikacheese/linux-servers/blob/imagesh2/media.png)

/var/log/ -> logitiedostot  



## d) The Friendly M. 3 kuvaavaa esimerkkiä grep-komennon käytöstä.  

grep bridge rauta.txt -> etsii tiedostosta rauta.txt rivit, joilla lukee bridge  

![grep bridge rauta.txt -> etsii tiedostosta rauta.txt rivit, joilla lukee bridge](https://github.com/mikacheese/linux-servers/blob/imagesh2/Grep1.png)

grep bridge -A3 -B2 rauta.txt -> etsii tiedostosta rauta.txt rivit, joilla lukee bridge ja tulostaa 3 seuraavaa ja 2 edellistä riviä  

![grep bridge -A3 -B2 rauta.txt -> etsii tiedostosta rauta.txt rivit, joilla lukee bridge ja tulostaa 3 seuraavaa ja 2 edellistä riviä](https://github.com/mikacheese/linux-servers/blob/imagesh2/Grep2.png)

grep [A-Z] rauta.txt  -> Näytetään tiedostosta rauta.txt rivit, joissa on iso kirjain  

![grep [A-Z] rauta.txt  -> Näytetään tiedostosta rauta.txt rivit, joissa on iso kirjain](https://github.com/mikacheese/linux-servers/blob/imagesh2/grep3.png)



## e) Pipe.  

uname -r | cowsay -> putkitus ytimen versio lehmälle  

![uname -r | cowsay -> putkitus ytimen versio lehmälle](https://github.com/mikacheese/linux-servers/blob/imagesh2/Putkitus.png)






