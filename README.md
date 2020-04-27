<p align="center"><img width="832" alt="payme-form" src="https://previews.dropbox.com/p/thumb/AAz4g69MsmsAGtCBEiSB_6N-F6Y388NsKd_9ReCpzztfCtgqjPVL2qF7Fm3kjndrdHI1XAkaxU-TYFzA3klVx_ibvprcPnttO97hIKbpPDlaHmB6YCGZCfy6hr-ckRUV_lwCTKQG_3zbZVvkQXdqjSNTFGYHGOa8LTgOXBv2pO6qIx4mR5iMiyk-438HnAjFgo6yo7ZjCUjM9F9SdRnGg7aahApdl58e_KNxUlQmQny05I-YcTeeBWWPIh_gKJLl-jlsfGVU9YlbUpCwOBN3KcAoiLcs1xEWGFu0cw5-_Gn1uKpJo9dD3mBiYtm3QCffGxbEtmeDHUdpKL5V-ZB1ypyuigtwxZKdJHLHTMV8Xve0og/p.png?fv_content=true&size_mode=5">
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
