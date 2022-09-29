[![Codacy Badge](https://app.codacy.com/project/badge/Grade/9846aeebc05b4d5d96d837af975836c2)](https://www.codacy.com/gh/clopenclassrooms/p7/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=clopenclassrooms/p7&amp;utm_campaign=Badge_Grade)

# Bilemo REST API

## Installation
```Bash
git clone https://github.com/c-lanon-dev/REST_API_with_Symfony.git
cd REST_API_with_Symfony
chmod +x run.sh config.sh config_db.sh
./run.sh
```
when all containers is launch (Ony for first launch)
```Bash
./config.sh
```

## REST API documentation
You can find the complete REST API documentation [here](https://github.com/c-lanon-dev/REST_API_with_Symfony/blob/main/Documentation/documentation.md)

## Test REST API
You can use this [Postman file](https://github.com/c-lanon-dev/REST_API_with_Symfony/blob/main/Documentation/Postman.json) for test the REST API.

The token is automatically add from the "GET /api/login" resquest : 
![](https://github.com/c-lanon-dev/REST_API_with_Symfony/blob/main/Documentation/img/bearer1.png)

You can manually add the token : 
![](https://github.com/c-lanon-dev/REST_API_with_Symfony/blob/main/Documentation/img/bearer2.png)

You can automatically config the host for all test :

![](https://github.com/c-lanon-dev/REST_API_with_Symfony/blob/main/Documentation/img/config_host.png)

## Other
If you want renew JWT SSL keys :
```Bash
./REST_API_with_Symfony/docker/sbash.sh
cd REST_API_with_Symfony
php bin/console lexik:jwt:generate-keypair --overwrite
```