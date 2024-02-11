```
                          _             _        _          _             
  ___ __ _ _ __ ___   ___| | ___     __| | ___  | |__  _ __(_) __ _  __ _ 
 / __/ _` | '_ ` _ \ / _ \ |/ _ \   / _` |/ _ \ | '_ \| '__| |/ _` |/ _` |
| (_| (_| | | | | | |  __/ | (_) | | (_| |  __/ | |_) | |  | | (_| | (_| |
 \___\__,_|_| |_| |_|\___|_|\___/   \__,_|\___| |_.__/|_|  |_|\__, |\__,_|
                                                              |___/       
```

Uma versão Bash da rinha do backend 2ª edição 2024/Q1

## Agradecimentos

Boa parte dos insights quanto a nginx e docker foram tirados do repo incrivel do [@leandronsp](https://github.com/leandronsp).

O repo de onde me baseei para essa app foi a versão em bash que ele fez pra rinha [https://github.com/leandronsp/canabrava]

## Requisitos

- [Docker](https://docs.docker.com/get-docker/)
- [Gatling](https://gatling.io/open-source/)

## Stack

- 2 OCaml apps
- 1 PostgreSQL
- 1 NGINX

## Usage

```sh
$ make
Usage: make [36m<target>[0m
  [36mhelp                     [0m  Prints available commands
  [36mstart.dev                [0m  Start the rinha in Dev
  [36mdocker.stats             [0m  Show docker stats
  [36mhealth.check             [0m  Check the stack is healthy
  [36mstress.it                [0m  Run stress tests
```

## Inicializando a aplicação

```sh
$ make start.dev
```

Testando a app:

```sh
$ make health.check
```

Teste de stress com gatling:

```sh
$ make stress.it
```
