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

### Instalace

Nginx a Docker jsou momentalne k instalaci skrz libovolneho spravce balicku.
Takze muzeme pouzit nasledujici prikaz na operacnim systemu Ubuntu:
