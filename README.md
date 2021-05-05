# docker-compose influxDBv2 with telegraf

can be used for docker swarm

## Telegraf configuration

Telegraf configured by **telegraf.conf**. Need to add `[[inputs.points]]`, and, if then need, change  `[[outputs.points]]`.  
*In example, standard metrics for Docker are used.*

## InfluxDB configuration

InfluxDB configured by **.env** file.

## To add boards, tasks, alerts, etc. like configs

Add config in `*.yml` or `*.json` to mounted folder `influx_config`. After starting, they will be applied.  
*In example, standard dashboard for Docker are used.*

## or

U can add they manually.

## Start by docker-compose

```docker-compose up -d```

## Start by docker swarm

```docker stack deploy -f docker-compose.yml StackName```

## License

This project is licensed under the Beer-ware license revision 42.
