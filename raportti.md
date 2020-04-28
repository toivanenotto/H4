# Palvelinten hallinta - h4

## Modulikimara. Asenna 6 saltin tilaa/modulia. Tässä siis yksi tila/moduli on esimerkiksi Apachen asennus package-file-service rakenteella. Tiloista/moduleista enintään neljä voi olla muiden tekemiä, esimerkiksi verkosta löytyneitä. Muista lähdeviitteet ja lisenssit. Käytä tiloja, joita et ole aiemmin käyttänyt ja joita ei ole käsitelty tunnilla. Tilojen tulee tehdä muutakin kuin pelkästään asentaa yksittäinen paketti, esimerkiksi tehdä sille astuksia (siis vaikka package-file, ei pelkkä package). Asennettavat ja konfiguroitavat ohjelmat voivat olla mitä vain valitset: palvelimia, graafisen käyttöliittymän ohjelmia, komentoriviohjelmia, vapaita, suljettuja... Muista testata lopputulos käyttämällä ohjelmaa sen pääasiallisessa käyttötarkoituksessa. Jos jäät jumiin, tee kaikki mitä osaat ja dokumentoi ongelmat, niin ratkotaan niitä yhdessä.

Aloitin harjoituksen tekemällä githubiin repositorion "H4" ja kloonamalla sen koneelle. Siirryin kansioon ja aloin tekemään tätä raporttia.

Ajattelin asentaa koneelleni aluksi Sayonara-musiikkiohjelman. Loin /srv/salt/ -kansioon uuden kansion ja sinne init.sls-tiedoston.

> sudo mkdir sayonara
> sudoedit init.sls

![sayonara-init](/h4images/sayonara-init.png)

Ja ajoin tilan komennolla

> sudo salt '*' state.apply sayonara

![sayonara-apply](/h4images/sayonara-apply.png)


