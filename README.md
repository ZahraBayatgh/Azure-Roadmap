# Azure Roadmap
<b>Design a complicated web system with  Azure.</b>
## Give a Star! :star:
If you like this project, learn something or you are using it in your applications, please give it a star. Thanks!

# Azure Roadmap
Welcome to the Git repo that is associated with the Azure roadmap
**[Azure Roadmap](https://github.com/ZahraBayatgh/Azure-Roadmap/blob/master/Azure_Roadmap_90_Resolution.jpg)**
published by [LinkedIn](https://www.linkedin.com/in/zahrabayat/).
This image is Design a complicated web system with Azure.

| Azure Roadmap |
| ------------|
|<sup> <img src="https://github.com/ZahraBayatgh/Azure-Roadmap/blob/main/Azure-Roadmap.png?raw=true" alt="Azure_Roadmap_90_Resolution.jpg"></sup>|

# Customers 

We have<b> customers </b>for our application that using various types of devices.
 
 <b>The customers :</b>
 
     1) Could be humans using web browsers.
     2) Could be other computers using web services.
     
# Azure Active Directory B2C
  In both cases, the traffic still flows over secure HTTP, and  we could use <b>Active Directory B2C</b> to <b>authenticate users</b> and<b> grant tokens</b> for service calls.
  
 # Azure Web Service
   We can deploy our application or APIs to  an <b>app service</b>. 
   
   If we want to stick with an app service approach, then two resources that we could use would be: 
   
     1) Azure WebJobs 
     2) Azure Functions

## Azure Function and Azure Web Job 
 <b>Both</b> of these <b>technologies</b> allow me to execute code when a message appears in a <b>queue</b>.
 
 # Azure Queue
 Now most systems that really need to scale and stay available, need to use some asynchronous processing. 
 So we need to set up an <b>Azure storage account</b> and make use of message queues.
 
 <b>Queues</b> are useful because they allow me to disconnect the application from some of the back-end processing that needs to take place.
 We often refer to this use of queues as load leveling, because we level the load and amortize the request over a slightly longer period of time.
 
 # Azure Blob Storage
  When we deploy our application, we can push our static content into <b>Blob storage</b> and then a server that contents through an Azure  content delivery network, a <b>CDN</b>.
  
 ## Azure CDN
  The <b>CDN</b> is good for serving content, static content like  images and movies, and even script and CSS files to serve that content as fast as possible.
  
  <b>But why use a content delivery network?</b>
  
  Well, if you want a fast, scalable website, a CDN can help reduce the page load time for your customers because content served from a CDN is probably closer to the user
  than the content in your app service, and therefore, the content arrives quicker.
  
 # Azure App Insights
 <b>Application insights</b> are also a resource that you'll want to include in any non-trivial web application. 
 Application insights can tell me where my application is slow, it can help me track down errors.
 
 It's a vital source of information about the behavior and the well-being of the system. You can also integrate application insights data into your application because application insights offer an API.
 
 So you might have a page that administrators can log into and view information about the recent errors and exceptions in the application, and they can do that without 
 leaving the application and going to the Application Insights portal because you can make all the information available right in the application itself.
 
 # Azure Key Vault
  Another resource that you should consider using is <b>Azure Key Vault</b>. Key Vault is designed to protect secrets, secrets as access keys, passwords,and certificates. 
  You definzitely do not want these secrets in your source code, and there's a good argument to be made that you don't want to copy these secrets around in the<b> Azure portal</b>
  either as an app setting. 

With Key Vault, you can set up things so only your system administrators need to know the secrets and they can import those access keys and passwords into <b>Azure Key Vault</b>.
Key Vault will store those secrets securely, even using hardware security modules and the administrator can provide URLs for an application to interact with the keys and 
monitor logs to see who is using those keys.

# Azure Redis
If we're building a <b>scalable</b> application, we will probably use some caching. 
<b>Azure Redis Cache</b> is one<b> distributed cache</b> that we can use.a distributed cache like Redis can give  you quick access to data from all the services and instances
running in your application.

You can scale up your app servicewith new instances and not need to worry about those instances having to warm up by populating a cache, and since Azure manages
Redis as a service, as a platform, you can have 10s of gigabytes of cache available with guaranteed uptimes and a disaster recovery plan. 

## Azure SQL and Azure Cosmos DB
 With <b>Redis</b>, you might cache query results from <b>Cosmos DB </b>or <b>Azure SQL</b>. 
  
 Not only will the cached results typically be faster to receive, but you'll also be reducing the load on your databases when the application is under stress. 
 
## Azure Search
For some applications, you might want to give your users the ability to search for data that is somewhere in the application. For this job, you might rely on <b>Azure Search</b>. 
Azure Search provides indexers that will crawl the data in Cosmos DB and Azure SQL and blob storage as well as other data sources, and then give you full-text
search and language processing, including support for faceted navigation, Lucene query syntax, search suggestions, scoring, and all of this across 56 different languages.
