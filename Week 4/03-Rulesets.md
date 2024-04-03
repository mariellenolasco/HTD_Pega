# Rulesets
A ruleset is a logical container or grouping mechanism used to organize and manage related rule instances within a Pega application. Rulesets provide a structured way to package and deploy rules, making it easier to manage and maintain the application's configuration and customization.
## Ruleset Versioning
Ruleset versioning in Pega refers to the process of managing different versions of rulesets and rule instances within a Pega application. It allows developers to track changes to rules over time, control the deployment of rule changes across different environments, and maintain the integrity and consistency of the application's configuration. 

**Version Numbers**:
   - Each ruleset in Pega is assigned a version number, which uniquely identifies a specific version of the ruleset.
   - Version numbers typically consist of three parts: major version, minor version, and patch version (e.g., 01-01-01).
   - The major version indicates significant changes or enhancements to the ruleset, the minor version indicates minor updates or improvements, and the patch version indicates bug fixes or patches.

**Rule Instance Versioning**:
   - Rule instances within a ruleset are also versioned, allowing developers to track changes to individual rules over time.
   - When a rule instance is modified, a new version of the rule instance is created, preserving the previous versions for reference and rollback purposes.
   - Version history for rule instances includes details such as the date of modification, the user who made the change, and a description of the changes made.

### Benefits of Versioning

**Deployment and Promotion**:
   - Ruleset versioning enables controlled deployment and promotion of rule changes across different environments, such as development, testing, and production.
   - Developers can promote ruleset versions from one environment to another using deployment tools provided by Pega, ensuring that changes are applied consistently and accurately across environments.

**Dependencies and Rollback**:
   - Ruleset versioning allows developers to define dependencies between rulesets, ensuring that dependent rulesets are deployed along with the main application ruleset.
   - In case of issues or errors with a ruleset deployment, developers can rollback to a previous version of the ruleset or rule instance, reverting the changes and restoring the application to a previous state.

**Governance and Compliance**:
   - Ruleset versioning helps enforce governance and compliance requirements by providing an audit trail of changes to rules over time.
   - Version history and change logs for rulesets and rule instances can be used for regulatory compliance, auditing, and troubleshooting purposes.

Overall, ruleset versioning in Pega enables developers to manage changes to rules effectively, control deployments across environments, and maintain the integrity and consistency of the application's configuration over time. It is a critical aspect of Pega application development and deployment processes, ensuring that applications remain stable, reliable, and compliant with business requirements.

## Ruleset Stack
In Pega, a ruleset stack refers to the ordered list of rulesets that are considered by the system when resolving rule conflicts or determining which version of a rule to use at runtime. The ruleset stack defines the hierarchy of rulesets within a Pega application and specifies the order in which rule instances are searched for and evaluated.

**Hierarchy**:
   - Ruleset stacks are hierarchical in nature, with rulesets organized in a top-down order based on their precedence.
   - The ruleset stack typically starts with the highest-level ruleset containing the application's core rules, followed by progressively more specific rulesets that contain customizations or overrides.

**Precedence**:
   - Rulesets higher in the stack have higher precedence, meaning that their rule instances are considered first during rule resolution.
   - If a rule instance is found in a higher-priority ruleset, it is used instead of a rule instance with the same name and type in a lower-priority ruleset.

**Rule Resolution**:
   - When a rule is referenced or invoked within a Pega application, the system searches for the rule instance in the ruleset stack based on its name, type, and other criteria.
   - The system starts searching from the top of the ruleset stack and progresses downwards until it finds a matching rule instance or reaches the end of the stack.
   - If multiple matching rule instances are found in different rulesets within the stack, the system uses the one with the highest precedence, as determined by its position in the stack.

**Customization and Overrides**:
   - Ruleset stacks allow for customization and overrides of standard or base rules provided by Pega.
   - Developers can create rule instances in lower-priority rulesets to override or customize the behavior of rule instances defined in higher-priority rulesets.
   - This flexibility enables developers to tailor the application's behavior to specific requirements without modifying the core rules provided by Pega.

**Versioning**:
   - Ruleset stacks can include multiple versions of rulesets, allowing for controlled deployment and promotion of rule changes across environments.
   - Developers can manage dependencies and conflicts between different versions of rulesets within the stack, ensuring consistency and integrity of the application's configuration.
