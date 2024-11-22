# Dispatcher Cart

Dispatcher Cart is a fully open-source eCommerce application that offers a wide range of products, including groceries, electronics, beauty products, fitness items, and much more. The application is designed to be user-friendly, scalable, and robust for online shopping needs.

---

## 🚀 Features

- ✅ **Wide Product Range**: Shop for groceries, electronics, beauty, fitness, and more in one app.
- ✅ **Open Source**: Completely free to use, modify, and contribute to.
- ✅ **Cloud Deployment**: Hosted on [DigitalOcean](https://www.digitalocean.com/) for high availability and scalability.
- ✅ **Modern UI/UX**: Clean and intuitive interface for seamless navigation and shopping experience.
- ✅ **Secure Checkout**: Safeguards user data with secure payment options.

---

## 🛠️ Tech Stack

- **Backend**: Spring Boot (Java 17)
- **Frontend**: Thymeleaf + HTML/CSS
- **Database**: MySQL
- **Deployment**: DigitalOcean Droplet
- **Build Tool**: Maven

---

## 🌐 Live Demo

Check out the live application here: [Dispatcher Cart Live](http://159.223.88.90:8080/)  
*(Ubuntu 24.10 x64 | 1GB Memory | 10GB Disk | SGP1)*

---

## 📥 Installation

### Prerequisites
- Java 17+
- Maven or Gradle
- MySQL or PostgreSQL
- DigitalOcean Droplet (optional for deployment)

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/Joaquin144/DispatcherCart.git
   cd dispatcher-cart
   
2. Configure the database:
   - Update the application.properties file in the src/main/resources directory with your database credentials.
   ```bash
    spring.datasource.url=jdbc:mysql://localhost:8080/dispatcher_cart
    spring.datasource.username=your-username
    spring.datasource.password=your-password
    ```

3. Build the project:
    ```bash
   mvn clean install
   
4. Run the application:
   ```bash
   java -jar target/dispatcher-cart-0.0.1-SNAPSHOT.jar

5. Access the application: Open your browser and visit http://localhost:8080.


### 📦 Deployment (DigitalOcean)

1. Setup a DigitalOcean droplet. Min requirements: 1vCPU, 1GB Memory, 10 GB Disk, Cost around USD 6$ per month).

2. Transfer the .jar file from local machine to server
    ```bash
   scp target/dispatcher-cart-0.0.1-SNAPSHOT.jar your-user@your-droplet-ip:/path/to/deployment

3. SSH login into the server:
   ```bash
   ssh droplet-user@your-droplet-ip

4. Run the application
   ```bash
   java -jar /path/to/deployment/dispatcher-cart-0.0.1-SNAPSHOT.jar
   
5. Alternatively, if you want to run the server permanently then you might want to create a start.sh bash script.
    ```bash
   #!/bin/bash

    nohup java -jar /projects/dispatcher-cart-0.0.1-SNAPSHOT.jar --spring.profiles.active=prod > /projects/log.txt 2>&1 &

    echo $! > /projects/pid.file
    ```
   
    - Use command to start service which won't be terminated when you close the SSH session.
   ```bash
   sudo ./start.sh


## Profile
- [LinkedIn](https://www.linkedin.com/in/vibhu-26m): Let's connect and network on LinkedIn.

- [GitHub](https://github.com/Joaquin144): Check out my repositories and contributions on GitHub.

- [Play Store](https://play.google.com/store/apps/developer?id=DevCommOP): Explore my apps on the Play Store.