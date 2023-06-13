<p align="center">
<img src="https://i.imgur.com/zwAH1gk.png" height="40%" width="60%"/>
</p>

<h1>Creating and configuring Azure SQL database</h1>

In this project, I created and deployed an Azure SQL database.<br />


<h2>Environments and Technologies Used</h2>

- Azure SQL Database
- Azure Networking
- Query Editor


<h2>High-Level Steps</h2>

- Create a resource group and then create an Azure SQL Databse within the resource group.
-	Configure a firewall by connecting it to an IP address
-	Adding locks to resourcer group to prevent deletion.





<h3>Step one: provisioning Azure SQL database</h3>
<p>
When creating an Azure SQL database the first thing you want to do is to create a resource group. Putting the database in a resource group makes it easier control access and it keeps everything nice an clean.
<p>
<img src="https://i.imgur.com/zwAH1gk.png" height="70%" width="70%"/>
</p>

<br />

<p>
The first thing I did to create my SQL Platform as a Service Database was clicking “create” and filling out the necessary fields. The fields I filled out were Resource group, database name, and server. I did not have a server so I needed to create a new one. It is important to note when creating a server the name might already be taken so try different combinations if you run into that issue.
</p>
<p>
<img src="https://i.imgur.com/rReYVZ4.png" height="70%" width="70%"/>
<img src="https://i.imgur.com/Gz5sCDU.png" height="70%" width="70%"/>
</p>
<p>
 After filling out the initial information I went into “Compute + storage” and this is where I was able to choose the plan and also the size of the database. After I finished this step it took me back to main page to officially create and provision the database.
</p>
<p>
<img src="https://i.imgur.com/IVEswsJ.png" height="70%" width="70%"/>
<img src="https://i.imgur.com/2DSsdBr.png" height="70%" width="70%"/>
</p>

<br/>
<h3>Step two: setting up Firewall and adding client IP</h3>

<p>
The first thing I did to set up my firewall for the SQL database was by selecting “Networking”, and then I gave my client machine access by clicking “Add your client IPv4 address” and this updated the firewall rules so I could connect to it.</p>
</p>
<br />


<h3>Step three: Connecting to SQL server</h3>
<p>
When connecting to the SQL server there are a couple of ways to do it. I choose to login through the Query editor but I could have also logged in using “SQL Server Management Studio”. </p>

<img src="https://i.imgur.com/QlOBCyM.png" height="70%" width="70%"/>
<img src="https://i.imgur.com/TzG84U2.png" height="70%" width="70%"/>
<br />


<h3>Step four: Adding locks to resource groups</h3>
<p>
I also added a lock to my database to prevent deletion of my database so that other people working in the resource group could not accidentally delete it if they were trying to modify something within the Azure settings.
</p>
<img src="https://i.imgur.com/LjZ8YzN.png" height="70%" width="70%"/>

<br />


