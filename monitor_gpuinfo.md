# Monitor GPU info on Multiple Server Nodes
With this tutorial, you can monitor multiple gpus' info on different nodes with `telegraf` + `Grafana` + `InfluxDB`. 
<img width="1802" alt="WechatIMG20" src="https://user-images.githubusercontent.com/70961580/196877990-add79d88-ba44-47c1-8c37-61747f3ef12f.png">

In order to monitor multiple nodes, you need to first setup a master node which host the database `InfluxDB` and Dashboard web service `Grafana`.

## Setup master node
Install `telegraf` + `Grafana` + `InfluxDB` on your chosen master node, this node can be any node of you servers.
Follow this [link](https://docs.urduheim.de/ubuntu-tutorials/how-to-install-grafana-influxdb-and-telegraf-on-ubuntu-20.04-lts)

## Setup Client node
Follow this [link](https://docs.urduheim.de/ubuntu-tutorials/how-to-monitor-multiple-servers-with-grafana-on-a-single-dashboard)
