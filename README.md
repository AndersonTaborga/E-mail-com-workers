# E-mail com workers

Esse projeto é sender de e-mails em python, postgres, redis e worker em Docker.

## Getting Started

Basta instalar o docker em seu OS, executar `docker-compose up -d`

Escalonar o Worker `docker-compose up -d --scale worker=3` o número de scales correspondente fica a seu critério.

Ver os logs `docker-compose logs -f -t`

Ver os logs com escalonamento `docker-compose logs -f -t worker`

Select `docker-compose exec db psql -U postgres -d email_sender -c 'select * from emails'`

### Prerequisites

While we’ll define concepts along the way, it is good for you to understand what Docker is and why you would use Docker before we begin.

We also need to assume you are familiar with a few concepts before we continue:

IP Addresses and Ports
Virtual Machines
Editing configuration files
Basic familiarity with the ideas of code dependencies and building
Machine resource usage terms, like CPU percentages, RAM use in bytes, etc.




