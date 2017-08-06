# Freek van der Herten - Spatie.be

## Build a dashboard with Laravel + Vue + Pusher

[GitHub - spatie/dashboard.spatie.be: The source code of dashboard.spatie.be](https://github.com/spatie/dashboard.spatie.be)

Scheduled API calls to refresh dashboard

LastFM to publish music now playing
Laravel Google Calendar

### Grid System
Columns/rows component just like Excel
Yahoo API for the weather (or Forecast.io) refresh periodically

### Packagist tile

Uses Laravel on the backend to fetch the data. Artisan command to fetch data and then broadcast an event on Pusher. Schedule commands every minute or every 5 minutes.

Uses private channel on Pusher and Laravel Echo to fetch the event on the frontend.

Use mixin for echo. Save the state after every update, so the page can be refreshed.

### How to display on TV

Raspberry Pi 2 using Chromium

Resources

Laravel Uptime Monitor
Vue save state

[Dashboard (PHP Limburg) // Speaker Deck](https://speakerdeck.com/freekmurze/dashboard-php-limburg)


