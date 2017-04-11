## Harjoitus 2

# Kotitehtävän raportti GitHubiin MarkDownilla sekä Puppet-moduli

Toteutin tämän tehtävän kokonaan kotikoneellani, jossa Intel Core i5-4430 3.00GHz prossori, NVIDIA GeForce 750ti ja 8Gt keskusmuistia.

Tehtävän ohjeistus löytyi opettajan kotisivuilta: http://terokarvinen.com/2017/aikataulu-%E2%80%93-palvelinten-hallinta-ict4tn022-2-%E2%80%93-5-op-uusi-ops-loppukevat-2017-p2

Aloitin tehtävän vaihtamalla näppäimistökielen komennolla 

$ setxkbmap fi 

ja ajamalla päivitykset Linux versiooni komenolla 

$ sudo apt-get -y update.

Tähän heti perään asensin myös Gitin ja Puppetin komennoilla

$ sudo apt-get intall puppet -y 

$ sudo apt-get intall git -y 

Siirryin sitten www.github.com sivustolle ja sillä tililläni lois uuden repositeryn tälle tehtävälle nimeltä "har2" ja annoin sille lisenssin GNU General Public License v3.0. Tämä ollen valmis saimme uuden valmiin hakemiston jossa tällä hetkellä on vain LICENSE tiedosto.
Napataan repositoryn linkki jotta saamme cloonattua sen terminaaliin komennolla:

$ git clone https://github.com/AAHyv/har2.git

ls komennolla voimme nähdä että har2 kansio on nyt siellä. Siirrytään sinne cd har2/ komennolla ja luodaan sinne tiedosto:

$ nano README.md

Tämä on tiedosto johon teen tällähetkelläkin kyseisen harjoituksen raportointia. Teen välitallennuksen ja päivitän tiedoston tilannetta komennoilla:

$ git add .

$ git commit

Tämä ei onnistunut sillä vaadittiin kirjautumis tunnuksia. Loin nämä virhe ilmoituksen antaman ohjeiden mukaan:

$ git config --global user.email "anna.hyvarinen94@gmail.com"

$ git config --global user.name "Anna Hyvarinen"

Tämän jälkeen ajoin alla olevan komennon jotta jokaisen push/pull tapauksen aikana en joudu syöttämään kirjautumis tietojani uudelleen

$ git config --global credential.helper "cache --timeout=3600"

Kokeilin uudelleen git commit komentoa ja onnistuin johon pivitys viestiksi pistin "CREATED README.MD"

Nyt pitäisi onnistua tiedostomme uppaaminen git'tiin komennoilla:

$ git pull & git push 

Annettuamme GitHubin tunnukset ja salasanat saimme README.md näkyviin selaimeen ja täten myös raportin.

