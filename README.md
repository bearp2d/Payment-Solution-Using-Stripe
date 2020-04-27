<p align="center"><img width="832" alt="payme-form" src="https://drive.google.com/open?id=11n73xUDxtugzbJRHuEJGr4iRLVXAq883">
</p>

---

# PayMe

PayMe is a checkout payment solution built on top of Stripe API.
The application is used as a real-world SaaS example. 

### Demo
Demo is available at [PayMe.rocks](https://payme.rocks)

Test mode is **enabled**, so feel free to create new account and take a look how it works.

## Setup

### Deployment

```
composer install

php artisan view:clear
php artisan cache:clear
php artisan vendor:publish
php artisan migrate

php artisan storage:link
php artisan queue:restart
php artisan config:cache

php artisan horizon:purge
php artisan horizon:terminate

php artisan horizon
```

Then change ```APP_DOMAIN``` to the actual domain name of your app.
Email verification is enabled, so do not forget to set proper SMTP settings for outgoing emails.
