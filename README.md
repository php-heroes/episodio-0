# PHP Hero - Episodio 0

PHP Hero e' una iniziativa benefica per coinvolgere piu' persone all'uso del PHP.

Per qualsiasi informazione, contattatemi scrivendo una email a `alessandro.lanni@gmail.com`.

## In questo Episodio

Nota! Gli argomenti saranno approfonditi nel corso della diretta.

### Docker come companion per lo sviluppo

- Concettti di base su Docker
    - Home page del progetto: https://www.docker.com/why-docker
    - Images
    - Containers
    - Uso del Docker Compose

- Perche' Docker e' utile a noi sviluppatori

- Installazione Docker Engine Community su Ubuntu
    - Guida online: https://docs.docker.com/install/linux/docker-ce/ubuntu/

- Rifinire l'installazione
    - Guida online: https://docs.docker.com/install/linux/linux-postinstall/

- Come controllare che il demone sia operativo
    -  `$ sudo systemctl status docker`

- Avviare helloworld
    - `$ docker run hello-world`

- Installare docker-compose
    - `$ sudo apt install  docker-compose`


### Costruiamo il nostro ambiente di sviluppo PHP

- Struttura del progetto

- Dockerfile
    - Installazione pacchetti apt
    - Installazione extensions php

- File docker-compose.yml
    - Servizi
    - Porte esposte
    - Volumi

- Comandi piu' usati per interagire con Docker
    - Build delle immagini: `$ docker-compose build`
    - Avvio del progetto: `$ docker-compose ps`
    - Stop del progetto: `$ docker-compose stop`

- Test del progetto mediante browser
    - http://localhost:8080/

- Test del progetto mediante php-cli
    - Verifica della versione dele PHP: `$ docker-compose exec episodio0 php --version`
    - Esecuzione script: `$ docker-compose exec episodio0 php public/index.php`

### Configruazione della IDE

- Aprire il progetto in Visual Studio Code

- Installare le Extensions:
    - Docker - Gestione integrata del demone Docker
    - PHP Extension Pack
