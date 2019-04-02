# coin_and_purse_app
This repo defines the coin and purse app level stuff.
The app is structured as a set of services deployed in
Docker containers. To run in a local environment, use
the `docker-compose` command in the same level as the
_docker-compose.yml_ file to start the app services.
The _docker-compose.yml_ file assumes that all the
images to be run have already been built, so prior to running
make sure the images are available on your local machine.

* The _docker-compose.yml_ file uses docker-compose file
format 3.7 which requires Docker Engine release 18.06.0+.

* The development notes and other [docs](https://drive.google.com/drive/u/1/folders/1xLJENx7cN4cYqaxV8rvz1g9m78HyrzCj).

## docker-compose Commands
From the directory containing the _docker-compose.yml_ file:

### Launch app
```Bash
docker-compose up -d
```

### Stop app
```Bash
docker-compose stop
```

### Clean up app containers
```Bash
docker-compose rm
```

### Complete app uninstall
```Bash
docker-compose down
```

## App Service Repos
* [ledgerapi](https://github.com/Drewan-Tech/coin_and_purse_ledger_service/tree/v0.1.0_int_branch)
* [ledgerdb](https://github.com/Drewan-Tech/coin_and_purse_ledger_db/tree/v0.1.0_int_branch)
* [browserclient](https://github.com/Drewan-Tech/coin_and_purse_browser_client/tree/v0.1.0_int_branch)
* [gateway](https://github.com/Drewan-Tech/coin_and_purse_gateway/tree/v0.1.0_int_branch)

## Versions

| Version | Comment|
| ---:|:---|
| 0.1.0 | Basic app structure. Ability to post and get transactions from ledger service. Browser client able to post transactions to ledger service and get list of transactions. |
