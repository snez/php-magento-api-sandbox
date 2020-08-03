# Place a magento order using Stripe via REST API as a guest customer

This is a fork of the example project from [https://github.com/acolono/php-magento-api-sandbox](https://github.com/acolono/php-magento-api-sandbox), modified to work with the Stripe payment method when the Stripe module at https://stripe.com/docs/magento is installed on a Magento 2 website.

## Usage

1. Create api key in Magento:

- Go to: System -> Integrations -> "Add new integration"
- Create a new Integration with sufficient permissions (e.g. set Ressource Access to "All" if you are just playing around)
- Note down the created Access Token for usage in place-order.php

2. Configure place-order.php

Set valid values for `$api_url`, `$token` and `$sku`.

3. Place the order

``php place-order.php``


