# E-mail com workers

Esse projeto é um sender de e-mails em python, postgres, redis e worker em Docker.

## Getting Started

Basta instalar o docker em seu OS, executar `docker-compose up -d`

Escalonar o Worker `docker-compose up -d --scale worker=3` o número de scales correspondente fica a seu critério.

Ver os logs `docker-compose logs -f -t`

Ver os logs com escalonamento `docker-compose logs -f -t worker`

Select `docker-compose exec db psql -U postgres -d email_sender -c 'select * from emails'`

