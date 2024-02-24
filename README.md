# Portfolio-Project-2
Monitoring the host and application metrics using prometheus and grafana.

***Prometheus***

Prometheus is a time series database used to store and scrape metrics from target endpoints.

***Grafana***

Grafana is a service which is used to visualize the data being scraped by a variety of datasources like prometheus.

***Exporters***

Exporters are agents which are installed on the host machines to collect and expose metrics locally. Prometheus will pull the metrics that are being exposed by the exporters. Eg: Node Exporter.

***Firewall and Security groups***

firewall-cmd command is used to allow incoming requests on system (system here is nothing but the operating system) whereas security groups in ec2 are responsible for managing the incoming and outgoing request on server.

        Step 1: Prometheus using manual
        
        Step 2: Prometheus as a service
        
        Step 3: Node Exporter using manual
        
        Step 4: Node Exporter as a service
        
        Step 5: Adding hosts to prometheus as targets
        
        Step 6: Grafana service
        
        Step 7: Adding prometheus as a datasource


- *In this setup, We have installed Prometheus, Grafana in same server.*  

- *Prometheus by default will collect its own metrics and expose them on http://localhost:9090/metrics. It doesn't require any exporters for exposing its own metrics. But for other metrics we can install exporters like node exporter (Step 1 to 4).*

- *We have added a new host as target by collecting its metrics using node exporter (Step 5: Adding hosts to prometheus as targets)*

- *Then we are installing grafana and configuring it to visualize the data from the datasources like prometheus*

