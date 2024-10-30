### Lyhyt kirjoitus

Tee viikolle 2 oma sivu (esimerkiksi vko2.md), jossa kuvailet miten Jekyll sivustoa voisi automatisoida käyttäen GitHub Actions-toimintoja. Vastaa myös millaisilla kehitystyökaluilla ja -tekniikoilla saataisiin CI/CD-putkisto rakennettua web-sovellukselle. Tekstimäärä noin 150 sanaa.

Jekyll-sivuston määritys Github Actionilla tapahtuu asettamalla YAML konffi tiedosto (workflow file) repositoryyn master haaraan. Tiedoston triggeröinti tapahtuu joko manuaalisesti, ajastettuna tai kun muutoksia havaitaan. Konffi tiedosto käynnistää Jekyllin prosessin, jossa ajetaan commitit ja pull requestit, ja automatisoi käyttöönoton (Rubyn ja Jekyllin määritys). Jekyll luo Gem -tiedoston, jossa määritellään versio asennus, lisäosat ja riippuvuudet. Gemfile on Ruby-riippuvuuksien hallintaan, joka määrittää tarvittavat kirjastot Jekyllissä. Jekyll Build luo staattiset sivustot hakemistoon.

Kehitystyökalut ja -tekniikat CI/CD-putkiston rakentamiseen web-sovellukselle esimerkiksi versionhallinta ja sen ylläpito Gitissä (Github), CI/CD alusta, joka automatisoi rakennuksen ja testauksen prosesseja (Github Actions), Säilöt kuten Docker, joka standardisoi sovellusympäristöt testauksessa ja tuotannossa, IaC työkalut kuten Ansible ja Salt, jolla hallitaan infraa koodina ympäristöä, automatisoidut testaustyökalut, valvonta ja lokityökalut (Prometheus, Grafana).
