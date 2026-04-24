## Load Balancer

A load balancer is a system that sits between users and servers and distributes incoming requests across multiple servers. We use it to avoid overloading a single server, improve performance, and ensure high availability so even if one server fails, others can still handle the traffic. It helps applications run smoothly under heavy load and provides a better, faster experience for users.

---

Create two ec2 instances for this load balancer practice.
<br/><br/>
<img width="1845" height="841" alt="Screenshot 2026-04-24 220257" src="https://github.com/user-attachments/assets/b1962a6a-830f-471a-a6b6-12b1bb03ffc0" />
<br/><br/>
We allow SSH to securely access and manage the server remotely (for setup, configuration, and maintenance), and HTTP to let users access the website or application through their browsers.
<br/><br/>
<img width="1843" height="843" alt="Screenshot 2026-04-24 220346" src="https://github.com/user-attachments/assets/01b39423-a5e1-4a1e-9a84-aacbe212cb61" />
<br/><br/>
Installed Apache2 on server-1 and Nginx on server-2
<br/><br/>
<img width="1835" height="783" alt="Screenshot 2026-04-24 220808" src="https://github.com/user-attachments/assets/f4a0f6b2-b7f9-44a1-b63b-828d582217bf" />
<br/><br/>
<img width="1831" height="812" alt="Screenshot 2026-04-24 221212" src="https://github.com/user-attachments/assets/50f79b8f-bda3-49de-9d9c-d049af7827ff" />
<br/><br/>
Let's check Apache2 and Nginx before creating load balancer , are they accessible from browser
<br/><br/>
<img width="1854" height="992" alt="Screenshot 2026-04-24 221812" src="https://github.com/user-attachments/assets/28fbe3da-89bc-4cbc-bd05-91bdf101e9c1" />
<br/><br/>
<img width="1850" height="1001" alt="Screenshot 2026-04-24 221801" src="https://github.com/user-attachments/assets/8a68b47b-a94a-47d6-8822-2346d4792ccb" />





