# Classes 
Pega Platform groups rules into classes according to their capacity for reuse. Each grouping is a *class*. Each application consists of three class types:

1. The **Work** class contains the Rules that describe how to process Cases, such as Processes, data elements, and user interfaces.
2. The **Integration** class contains the Rules that describe how the application interacts with other systems, such as the integration assets that connect the application to an external customer database or a third-party web server.
3. The **Data** class contains the Rules that describe the data types in the application, such as a customer data type or an order items data type.

## Inheritance
Inheritance allows your application to reuse existing Rules for other Cases or applications. Rule reuse through Rule inheritance reduces development and testing time without sacrificing application quality.

Pega provides two mechanisms for rule inheritance: **Pattern and Directed Inheritance**.

### Pattern Inheritance
Pattern inheritance is automatic. Pattern inheritance uses the existing class name structure to determine which Rules are available for reuse. Pattern inheritance searches classes that share a class name prefix. Pattern inheritance promotes reuse based on business suitability because Rules are aggregated at higher levels to reflect their usability throughout an entire division or organization. For example, a Rule applied at the division level that defines elements of payment processing for insurance claims can be reused by each claims department belonging to that division.

### Directed Inheritance
Directed inheritance is inheritance between classes where the parent class is explicitly specified, unlike pattern inheritance, which is automatic. You apply directed inheritance to reuse standard Pega Platform Rules and Rules from other applications outside the business class hierarchy. You list directed inheritance on the class Rule form. Because Rules are aggregated based on whether they apply to all Cases or Cases of a certain type, directed inheritance promotes reuse based on functional suitability.

## Class Hierarchy
To save development time when creating an application, reuse Rules by organizing them into classes, and then creating dependencies between the classes. When you create a class hierarchy you define which classes contain other classes, and as a result, you define how classes reuse or inherit Rules.

In Pega Platform, you can create parent classes that contain child classes. Any Rules available in a parent class are also available to the child classes. Because of this, Pega organizes classes in the following groups:
- *The ultimate base class*, which Pega Platform provides and identifies by the keyword **@baseclass**. The ultimate base class is a root for all other classes.
- *Base classes that store the Rules that provide basic functionality for processing Cases*, such as data elements that record the creator of a Case. The most common base classes include **Work-, Data-, and History- classes**.
- *Classes from other applications*, such as industry-specific Pega applications. For example, you can use a generic application for policy administration as a base for customizing versions for different policy types.
- *Classes that collect Rules and data elements that are common at the division and organization level*, such as a class that stores an approval Process shared across an entire IT department.
- *Classes that describe a specific Case Type*, such as expense reports or vehicle insurance claims.