# Simple Java 3-Tier Application with Docker Compose
Welcome to the Simple Java 3-Tier Application Docker Compose project! This project aims to provide a seamless deployment of a Java application using a 3-Tier architecture, orchestrated with Docker Compose.

## Components
Nginx (Port 80): The powerful web server Nginx will be used to render the frontend on port 80.

Tomcat with WebApp (Port 8080): Apache Tomcat will host our Java web application, making it accessible on port 8080.

MySQL Database (Port 3306): The MySQL image will be used to store and manage the application's data on port 3306.

## Getting Started

Prerequisites

Before you begin, ensure that you have Docker and Docker Compose installed on your system.

Copy code

git clone https://github.com/yourusername/simple-java-docker-compose.git

Navigate to the project directory:

cd simple-java-docker-compose

Run the Docker Compose command to start the 3-Tier application:

docker-compose up -d

The -d flag runs the containers in the background.

### Access the application:

Frontend (Nginx): http://localhost

Java Web Application (Tomcat): http://localhost:8080

MySQL Database: Use your preferred MySQL client, connecting to localhost:3306

## Customization

Feel free to customize the project to suit your needs. You can modify the Java web application, tweak Nginx configurations, or adjust the MySQL settings in the docker-compose.yml file.

## Troubleshooting

If you encounter any issues during setup, refer to the troubleshooting section in the Wiki.

## Contributing
We welcome contributions! If you find any bugs or have suggestions for improvements, please open an issue or submit a pull request.

