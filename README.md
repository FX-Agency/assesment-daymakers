# DayMakers Assessment

See `ASSESSMENT.md` for details about this project.

## System requirements

- `php 8.4`
- `composer 2`
- `nodejs 22.12+`

## Local installation

The following steps assume you are working on your local / wsl2 environment on this project. If you want to run this project in
docker, you can use Laravel Sail for that.

- `git clone git@github.com:FX-Agency/assesment-daymakers.git`
- `cd assesment-daymakers`
- `composer install`
- `npm ci`
- `cp .env.example .env`
- `php artisan key:generate`
- `php artisan migrate`
- `php artisan storage:link`
- `composer run dev`

## About this project

Starter project for the event registration assessment, using Laravel 13, Inertia 3,
React 19 and Tailwind CSS 4. See `ASSESSMENT.md` for the assignment.
