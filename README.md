## AWS EC2 Instance

- Go to AWS Console
- Select ubuntu Operating system
- Instances(running)
- Launch instances
  
![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/bbbe3cdd-8c50-4071-9a65-c5df2354998c)

### Grafana-installation

Step 1: First we need to come on official website of Grafana.
#### Website link: https://grafana.com/grafana/download?edition=oss

# Change Enterprise to OSS( open source) 

#### FIG: 1

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/d248c79c-f9de-48d7-a640-831eccc46084)

### Run the below commands to install Grafana and start their services. Ubuntu(64 Bit):

```
sudo apt-get install -y adduser libfontconfig1
```

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/2ab8b80a-5a9a-4d8f-a6fe-85e50e88a892)

wget https://dl.grafana.com/oss/release/grafana_10.0.1_amd64.deb

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/a30fd40d-2a56-4ee1-8329-3efa75e9a45b)

sudo dpkg -i grafana_10.0.1_amd64.deb

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/70d6a4ef-d2ff-4abc-8509-2f21c306434f)

Please execute to enable the grafana services

sudo /bin/systemctl enable grafana-server
### You can start grafana-server by executing
 sudo /bin/systemctl start grafana-server
 ### You can start grafana-server status by executing
 sudo /bin/systemctl status grafana-server
Output:
 ![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/8b5bd0c5-b2be-4c3b-b2d4-be79ddda9772)

____________

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/b6056800-00af-4b1f-8eee-ad403703f9de)


################

Now you need to go to your brower and paste the public IP address of your server eg: http://52.15.56.112:3000/

Grafana runs on 3000 ports.

if that is not enable then you need to enable on your aws console:

1st go to your instance> click on there> go to security> click on security group> click on edit inbound rule>add rule>

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/f15b42e1-5b1e-4a34-9e6f-ffd63b271f78)


![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/0893d932-86a7-4d81-8d7e-7ac61d4ac428)

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/91fb59e4-4b4d-45d0-9173-217c5910dee9)

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/3e20fa37-e170-40f7-a414-b37e7c30fa55)

# Now save the rule:

Now paste the given url: eg: http://52.15.56.112:3000/
![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/1b04f715-02ec-48ba-9e31-070d105ddda1)

This is the Login page of your Grafana.

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/ff2d898f-2a76-4709-b898-0dbfe5cbd61b)

By default:
Username: admin
Password: admin

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/b1c96f95-1c95-43de-aa1e-15b3e7867229)

If you want to change your password then you can change, I am not going to change this: Skip for now.

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/199615cf-aaed-4734-9ecb-b7938d8807dc)

So finally this is your Grafana Home Page:

![image](https://github.com/RitikPyCode/Grafana-installation/assets/69500530/3e0cf806-65ae-41e8-8921-977545bde31a)








