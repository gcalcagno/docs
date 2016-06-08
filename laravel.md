####GULP

#
gulp watch

####MIGRATE
php artisan migrate
#
php artisan db:seed

#ENVIO DE EMAILS CON GMAIL
#####Activar envio de email en cuenta gmail para aplicaciones
https://www.google.com/settings/security/lesssecureapps and active it.
#

#####composer.json
"guzzlehttp/guzzle": "~5.3|~6.0",
#

#####.env
MAIL_DRIVER=smtp
MAIL_HOST=smtp.gmail.com
MAIL_PORT=587
MAIL_USERNAME=desarrollowirall1@gmail.com
MAIL_PASSWORD=P4ss10nfru1t
MAIL_ENCRYPTION=tls
