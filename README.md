## Docker Assignment - Agile Software Practice.

__Name:__ Ursula Tamen

__Demo:__ [.... Link to YouTube demonstration ....](https://youtu.be/PC193c774ps)

This repository contains the containerization of the mukti-container application illustrated below.

![](./images/arch.png)

### Database Seeding.

Not done. But had intended to include it as a seeding service with a script. And assign it a develoment profile variable only. It would have been in the api-network.

### Multi-Stack.

To support buiding development and production stack options I set the profiles variable of the different services. All but mongo-express had both production and development profiles hence will be deployes in both environments, while mongo-express only had a development profile so it would not be deployed in a production environment. The command used to build the containerized application is docker-compose --profile <environment> up -d. For example: docker-compose --profile production  up -d, wont deply the express container.
