# Dispatcher Cart

Dispatcher Cart is a fully open-source eCommerce application that offers a wide range of products, including groceries, electronics, beauty products, fitness items, and much more. The application is designed to be user-friendly, scalable, and robust for online shopping needs.

[![DigitalOcean Referral Badge](https://web-platforms.sfo2.cdn.digitaloceanspaces.com/WWW/Badge%203.svg)](https://www.digitalocean.com/?refcode=a2e2ec1d058e&utm_campaign=Referral_Invite&utm_medium=Referral_Program&utm_source=badge)

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

## 📸 DigitalOcean Screenshots

Below are some screenshots of the **Dispatcher Cart** deployed on a DigitalOcean Droplet:

### 1. Droplet Dashboard
![Droplet Dashboard](assets/do1.png)
![Droplet Dashboard](assets/do2.png)
![Droplet Dashboard](assets/do3.png)
_The dashboard showing the created droplet for hosting Dispatcher Cart._

### 2. Logs for Application Running on Droplet
![App Running](assets/logs.png)  
_Dispatcher Cart running live on the droplet._

### 3. Estimated bill for 1 droplet
![SSH Terminal](assets/estimate_bill.png)  
_The estimated bill on DigitalOcean for the aforementioned configuration_

## 🌟 SignUp with DigitalOcean
Looking for a reliable cloud platform? Sign up for DigitalOcean through my [referral link](https://m.do.co/c/a2e2ec1d058e) and get **$200 in free credit** (valid for 60 days)! 🚀

Why choose DigitalOcean?
- **Affordable Pricing**: Perfect for developers and startups.
- **Easy Setup**: Get your servers running in minutes with an intuitive interface.
- **High Performance**: Reliable and scalable cloud solutions.

Start your cloud journey today and power up your projects with DigitalOcean! 💻

## Profile
- [LinkedIn](https://www.linkedin.com/in/vibhu-26m): Let's connect and network on LinkedIn.

- [GitHub](https://github.com/Joaquin144): Check out my repositories and contributions on GitHub.

- [Gmail](mailto:vvpp98.comco@gmail.com): Mail to me at my gmail id

- [Play Store](https://play.google.com/store/apps/developer?id=DevCommOP): Explore my apps on the Play Store.