# Palvelinten hallinta - h4

## Modulikimara. Asenna 6 saltin tilaa/modulia. Tässä siis yksi tila/moduli on esimerkiksi Apachen asennus package-file-service rakenteella. Tiloista/moduleista enintään neljä voi olla muiden tekemiä, esimerkiksi verkosta löytyneitä. Muista lähdeviitteet ja lisenssit. Käytä tiloja, joita et ole aiemmin käyttänyt ja joita ei ole käsitelty tunnilla. Tilojen tulee tehdä muutakin kuin pelkästään asentaa yksittäinen paketti, esimerkiksi tehdä sille astuksia (siis vaikka package-file, ei pelkkä package). Asennettavat ja konfiguroitavat ohjelmat voivat olla mitä vain valitset: palvelimia, graafisen käyttöliittymän ohjelmia, komentoriviohjelmia, vapaita, suljettuja... Muista testata lopputulos käyttämällä ohjelmaa sen pääasiallisessa käyttötarkoituksessa. Jos jäät jumiin, tee kaikki mitä osaat ja dokumentoi ongelmat, niin ratkotaan niitä yhdessä.

Aloitin harjoituksen tekemällä githubiin repositorion "H4" ja kloonamalla sen koneelle. Siirryin kansioon ja aloin tekemään tätä raporttia.

# Sayonara

Ajattelin asentaa koneelleni aluksi Sayonara-musiikkiohjelman. Loin /srv/salt/ -kansioon uuden kansion ja sinne init.sls-tiedoston.

> sudo mkdir sayonara

> sudoedit init.sls

Tiedostoa varten löysin tämän ohjeen https://docs.saltstack.com/en/latest/ref/states/all/salt.states.pkgrepo.html

![sayonara-init](/h4images/sayonara-init.png)

Ja ajoin tilan komennolla

> sudo salt '*' state.apply sayonara

![sayonara-apply](/h4images/sayonara-apply.png)

# Steam

Seuraavaksi päätin asentaa Steamin

Eli aloitin samoilla luomalla alkuun kansion ja init.sls-tiedoston

> sudo mkdir steam

> sudoedit init.sls

Kyseistä tiedostoa varten googlailin Steamin asennusta ja löysin tämän ohjeen https://gist.github.com/garbast/ff5e36d55c11c7558a3b

![steam-init](/h4images/steam-init.png)

Ja tilan ajaminen

> sudo salt '*' state.apply steam

![steam-apply](/h4images/steam-apply.png)


# Lähteet

https://itsfoss.com/sayonara-music-player/
https://gist.github.com/garbast/ff5e36d55c11c7558a3b
