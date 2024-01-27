# Workspace

## Running Airflow in Docker

Before we run Airflow, let's create these folders below first. Please note that if you're using Windows, you can skip this step.

```sh
mkdir -p mnt/dags mnt/logs mnt/plugins mnt/tests #1.รันใน terminial ก่อน
```

On **Linux**, please make sure to configure the Airflow user for the docker-compose:

```sh
echo -e "AIRFLOW_UID=$(id -u)" > .env #2.รันใน terminial ก่อน
```

```sh
docker compose build
docker compose up
```

To stop Airflow, run:

```bash
docker compose down
```