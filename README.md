# Accelerate Web Application Development through Jenkins CI/CD Pipeline triggerred by Github Webhook Integration

This Project has been created to learn to Accelerate Web Application development through Jenkins Pipeline triggered by Github Webhook Integration process.

## Step-1 : Login to your AWS Free Tier Account and Create a Ubuntu Instance.

![image](https://github.com/rahulchauhan7874/Accelerate-Web-Application-Development-through-Jenkins-Pipeline-triggerred-by-Github-Webhook/assets/108551570/18d929e3-2fb3-44bd-a044-fcccd2b86a3d)


## Step-2 : Login to your instance using SSH client (Direct, Putty, MobaxTerm etc)

![image](https://github.com/rahulchauhan7874/Accelerate-Web-Application-Development-through-Jenkins-Pipeline-triggerred-by-Github-Webhook/assets/108551570/99e6c9ca-6693-4193-8429-0ab0217c34b9)

- Update your Ubuntu Instance

```Bash
sudo apt-get update -y
```

![image](https://github.com/rahulchauhan7874/Accelerate-Web-Application-Development-through-Jenkins-Pipeline-triggerred-by-Github-Webhook/assets/108551570/40af6492-f588-43ae-bedc-1db488cec43f)


## Step-3 : Install Java on your AWS EC2 Ubuntu Instance

- Jenkins has been created in Java that's why we require Java Runtime Environment (JRE) to run Jenkins on the Ubuntu Server.
- Install Openjdk11 -

```Bash
sudo apt install openjdk-11-jre -y
```

![image](https://github.com/rahulchauhan7874/Accelerate-Web-Application-Development-through-Jenkins-Pipeline-triggerred-by-Github-Webhook/assets/108551570/c7c823c5-0b0b-4c8b-bfaa-2bd1e8915657)


## Step-4 : Now Install Jenkins on your Ubuntu Instance

- Start by importing the GPG key. The GPG key verifies package integrity but there is no output.

```bash
curl -fsSL https://pkg.jenkins.io/debian/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
```

- Add the Jenkins software repository to the source list and provide the authentication key:

```Bash
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
```

- Update the system repository

```bash
sudo apt-get update -y
```

- Now install Jenkins

```bash
sudo apt-get install jenkins -y
```

![image](https://github.com/rahulchauhan7874/Accelerate-Web-Application-Development-through-Jenkins-Pipeline-triggerred-by-Github-Webhook/assets/108551570/b9e62319-17b7-49b1-ae77-ee0205b68046)
