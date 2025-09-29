# Automate-Multi-Tier-Java-Web-Application-on-Premises-Using-Scripts-
Automated Multi-Tier Java Web Application Deployment. This project uses reusable shell scripts to provision and configure a complete multi-tier environment on local infrastructure. It sets up essential components including a database server (MySQL), application server (Tomcat), web server (Nginx), and optional caching layer, ensuring faster, consistent, and error-free deployments while demonstrating practical DevOps automation practices.

<img width="1051" height="610" alt="image" src="https://github.com/user-attachments/assets/35c699be-45b3-4ab0-b1f8-db14b3b3e592" />


# What tools will we use in the project?

# Prerequisite
1. Oracle VM Virtualbox
2. Vagrant                                                                                                
3. Vagrant plugins

# PROVISIONING
Services
1. Nginx => Web Service
2. Tomcat => Application Server                                                                            

3. RabbitMQ => Broker/Queuing Agent
4. Memcache => DB Caching
5. ElasticSearch => Indexing/Search service
6. MySQL => SQL Database
7. # Project Steps

# 1:Create shell script (Backend vms ) 
 Create a ShellScript file for Database we will call mariadb.sh  We will write the following in the file 
 
<img width="1918" height="992" alt="image" src="https://github.com/user-attachments/assets/4a67d12f-11b5-4940-ba54-239da8d4cb9e" />

 
# 2 Create a ShellScript file for Memcached we will call memcashed.sh  We will write the following in the file 
 

 <img width="1913" height="992" alt="image" src="https://github.com/user-attachments/assets/ff909eca-fde3-448b-8dec-66eb13940103" />



# 3 Create a ShellScript file for RabbitMQ  we will call rabbitmq.sh  We will write the following in the file 


<img width="1918" height="1000" alt="image" src="https://github.com/user-attachments/assets/fe3f9750-7562-47a3-84dd-d972a087941e" />


# 4 Create a ShellScript file for APP in clude ( tomcat , nginx )

<img width="1918" height="980" alt="image" src="https://github.com/user-attachments/assets/9ba9a920-089a-4e24-bccc-f82143df35fe" />


<img width="1918" height="1001" alt="image" src="https://github.com/user-attachments/assets/16c51ee3-3249-4130-9399-5ec0e55ff34c" />


# After writing the scripts
 we will write a vagrantfile, which should be like this, and we will put in it all the VM that we will create, and we will also make a private network and connect the VM to each other and introduce the

 <img width="1903" height="995" alt="image" src="https://github.com/user-attachments/assets/df80c5b6-d3bb-4863-8622-73ca4062e3fd" />

  
 <img width="1918" height="995" alt="image" src="https://github.com/user-attachments/assets/beb689da-d39c-4f51-8369-1bf89c3ece29" />

# After End write ip to connect 

<img width="1003" height="529" alt="image" src="https://github.com/user-attachments/assets/0fb53ac1-5637-43bd-a8ef-05096e9527fd" />

What we learn from Scripts ?

Improve your automation skills
Working with shell scripts enhances your ability to automate repetitive tasks. You learn how to write commands that configure services like Tomcat, MySQL, and Nginx without manual steps.

Save time and effort
Instead of setting up each service manually, scripts allow you to deploy and configure the entire environment in seconds, saving hours of work.

Reduce errors
Automation with scripts ensures consistency — every time you run the script, it performs the exact same steps, reducing mistakes caused by manual configuration.

Reusable and shareable solutions
Scripts can be reused across multiple projects or shared with team members, making collaboration easier and avoiding "works on my machine" issues.

Boost productivity
With automation, you spend less time on setup and more time on actual development and problem-solving.

<img width="1200" height="552" alt="image" src="https://github.com/user-attachments/assets/3d436440-db06-48a3-ac2e-cb245beebec7" />


