# Project 1: Technical Brief
## Description: Developed a personal Cyber-Security focused blog and answered questions regarding networking, web development, cryptography and cloud services.




### General Questions

##### What option did you select for your domain (Azure free domain,  GoDaddy domain)?

GoDaddy 


##### What is your domain name?

joeyssecurityblogs


Networking Questions

##### What is the IP address of your webpage?

20.119.0.18


##### What is the location (city, state, country) of your IP address?

East US 


##### Run a DNS lookup on your website. What does the NS record show?

Server:         168.63.129.16
Address:        168.63.129.16#53




### Web Development Questions

##### When creating your web app, you selected a runtime stack.  What was it? Does it work on the front end or the back end? 

Runtime Stack was PHP 8.0. 


##### Inside the /var/www/html directory, there was another directory called assets. Explain what was inside that directory.

Seems to be all the coding for html 


##### Consider your response to the above question. Does this work with the front end or back end?

Back end 





### Cloud Questions

##### What is a cloud tenant?

a consumer who purchases cloud computing resources


##### Why would an access policy be important on a key vault?

Because it can determine whether a security principal can perform different operations on secrets, keys and certificates.


##### Within the key vault, what are the differences between keys, secrets, and certificates?

Keys enables the use of software. Secrets provide secure storage for passwords and database connection strings. Certificates are built on top of the keys and secrets and add an automated renewal feature.


### Cryptography Questions

##### What are the advantages of a self-signed certificate?

Some advantages are that they are free and easy to use. Good for testing environments and internal network websites and they are simple to modify or customize. 


 ##### What are the disadvantages of a self-signed certificate?

Some disadvantages would be that, for one, is that browsers don’t trust them so you will always have the “not secure” prompt which can affect the volume of traffic to the website. Also, users can become more vulnerable to data theft when attackers create self-signed certificates that can be used in MITM attacks.  


##### What is a wildcard certificate?

Is a public key cert that can be used with multiple sub-domains pertaining to the same base domain.


##### When binding a certificate to your website, Azure only provides TLS versions 1.0, 1.1, and 1.2.  Explain why SSL 3.0 isn’t provided.

This was to ensure user safety. It had to many vulnerabilities which was affecting the users. 

##### Is your browser returning an error for your SSL certificate? Why or why not?

Yes, it tells be it is not secure, and this is because I have an Self-Signed certificate which by browser does not trust.  

##### What is the validity of your certificate (date range)?

Tues. December 27, 2022 to Friday, December 22, 2023.

##### Do you have an intermediate certificate? If so, what is it?

Yes, it is  *.azurewebsites.net

##### Do you have a root certificate? If so, what is it?

Yes, it is Microsoft Azure TLS Issuing CA 05 

##### Does your browser have the root certificate in its root store?

yes


##### List one other root CA in your browser’s root store.

AAA Certificate Service 


### Cloud Security Questions 

##### What are the similarities and differences between Azure Web Application Gateway and Azure Front Door?

They are both layer 7 load balancers but front door is a non-regional service whereas gateway is a regional service. 


##### A feature of the Web Application Gateway and Front Door is “SSL Offloading.” What is SSL offloading? What are its benefits?

SSl Offloading handles the encryption/decryption process on a separate device so that it does not affect the web servers performance. The benefits, well that it brings smooth loading of the website and faster processing of requests at the end of the web application. 


##### What OSI layer does a WAF work on?

Layer 7 - application layer 


##### Select one of the WAF managed rules (e.g., directory traversal, SQL injection, etc.), and define it.

SQL is a web security vulnerability that allows attackers to interfere w/ the queries that an application makes to its database. Basically allows and attacker to view data they are not normally able to see. 


##### Consider the rule that you selected. Could your website (as it is currently designed) be impacted by this vulnerability if Front Door wasn’t enabled? Why or why not?




##### Hypothetically, say that you create a custom WAF rule to block all traffic from Canada. Does that mean that anyone who resides in Canada would not be able to access your website? Why or why not? 

I would say that if their IP address was from Canada then yes it would block the traffic but they could use a VPN and still access.

