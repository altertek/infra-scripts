# Altertek infra-scripts
Repository containing various scripts used on Altertek servers

## Requirements (optional)
apt install jq
pip install yq

## backup-docker-psql
In your docker-compose directory:
```
./backup-docker-psql
```
or elsewhere:
```
./backup-docker-psql -c mattermost-app -u postgres_user -n postgres_name
```

## restore-docker-psql
In your docker-compose directory:

```
./restore-docker-psql <postgres_backup_file>
```
or elsewhere:
```
./restore-docker-psql -c mattermost-app -u postgres_user -n postgres_name <postgres_backup_file>
```
