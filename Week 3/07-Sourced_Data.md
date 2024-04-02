# Sourced Data in Pega
In Pega, accessing sourced data involves retrieving data from external sources such as databases, APIs, or other systems, and making it available within your Pega application for use in various processes, user interfaces, and reports. 

There are several ways to access sourced data in Pega:

1. **Data Pages**: Data pages are a key mechanism for accessing and managing data in Pega applications. You can configure data pages to retrieve data from external sources, such as databases or REST APIs, and store it temporarily in memory for reuse across multiple parts of your application.

2. **Connectors**: Pega provides connectors for integrating with external systems and services. You can use connectors to establish connections to databases, web services, legacy systems, and other external sources, and retrieve data in real-time as needed.

3. **Integration Services**: Pega offers integration services, such as Connect SQL and Connect REST, which allow you to execute SQL queries against databases or interact with RESTful APIs to retrieve data from external sources. These services provide flexibility and control over the data retrieval process.

4. **Report Definitions**: Report definitions allow you to define queries that retrieve data from various sources, including databases, data pages, and other Pega objects. You can use report definitions to create ad-hoc or scheduled reports that present sourced data in a tabular format.

5. **Data Transformations**: Data transforms can be used to transform and manipulate sourced data retrieved from external sources. You can apply transformations to convert data into different formats, perform calculations, or apply business rules before presenting it to users or storing it in the Pega database.

6. **Custom Code**: In some cases, you may need to write custom code, such as Java or JavaScript, to access sourced data from external sources. Pega provides integration points and extension capabilities to incorporate custom code into your application for accessing data as needed.

7. **Data Propagation**: Once sourced data is retrieved and processed within Pega, you can propagate it to other parts of the application using various mechanisms, such as data pages, clipboard pages, properties, or activities.

When accessing sourced data in Pega, it's important to consider factors such as data security, performance optimization, error handling, and data consistency. By leveraging the appropriate tools and techniques, you can effectively integrate external data sources into your Pega application and provide users with access to relevant and up-to-date information.