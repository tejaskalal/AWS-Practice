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
<br/><br/>
We created a target group in Amazon Web Services to group and manage our backend servers (EC2 instances) that will receive traffic from the load balancer. It is used so the load balancer knows where to send requests and can perform health checks to ensure traffic is only routed to healthy servers. This helps improve availability, reliability, and proper traffic distribution in the system.
<br/><br/>
<img width="1845" height="829" alt="Screenshot 2026-04-24 223706" src="https://github.com/user-attachments/assets/e7fa8530-b665-4f4c-97b2-d70ad881dbfa" />
<br/><br/>
We created an Application Load Balancer in Amazon Web Services to distribute incoming HTTP/HTTPS traffic across multiple servers based on request details like URL or path. It helps ensure high availability, better performance, and fault tolerance by routing traffic only to healthy instances in the target group, making the application more scalable and reliable.
<br/><br/>
<img width="1851" height="841" alt="Screenshot 2026-04-24 224114" src="https://github.com/user-attachments/assets/1145a799-1ed5-4c15-b1ce-29a55be4b86b" />
<br/><br/>
The result for both servers shows that the Application Load Balancer in Amazon Web Services is successfully distributing traffic between them. When users access the application, requests are routed to different servers (like Nginx and Apache), and both respond correctly. This confirms that the setup is working properly, providing load distribution, high availability, and better performance.
<br/><br/>
<img width="1849" height="840" alt="Screenshot 2026-04-24 225134" src="https://github.com/user-attachments/assets/77520231-8d45-4d74-9cfb-e7c719c49c35" />
<br/><br/>
<img width="1858" height="969" alt="Screenshot 2026-04-24 225323" src="https://github.com/user-attachments/assets/943611df-8f94-425f-8e09-2d87b5ab208a" />










