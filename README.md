# Laravel-Vue SPA 


> A Laravel-Vue SPA starter project template.

## Features

- Laravel 5.6 
- Vue + VueRouter + Vuex + VueI18n + ESlint
- Pages with dynamic import and custom layouts
- Login
- Authentication with JWT
- Socialite integration
- Bootstrap 4 + Font Awesome 5
- CoreUI
- Flags

## Installation

- `composer create-project --prefer-dist cretueusebiu/laravel-vue-spa`
- Edit `.env` and set your database connection details
- (When installed via git clone or download, run `php artisan key:generate` and `php artisan jwt:secret`)
- `php artisan migrate`
- `yarn` / `npm install`

## Usage

#### Development

```bash
# build and watch
npm run watch

# serve with hot reloading
npm run hot
```

#### Production

```bash
npm run production
```
