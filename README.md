# mysql_cloudmanaged_databases

## 1. MySQL Setup on Azure and GCP

### GCP: 

### Azure: 
1. Sign into Microscoft Azure https://azure.microsoft.com/en-us with your email.
2. Once logged in, in the search bar at the top of the page, type `Azure Database for MySQL`. Before you hit enter, it will populate a few options under the search bar. Find the 'Marketplace' section, and click `Azure Database for MySQL`.
3. The site will bring you to a page called `Select Azure Database for MySQL deployment option`. Click `create` under the `Flexible server`.
4. It will bring you under the `Basics` tab, for "Subscription" ensure it says `Azure for Students`, and for the "Resource group" hit `Create new`, and type what you'd like related to the project. For instance, I named mine "amna-504-wk4".
5. Next to `Server name`, name the server something related to what you will be working on. For instance, I anmed mine "hha504-wk4"
6. Ensure the `Wordkload type` is `For development or hobby projects' and the `Compute + storage` section looks like this: ![image](https://github.com/amnasyed1/mysql_cloudmanaged_databases/assets/123895397/85d92fd9-9ff1-41f0-8e48-7b5b37e72dda)
7. Then set up the `server admin login name` and `password`.
8. Now navigating to the `Networking` tab, next to "Basics", ensure the `Connectivity method` is `Public access (allowed IP addresses) and Private endpoint`.
9. Under `Firewall rules`, check the box that states `Allow all public access from any Azure Service within Azure to this server` and click `+ Add 0.0.0.0 -255.255.255.255`. After these steps are completed, it should look like this: ![image](https://github.com/amnasyed1/mysql_cloudmanaged_databases/assets/123895397/134c2f7e-eec0-441f-bd88-0e363fe44ed7)
Lastly, at the bottom of the page hit `Review & Create`. Check if all the details presented are correct and then hit `Create`. 
