---
tags:
  - entry
---
[[DDD_책 내용]]

라이브러리 설치
```sh
composer require spatie/laravel-event-sourcing
```
```
php artisan vendor:publish --provider="Spatie\EventSourcing\EventSourcingServiceProvider" --tag="event-sourcing-migrations"
php artisan migrate
```
```
php artisan vendor:publish --provider="Spatie\EventSourcing\EventSourcingServiceProvider" --tag="event-sourcing-config"
```


event 만들기 ([링크](https://spatie.be/docs/laravel-event-sourcing/v7/advanced-usage/preparing-events))
```sh
php artisan make:storable-event
```
make:aggregate
make:projector