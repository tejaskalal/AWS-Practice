## EC2

EC2 stands for Elastic Compute Cloud, a service provided by Amazon Web Services (AWS).
In simple terms, EC2 lets you rent virtual computers (servers) on the internet so you can run applications, websites, or services without buying physical hardware.

To access server we need to give security with inbound and outbound rules
Inbound = traffic coming into your server
Outbound = traffic going out from your server

Launching server name my-server and number instances is 1 (number ec2 instances you want with same configuration)
<br/><br/>
<img width="1860" height="802" alt="Screenshot 2026-04-26 161349" src="https://github.com/user-attachments/assets/2f7f124d-d1fc-49e4-8096-d483661134b3" />
<br/><br/>
An AMI (Amazon Machine Image) in Amazon Web Services is a pre configured template used to launch EC2 instances. It includes the operating system, required software, and necessary configurations, allowing you to quickly create servers without setting everything up from scratch. In simple terms, an AMI acts like a blueprint of a system, so you can launch multiple identical virtual machines easily and efficiently.
Here we are using ubuntu,
<br/><br/>
<img width="1852" height="834" alt="Screenshot 2026-04-26 161405" src="https://github.com/user-attachments/assets/d0223f03-bf24-432b-8001-b6253adb5921" />
<br/><br/>
An instance type in Amazon Web Services defines the size and power of your EC2 server, including CPU, RAM, and storage. It simply decides how strong or fast your virtual machine will be.And we are creating .pem key , .pem key (Privacy Enhanced Mail key) in Amazon Web Services is a private security file used to securely connect to your EC2 instance
<br/><br/>
<img width="1847" height="835" alt="Screenshot 2026-04-26 161423" src="https://github.com/user-attachments/assets/b33a7caf-23e3-4787-9da3-f7b3c1f9c0fe" />
<br/><br/>
SSH (Secure Shell) is a protocol used to securely connect to and control a remote server over the internet. In Amazon Web Services, it’s commonly used to log into EC2 instances using a .pem key.
<br/><br/>
<img width="1851" height="842" alt="Screenshot 2026-04-26 161442" src="https://github.com/user-attachments/assets/6386dab7-8337-4573-a947-64c06ae145a8" />
<br/><br/>







