# Magento2 Boilerplate

## How to use

1. Clone this repo
2. Copy and rename _.env.dist_ file to _.env_. If you need you can change some settings there.
3. Add to your system _hosts_ file domain from _.env_ (option _APP_HOST_). We don't recommend to use _localhost_.
4. Build docker images  
   Run this command from project root folder:
   ```
   $ docker-compose build
   ```
5. Run docker stack
   ```
   $ docker-compose up -d
   ```
6. Install Magento via Composer
   ```
   $ docker-compose exec phpfpm composer install -a
   ```
7. Open magento site in your browser. You should see Magento Setup Wizard page.
