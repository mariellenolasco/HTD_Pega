# Data Transforms
In Pega, data transforms are used to transform and manipulate data within the context of a case or a flow. They are commonly used to map data from one format to another, apply business rules or calculations, and prepare data for presentation or processing.

**Purpose**

Data transforms serve the purpose of transforming data from one format to another. This can include copying data from one property to another, applying calculations or formulas, performing conditional logic, and formatting data for display or integration with external systems.

**Types of Data Transforms**:
   - **Activity-based Data Transforms**: These data transforms are executed as part of an activity rule and are often used to perform complex data transformations or business logic.
   - **Flow Action-based Data Transforms**: These data transforms are associated with flow actions and are executed when a user interacts with a screen to update data.
   - **Utility-based Data Transforms**: These data transforms are standalone and can be called from other rules or components within the application to perform specific data transformations.

**Mapping and Manipulating Properties**

Data transforms allow you to map values from one property to another, set property values based on conditions, concatenate strings, format dates, perform mathematical calculations, and more.

**Contextual Execution**

Data transforms execute within the context of a specific case or flow. This means they have access to the properties and data associated with that context, allowing for targeted data transformations.

**Reusability**

Data transforms can be reused across multiple rules and components within the application. This promotes consistency and reduces redundancy in data transformation logic.

**Integration with Other Rules**

Data transforms can be integrated with other rules in Pega, such as activities, decision rules, and UI rules. This allows for seamless data transformation across different parts of the application.

**Error Handling**

Data transforms can include error handling logic to handle exceptional scenarios or data validation errors. This ensures that data is transformed accurately and reliably.

**Performance Considerations**

While data transforms provide flexibility and ease of use, it's important to consider performance implications, especially when dealing with large datasets or complex transformations. Optimizing data transforms can help improve application performance.

Overall, data transforms are a powerful feature in Pega that enable developers to manipulate and transform data effectively within their applications. They play a crucial role in data integration, business logic implementation, and user interface customization.