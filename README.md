## AWS EC2 Instance

- Go to AWS Console
- Select ubuntu Operating system
- Instances(running)
- Launch instances
  
![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/bbbe3cdd-8c50-4071-9a65-c5df2354998c)

### Grafana-installation Step by step:

## Step 1: First we need to go to the Grafana official website.

#### Website link: https://grafana.com/grafana/download/

# Change Enterprise to OSS( open source) 

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/d248c79c-f9de-48d7-a640-831eccc46084)

### Run the below commands to install Grafana and start their services. Ubuntu(64 Bit):

```
sudo apt-get install -y adduser libfontconfig1
```

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/2ab8b80a-5a9a-4d8f-a6fe-85e50e88a892)

```
wget https://dl.grafana.com/oss/release/grafana_10.0.1_amd64.deb
```

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/a30fd40d-2a56-4ee1-8329-3efa75e9a45b)

```
sudo dpkg -i grafana_10.0.1_amd64.deb
```

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/70d6a4ef-d2ff-4abc-8509-2f21c306434f)

Please execute to enable the grafana services

```
sudo /bin/systemctl enable grafana-server
```
### You can start grafana-server by executing below command
```
sudo /bin/systemctl start grafana-server
```
### You can check the status of grafana-server by executing below command
```
sudo /bin/systemctl status grafana-server
```

##### Output:
 ![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/8b5bd0c5-b2be-4c3b-b2d4-be79ddda9772)


##### Now you need to go to your brower and paste the public IP address of your server eg: http://52.15.56.112:3000/

##### Grafana runs on 3000 ports.

If port is not enable then you need to enable that port: 3000 on your aws security group:

# Steps: 

###### First go to your instance> click on there> go to security> click on security group> click on edit inbound rule>add rule>save rule

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/f15b42e1-5b1e-4a34-9e6f-ffd63b271f78)


![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/0893d932-86a7-4d81-8d7e-7ac61d4ac428)


![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/91fb59e4-4b4d-45d0-9173-217c5910dee9)


![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/3e20fa37-e170-40f7-a414-b37e7c30fa55)

# Now save the rule:

##### Once you are done with the above steps, then paste the given url with your IP: eg: http://PublicIP:3000/


![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/1b04f715-02ec-48ba-9e31-070d105ddda1)


## This is the Login page of your Grafana.

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/ff2d898f-2a76-4709-b898-0dbfe5cbd61b)


### By default:
```
Username: admin
Password: admin

```

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/b1c96f95-1c95-43de-aa1e-15b3e7867229)


###### If you want to change your password then you can change, I am not going to change this: Skip for now.

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/199615cf-aaed-4734-9ecb-b7938d8807dc)


### So finally we have successfully installed Grafana on our machine, this is our Grafana Home Page:

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/3e0cf806-65ae-41e8-8921-977545bde31a)


'''
Remember, practice makes perfect 🎯 Don't forget to work on personal projects and contribute to open-source projects on platforms like GitHub. Building a portfolio will showcase your skills and help you stand out to potential employers.

Networking is key! ✨ Join DevOps communities, attend conferences, and engage with professionals in the field. LinkedIn is a great platform to connect and learn from industry experts.
Stay curious and keep learning 📖
'''

##### Good luck on your DevOps journey. Feel free to reach out if you have any questions or need further guidance. Together, let's accelerate your career in DevOps 💪
## LinkedIn: https://www.linkedin.com/in/ritikktiwari/

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/dbd3cb71-3d98-47c3-95c2-43c231b2e300)

