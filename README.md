# responsiveSmallMedium

Potpuno responsive layout bez korišćenja framework-a. Korišćen je Mobile First pristup.

![Alt text](screenshots/small.png?raw=true "Small layout")

Layout je inicijalno kodiran za male ekrane. Potom su definisane dve prelomne tačke: Za srednje ekrane: 768px - 992px i za velike ekrane >= 922px.

Tablet layout izgleda ovako:
 
![Alt text](screenshots/medium.png?raw=true "Medium layout")

Sekcija za postove je realizovana na sledeci nacin:

/* kontejner za postove */

.posts { display: flex; flex-direction: row; flex-wrap: wrap;}

.post { flex: 1 1 45%; }

...pri cemu 45% predstavlja širinu bloka, tako da u jednom redu mogu stati maksimalno dva bloka. Ta procentualna vrednost je promenjena u Media Query-u za velike ekrane na 30%, kako bi u jednom redu stala tri bloka.

![Alt text](screenshots/large.png?raw=true "Medium layout")
