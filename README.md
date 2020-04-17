# laravel7-api-boilerplate backend

# Origin
Original Source: https://github.com/cretueusebiu/laravel-nuxt

## cretueusebiu/laravel-nuxt Features
- Socialite integration
- Login, register, email verification and password reset

## Modified
- Upgrade to Laravel 7 based on laravel 6
- Improved Handler Exception
- Added API Responser
- Improved Cors

## Installation

- `composer install`
- `php artisan migrate`
- `php artisan serve`

## Socialite

This project comes with GitHub as an example for [Laravel Socialite](https://laravel.com/docs/5.8/socialite).

To enable the provider create a new GitHub application and use `https://example.com/api/oauth/github/callback` as the Authorization callback URL.

Edit `.env` and set `GITHUB_CLIENT_ID` and `GITHUB_CLIENT_SECRET` with the keys form your GitHub application.

For other providers you may need to set the appropriate keys in `config/services.php` and redirect url in `OAuthController.php`.

## Email Verification

To enable email verification make sure that your `App\User` model implements the `Illuminate\Contracts\Auth\MustVerifyEmail` contract.
