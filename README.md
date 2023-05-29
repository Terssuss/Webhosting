# Webhosting sluzba dokumentace

## Uvod 

Tato dokumentace slouzi jak navod pro nainstalaci a konfiguraci web hostingove sluzby.

## Potrebne programy 

Programy ktere byly vyuzity pro tvorbu teto sluzby:

1. Nginx
    - funguje jako reverse proxy, smerujici provoz do vybraneho kontejneru
    - dale bylo pouzito jako server pro webove stranky


2. Docker
    - diky nemu je mozne spustit vice webovych stranek bez toho aby se vzajemne rusily
    - take na nem bezi reverse proxy

## Instalace

Zezacatku musime naklonovat cely repozitar na system
`git clone https://github.com/Terssuss/Webhosting`
Pokud by certifikaty delaly problem, mozna bude potreba zmenit opravneni.
`chmod 700 *certifikat*`

Dale budeme potrebovat Nginx a Docker, kteri jsou momentalne k instalaci skrz libovolneho spravce balicku.
Takze muzeme pouzit nasledujici prikaz na operacnim systemu Ubuntu:
`sudo apt install nginx docker docker.io`


### Reverse-proxy
    
Reverse proxy musime vytvorit manualne (nevim jak to dat na dockerhub), toho docilime vytvoreni docker image:
```
cd REVERSE-PROXY
sudo docker build -t *nazev_image* .
```
## Konfigurace

Dulezita je konfigurace jednotlivych prvku webhostingu.
Konfigurace je mozna zmenou souboru v REVERSE-PROXY adresari.

## Schema 

![schema]('Webhosting scheme.jpg')
