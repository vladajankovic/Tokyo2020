# Tokyo2020

Tokyo2020 je skolski projekat na predmetu "Programiranje internet aplikacija", koji simulira zvanicni sajt Olimpijskih Igara u Tokiju 2021.
Tehnologija koja se koristila u izradi ovog projekta je **MEAN Stack** (mongoDB, express, node.js, angular).

Da bi se projekat pokrenuo na racunaru, potrebno je da se:
> 1. Instalira **Node.js** sa zvanicnog sajta: https://nodejs.org/en/
>     - uz instalaciju Node.js-a dolazi i **Node package manager - npm** u nastavku.
> 2. U komandnoj liniji izvrsi sledeca naredba: ```npm install -g @angular/cli``` \
>     da bi se omogucio koriscenje angular komandne linije za izvrsavanje angular naredbi
> 3. Instalira **mongoDB** sa zvanicnog sajta: https://www.mongodb.com/
> 4. Instalira **Robo 3T** za laksi rad sa bazom: https://robomongo.org/

Potrebo je skinuti/raspakovati sledece foldere/fajlove sa repozitorijuma: _baze, backend.zip, src.zip i initiate.bat_\
Opciono je napraviti novi folder i u okviru njega pokrenuti komandnu liniju.\
Novi angular projekat se pravi izvrsavanjem sledece komande: \
```
ng new <naziv_projekta>
Angular routing (y/N)? y
Stylesheet: CSS
```
![ng_new](https://drive.google.com/file/d/13by6PHNN6GTyQaknIKl6s-kSr3yyyV9j/view?usp=sharing)\
Posle malo vremena napravice se gotov angular projekat. Sad treba da se folder ***src*** u projektu zameni sa folderom src iz zipovanog fajla.\
Raspakovani folder backend smestiti na istoj lokaciji kao i angular projekat, npr: 
```
C:Users\Student\backend
C:Users\Student\<naziv_projekta>
```
Pre nego sto se projekat pokrene potrebno je napuniti bazu sa podacima. Aplikacija **Robo 3T** je GUI za mongoDB bazu i olaksava nam rad sa samom bazom.
Nakon otvaranja Robo 3T, pravi se nova konekcija sa bazom pritiskom na dugme _File>Connect... (Ctrl + N)_. \
U novo-otvorenom prozoru se noca konekcija pravi kad se klikne na _Create_. \
***Jedino je bitno da se za adresu konekcije stavi ```localhost:27017``` za uspesno povezivanje***\
Radi provere konekcije, postoji dugme _Test_ i ako je sve uredu klikne se na dugme _Save_, pa nakon toga izabere novokreirana konekcija i klikne dugme _Connect_.
Desni klik na _New Connection>Create Database_ i staviti ime ***tokyo2020***. Svaka baza ima 3 foldera, a jedan folder se zove _Collections_. Desnim klikom na taj folder pojavljuje se opcija za kreiranjem nove kolekcije. 
