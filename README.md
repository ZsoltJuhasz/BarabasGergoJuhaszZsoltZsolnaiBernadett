# BudgetApp

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

![Screenshot (7)]

![Screenshot (8)]

![Screenshot (9)]

![Screenshot (10)]

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
