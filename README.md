# BudgetApp
(Az alkalmazás és a projekthez tartozó leírás a web mappában található)

## Közreműködők

* Barabás Gergely
* Juhász Zsolt
* Zsolnai Bernadett

## About Budget App

Features:
- Add, Edit, Delete Daily income,expense or any Note.
- In the Dashboard you can see This month Cost with how many income, expense and balance also.
- It has a calculator made with JS.You can calculate with this.
- And also you can see all your summary like all income and expense from all time that you added in this software.


## Screenshot

![Screenshot (7)](https://user-images.githubusercontent.com/40033062/66742324-364e0300-ee99-11e9-98c3-2ab492bd154d.png)

![Screenshot (8)](https://user-images.githubusercontent.com/40033062/66742412-64334780-ee99-11e9-99dc-6031ebb16cad.png)

![Screenshot (9)](https://user-images.githubusercontent.com/40033062/66742420-69909200-ee99-11e9-8fa5-ce8c95007823.png)

![Screenshot (10)](https://user-images.githubusercontent.com/40033062/66742428-6d241900-ee99-11e9-9089-e1bd2e2311ad.png)

## Installation Process

Clone this repository-
```sh
git clone https://github.com/ZsoltJuhasz/BarabasGergoJuhaszZsoltZsolnaiBernadett.git
```
Go to the project folder
```sh
cd web cd budgetApp
```
Copy .env.example to .env 
```sh
cp .env.example .env
```
Install composer for vendor file
```sh
composer install
```
Create a database and set information to .env,
after that run composer update(if it is needed) and php artisan key:generate
and check for the right php version (7.3.10) if this isn't the correct version then 
this is a video how to set up your php version in xampp 
https://www.youtube.com/watch?v=wtgiEluCbhc


Run migrate (--seed for faker data)
```sh
php artisan migrate --seed
```
Then run 
```sh
php artisan serve
```
GoTo [http://127.0.0.1:8000](http://127.0.0.1:8000) for visiting your budget app

For Login:

**email: admin@admin.com**

**password: password**
