# Things Board

ThingsBoard is an open-source IoT platform for data collection,
processing, visualization, and device management.

It enables device connectivity via industry standard IoT protocols
- MQTT, CoAP and HTTP and supports both cloud and on-premises deployments.
ThingsBoard combines scalability, fault-tolerance and performance
so you will never lose your data.

## Get Started

Create data and logs directories:

```console
mkdir -p data && sudo chown -R 799:799 data
mkdir -p logs && sudo chown -R 799:799 logs
```

Running the service:

```console
docker compose up
```

After executing this command you can open http://localhost:8080 in your browser.
You should see ThingsBoard login page.

Use the following default credentials:
- System Administrator: sysadmin@thingsboard.org / sysadmin
- Tenant Administrator: tenant@thingsboard.org / tenant
- Customer User: customer@thingsboard.org / customer

More informations:
https://thingsboard.io/docs/user-guide/install/docker

## API

```console
curl -v -X POST -d "{\"consumed\": 2000}" http://localhost:8080/api/v1/rpu11qy8wiwilax5647p/telemetry --header "Content-Type:application/json"
```
