## About

Use this sample PHP code to place a Magento 2 order using the Stripe payment method via REST API as a guest customer.

Forked from [https://github.com/acolono/php-magento-api-sandbox](https://github.com/acolono/php-magento-api-sandbox), modified to work with the Stripe payment method when the Stripe module at [https://stripe.com/docs/magento](https://stripe.com/docs/magento) is installed on a Magento 2 website.

### Example

[https://stripe-magento2.cryozonic.com/3d_secure.html](https://stripe-magento2.cryozonic.com/3d_secure.html)

### Usage

Step 1: Create an API key in Magento:

  - Go to: System -> Integrations -> "Add new integration"
  - Create a new Integration with sufficient permissions (e.g. set Ressource Access to "All" if you are just playing around)
  - Note down the created Access Token for usage in place-order.php

Step 2: Configure place-order.php

  - Set valid values for `$api_url`, `$token` and `$sku`.

Step 3: Place the order

*Via the CLI*

```sh
php place-order.php
```

*Using a 3D Secure Card*

Edit 3d_secure.html and set your Publishable Key.

Visit yourdomain.com/3d_secure.html and click the place order button.


