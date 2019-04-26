# Migrating your database to Azure

![Moving a database is a little like moving puppies...](https://media.giphy.com/media/RIZ0uSqLiLx3Um0QDC/giphy.gif)

From November 2018 to May 2019, my team has been preparing and presenting sessions at [Microsoft Ignite | The Tour](http://gslb.ch/d345b) all over the world. This series of articles is a write-up of the session MIG20 titled "[Migrating your database to Azure](http://gslb.ch/d346b)".

This session was also recorded in Amsterdam and you can find the recording embedded at the end of this page.

# It's a great time to move to Azure

![Great time to move to Azure](https://i.imgur.com/f1GfgE8.png)

We have more services and features than ever before, and this makes it a great time to move to Azure. On one hand we have [SQL databases that are more compatible](http://gslb.ch/d296b) with older on-premise databases, with more features. We also support [multiple models and APIs with CosmosDB](http://gslb.ch/d7b). But also we have [new ways to perform migration](http://gslb.ch/d347b), either using the traditional tools that you know and love, but also we now have managed services that can help you do the migration in an easy manner and with minimum downtime. We will talk about all these services in this series of articles.

# Why move?

There are usually a number of reasons why one wants to move data to the cloud in general, and to Azure in particular.

![Reasons to move to Azure](https://media.giphy.com/media/clop0So4y9OnuAyLAK/giphy.gif)

- Maybe your datacenter contracts expire and you need to ask yourself if you want to just continue like before, or find a new modern solution for your data.

- Maybe you acquired a firm, or you have been acquired, and you are faced with a hybrid data architecture where multiple operating systems, platforms and database systems are involved. On Azure, you can easily migrate these hybrid systems to the cloud, and use messaging services to make these diverse systems work together. 

> It's also interesting to note that Azure works great with on-premise systems, and it is very common in fact that some people prefer to have some of their data on their own data servers, and other data in Azure.

- Maybe your business is booming and you need some capacity fast (RAM, CPUs, bandwidth, storage...). On the other hand, maybe this peak demand won't last forever and then you also want to scale down, so that you don't waste money on unused resources.

- You want to always be up to date with the latest software and hardware. If something breaks and your data is on Azure, we will fix it for you. Since your data is replicated on multiple servers and possibly in multiple regions as well (depending on your setup), we can failover to another set of synchronized data somewhere else, while our engineers fix the problem. For software, when you use platform-as-a-service (PaaS) such as [Azure SQL Database](http://gslb.ch/d349b), [Cosmos DB](http://gslb.ch/d7b) or [storage accounts](http://gslb.ch/d348b), we always provide the latest patches to you automatically, for example to prevent hacking or other issues.

- Azure is very secure by default. Data is [always encrypted when it rests](http://gslb.ch/d350b) on our servers, using our own symetrical encryption keys. Of course you can also use your own keys if you prefer. During transport data is also encrypted, for example using SSL, TLS, VPN, Express Route or other protocols depending on your use case. 

- As for the physical security, Azure data centers are extremely secure too, and most of the time no one can be found on the floor. Entrance control is very strict and guarantees that there are no "surprises" like someone breaking in your firm's data center and stealing servers (and the data on it).

- Compliance is very important to us and to you, and Azure is compliant with every major organization.

- With our new application development platforms, such as [Serverless Functions](http://gslb.ch/d10b), [App Services](http://gslb.ch/d205b), [Cognitive Services](http://gslb.ch/d117b) and more, it is possible to develop innovative solutions for your users, leveraging the data that you acquired over the years and using brand new development platforms to create new experiences.

- Software end of support means that some older platforms won't be supported anymore soon, for example [Windows Server 2008 | R2](http://gslb.ch/d351b) and [SQL Server 2008 | R2](http://gslb.ch/d352b) are approaching end of support.

All these reasons mean that its probably a good time to ask yourself about your data strategy, and to think about moving to a moder global platform such as Azure.

# A choice of tools

![A choice of tools](https://i.imgur.com/JJR7m5t.png)

Azure and Microsoft have a number of native tools that you can of course use with your cloud data. For example we will talk about the assessment phase, during which you make sure that your data is going to fit well on our cloud platform.

In this series of articles, we will introduce the [Data Migration Assistant](http://gslb.ch/d318b) which can be used before the migration even starts, to make sure that you won't encounter issues when you are ready to press the "migrate" button. Stay tuned for more information and a demo.

In general though, you always want to get started at [the Azure Migration Center](http://azure.com/migrate).

For the migration itself, we also have a number of tools, for example [the Azure Site Recovery](TODO) which allows for a backup-and-restore migration. But if you prefer a managed service, we also have [the Database Migration Service (DMS)](TODO) which we will talk about and demo further in this article series. This service is brand new and allows for a migration with minimum downtime (meaning that you can perform the migration without shutting down your websites or applications).

For optimization, the [Azure Cost Management center](TODO) is where you want to go. This is the place where you can see what your services cost, and we will offer suggestions on how to optimize your spending, for example by scaling down to a server with less cores, or using less RAM, etc.

Finally it is worth noting that if you have tools that you prefer, we are integrating many of our partners' solutions into the Azure portal directly. Gradually you will find more of these tools, and will be able to use them easily to manage and use your Azure data.

# Innovative migration solutions

![Azure Data Box](https://i.imgur.com/soIvS8e.png)

Sometimes when you want to migrate large quantities of data, you might not want to use the Internet. Either you don't trust it with confidential data, or it is going to take a long time to copy tera- or petabytes on a slaow connection. [One innovative solution to this problem is Azure Data Box](TODO). You can select the size that you need, and we will ship you one of these boxes. You can then copy your data to it at your convenience. Once done, we will ship the Data Box back to our data center and our engineers will copy the data to your database. 

Another way to use Azure Data Box is to order one of [our Gateway options](TODO). On these data boxes, you can even run some of Azure's services, [using Azure Stack](TODO). This is a way to get started with Azure services on your own premises, with a super easy migration path later on if so desired.

# Next steps

Now that we saw why and how you can migrate your database to Azure, we will take a look at the problem we are trying to solve and get acquainted [with Tailwind Traders legacy architecture](./migrating-your-data-to-azure-2.md).

# The video

If you prefer you can also watch the video of this session which was recorded in Amsterdam on March 21st. This video [is also available on the Microsoft Ignite | The Tour site](http://gslb.ch/d346b).

[TODO EMBED VIDEO 6qS4XxycEbM]