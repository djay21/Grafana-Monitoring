# Grafana-Monitoring


Grafana is a multi-platform open source analytics and interactive visualization web application. It provides charts, graphs, and alerts for the web when connected to supported data sources. It is expandable through a plug-in system. End users can create complex monitoring dashboards using interactive query builders.
You can add & manage multiple data sources ( Elastic search, Azure metrics etc ) for single grafana server.

This repo includes:-
1. how to install grafana,
2. Setting prometheus,cadvisor, & node exporter on the target machine through <i>docker-compose and promethues.yml</i> file , &
3. Adding prometheus as a datasource to grafana server.
4. A customised dasboard which is developed only to monitor docker containers and basic system details, like cpu load, memory, space left etc. 

 To integrate this dashboard into your grafana server, <br>
 Go to Dashboards >> Manage dashboards >> import from panel json && paste this dashboad.json and then save it. 
 
 A screenshot is attached below for reference.


** Also you can reset grafana credentials with the command given below.

<b>grafana-cli --config "/etc/configuration/" admin reset-admin-password mynewpassword <b>

** Also you can integrate email, teams, slack and much more alerts with grafana so if anything goes unexpectedly up, it will alert on your respective integrated channel.
<br>



![Dashboard](https://github.com/djay21/Grafana-Monitoring/blob/master/grafana.png)

![Dashboard](https://github.com/djay21/Grafana-Monitoring/blob/master/grafana-2.png)

