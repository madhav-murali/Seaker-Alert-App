# Seaker-Alert-App: System Monitoring Dashboard


Welcome to the Seaker-Alert-App, a real-time system monitoring solution. This project uses a professional-grade stack of  Prometheus, Grafana, and Docker to collect, store, and visualize system metrics like CPU, RAM, and Disk usage from the host machine.

The entire application is containerized, allowing for a simple, one-command setup.

The current version is setup to monitor from the local device , but promethues node-exporter can be installed via ssh in any supported iot devices to access their data.

## Local Setup Instructions (2 Minutes)
To run this project on your local machine, please follow these steps.

Prerequisites
Docker and Docker Compose (Docker desktop is what i am using.)

Running the Application
Clone the Repository:

    git clone [Your GitHub Repository Link]
    cd Seaker-Alert-App

Start the Services:
Run the following single command from the Seaker-Alert-App directory. This will download the necessary images and start the Grafana, Prometheus, and Node Exporter services.

docker-compose up -d

## Accessing and Using the Dashboard
Open the Dashboard:
Navigate to http://localhost:3000 in your web browser.

Login Credentials:

    Username: admin
    Password: admin
(You can skip the prompt to change the password.)

View Metrics:
The "System Monitoring" dashboard will be available on the home page. Click it to see live and historical data for your machine.

## How to Test the Alerting System
You can easily simulate and test an alert.

Edit a Panel: On the dashboard, find the "CPU Usage" panel, click its title, and select Edit.

Configure Alert:

Go to the Alert tab.

Set the Threshold to a low value, like 10. This means an alert will trigger if CPU usage is above 10%.

Save and Observe: Click Save and then Apply. The panel on the dashboard will quickly turn red and show a "Firing" state, demonstrating that the alert mechanism is working.


# Thank you for taking the time to review my project.