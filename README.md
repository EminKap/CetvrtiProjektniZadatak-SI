# CetvrtiProjektniZadatak-SI

Projekat koji prikazuje jednostavnu primjenu fetch() metode u VanillaJS-u uz GET i POST zahtjeve

Funkcija getPosts šalje GET zahtjev na URL stranice jsonplaceholder.typicode.com, koja nudi razne testne podatke u vidu JSON file-a, koristeći fetch metodu.
Kada se primi odgovor, on se pretvara u JSON format koristeći res.json() metodu.
Dobijeni JSON podaci se zatim koriste za generisanje HTML koda, koji se prikazuje na stranici.

Funkcija addPost koristi se za slanje novih podataka na server.
Kada korisnik pošalje formu, funkcija se pokreće i koristi fetch metodu da pošalje POST zahtjev na isti URL.
Podaci koje korisnik unosi u formu se uzimaju iz polja "title" i "body" i šalju na server u JSON formatu.

Nakon što se podaci pošalju, server vraća odgovor u JSON formatu koji se zatim pretvara u JavaScript objekat pomoću res.json() metode.
U ovom kodu se trenutno samo ispisuje taj objekat u konzoli koristeći console.log(data) jer nemamo pristup serveru jsonplaceholder stranice.
