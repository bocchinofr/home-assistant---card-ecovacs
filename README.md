# home-assistant-card-ecovacs-N8

Questo progetto non è un installer, ma si tratta di una card personalizzata per il robot aspirapolvere (io ho utilizzato Ecovacs N8 Pro ma può essere adattata ad altri dispositivi).

![Schermata 2023-09-22 alle 12 30 18](https://github.com/bocchinofr/home-assistant---card-ecovacs/assets/102295851/49b5002e-3d37-4afe-b03f-f0c754725cab)

## Installazione package

Come dicevo non c'è un installer, basta aver creato ed attivato la cartella package 
```
homeassistant:
  packages: !include_dir_named packages
```
Una volta creata la cartella basta aggiungere in essa il file package_ecovacs.yaml in questo progetto.
All'interno del file vi sono quasi tutti i sentori, le automazioni e gli script utili per il funzionamento della card (ovviamente personalizzabili).

Nei 3 script di pulizia (giorno, notte, zone) , sono indicate le stanze della casa (si presuppone che siano state aggiunte sull'applicazione ecovacs)

![Schermata 2023-09-22 alle 12 40 09](https://github.com/bocchinofr/home-assistant---card-ecovacs/assets/102295851/7a254dd1-0c8b-40ba-843b-241f5404bf59)

le stanze devono essere modificate in base alle proprie definite.
E' possibile trovare i numeri associati alle stanze tra le proprietà del dispositivo vacuum.<nome_disositivo>

## installazione card

Per installare la card, occorre incollare il codice che trovate all'interno di quqesto progetto "card_ecovacs.yaml" e poi effettuare le modifiche ai vari nomi delle entità.
Il codice può sembrare un pò lungo ma non è difficile da interpretare (nel caso scrivetemi per supporto).

Di seguito una demo delle funzionalità

https://github.com/bocchinofr/home-assistant---card-ecovacs/assets/102295851/3c0ea6a4-a1eb-4172-8359-07f5ae677e03

Per la pulizia delle zone, personalmente ho creto una piantina della casa in 3d e poi ho catturato l'immagine ma può essere utilizzato anche uno screen della piantina creata dall'applicazione ufficiale ecovacs

Tutte le immagini utilizzate nella card ed inserite nelle varie cartelle local sono all'interno di questo progetto.


### Ovviamente è d'obbligo ringraziare domhouse.it da cui ho preso il template della card ed inspirazione.
