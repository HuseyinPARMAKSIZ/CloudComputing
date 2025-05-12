📊 CMS Monitoring Stack with Prometheus & Grafana

This project sets up a complete monitoring environment using Docker Compose, including Joomla CMS instances with both MySQL and PostgreSQL support, Prometheus for metric collection, Grafana for visualization, and related exporters.

🧱 Stack Components

    Joomla: Two separate CMS instances
        One with MySQL
        One with PostgreSQL

    MySQL & PostgreSQL: Database services

    Prometheus: Metrics collection

    Grafana: Metrics visualization

    mysqld_exporter & postgres_exporter: Exporters for database metrics

    node_exportor : for OS (operating system) metrics

🚀 Getting Started

sudo apt install docker.io

sudo curl -L "https://github.com/docker/compose/releases/download/v2.36.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

sudo docker-compose version

Docker Compose version v2.36.0


Clone the repository:

git clone https://github.com/HuseyinPARMAKSIZ/CloudComputing.git

cd CloudComputing

Start the services:

sudo docker-compose up -d

durdur - docker-compose down
ağları uçur - docker network prune
Her servisin Dockerfile’ına göre imajını yeniden oluşturur - docker-compose up --build
arka planda (detached mode) başlat -  "-d" 


🌐 Access Web Interfaces

    Joomla (MySQL): http://localhost:8081
    Joomla (PostgreSQL): http://localhost:8082
    Prometheus: http://localhost:9090
    Grafana: http://localhost:3000

📊 Grafana Dashboard

You can visualize MySQL and PostgreSQL metrics directly in Grafana. Default credentials:

    Username: admin
    Password: admin
