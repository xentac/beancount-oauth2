To use you will need to do a few things:

* Fill in `<yourdomain>` in all files
* Changes in `docker-compose.yml`
  * Follow the instructions for [oauth2_proxy](https://github.com/bitly/oauth2_proxy/) and fill in `<client-id>`, `<client-secret>`, and `<cookie-secret>`
  * Change `/absolute/path/to/beancount/directory` to the path of your beancount directory
  * Fill in `<beancount.filename>`
* Changes in `authenticated-emails`
  * List emails of people you want to have access to your beancount site
* Store nginx compatible crt and key files in the nginx directory called `sslcert.crt` and `sslcert.key` respectively

To start everything run `docker-compose up`.
