# BudgetApp

## Közreműködők

* Barabás Gergő 
- Back-end
- Adatbázis tervezés 
* Juhász Zsolt
- Front-end
- Dokumentáció
- Adatbázis megvalósítást
* Zsolnai Bernadett
- Asztali alkalmazás


## A pénzmozgás követő alkalmazásról

Tulajdonságok:
- Napi bevételek, költségek vagy bármilyen megjegyzés hozzáadása, szerkesztése, törlése.
- Az irányítópulton megtekintheti az e havi költségeit, bevételeit, és egyenlegét is.
- A programban található egy Javascriptel készült számológép. Ezzel lehet számolni(kivéve a negatív értékeket, azt az alkalmazás megoldja).
- Ezenkívül láthatja az összefoglalót az összes bevételről és kiadásról, láthatja az e havi és az eddig megtörtént összes tranzakciót az alkalmazásunkban. 


## Installation process/Telepítési folyamat

Clone this repository/Klónozza az alábbi tárhelyet-
```sh
git clone https://github.com/ZsoltJuhasz/BarabasGergoJuhaszZsoltZsolnaiBernadett.git
```
Go to the project folder/ Menjen bele a projekt mappájába
```sh
cd web cd budgetApp
```
Copy .env.example to .env/ Mésolja le a .env.example mappa tartalmát és nevezze át .env-re
```sh
cp .env.example .env
```
Install composer for vendor file/ Telepítse a composert
```sh
composer install
```
Create a database and set the database name to the same as the one you created in phpMyAdmin in the .env file,
then run the composer update (if necessary) and php artisan key: generate.
Then check the correct php version (7.3.10). If you don't have this php version on your machine, then
you can watch this tutorial video. This is a video on how to change your php version in xampp
https://www.youtube.com/watch?v=wtgiEluCbhc

Hozzon létre egy adatbázist, és állítsa be az adatbázis nevét ugyanarra, amelyet a phpMyAdmin programban hozott létre az .env fájlban,
majd futtasd a zeneszerző frissítést (ha szükséges) és a php artisan kulcsot: generáld.
Ezután ellenőrizze a megfelelő php verziót (7.3.10). Ha nincs a számítógépén ez a php verzió, akkor
megtekintheti ezt az oktatóvideót. Ez egy videó a php verzió megváltoztatásáról xampp-ban
https://www.youtube.com/watch?v=wtgiEluCbhc

Run migrate (--seed for faker data) Futassa a migrációs parancsot (--seed kapcsoló a fakerrel feltöltött adatok miatt szükséges)
```sh
php artisan migrate --seed
```
Then run / Ezek után futassa(indítsa el a szervert)
```sh
php artisan serve
```
GoTo [http://127.0.0.1:8000](http://127.0.0.1:8000) for visiting your budget tracker app

Majd ezután nyissa meg a következő linket a böngészőben(ctrl + bal klikk az egeren) <http://127.0.0.1:8000>

For the first Login:

**email: admin@admin.com**

**password: password**

Az első bejelentkezéshez: 

**email: admin@admin.com**

**password: password**
