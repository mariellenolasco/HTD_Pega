# Conditional Execution
Conditional execution in Pega refers to the ability to control the flow of a process or decision logic based on specified conditions or criteria. It allows users to define rules that determine whether certain actions or steps should be executed within a workflow or business process. Conditional execution enables dynamic and flexible behavior in Pega applications, allowing processes to adapt to changing conditions or inputs.

Here's how conditional execution works in Pega:

1. **Conditions**: Users can define conditions using Pega's built-in expression language or decision rules. Conditions typically involve comparing data values, properties, or variables against predefined criteria, such as equality, inequality, or range checks.

2. **Decision Points**: Conditional execution is often used at decision points within a process flow, where the workflow branches based on the evaluation of specific conditions. For example, a decision point may determine whether to approve a request based on the value of certain properties or attributes associated with the request.

3. **Routing Logic**: Conditional execution can also be used to control the routing of work items or cases within a Pega application. For example, based on the outcome of a condition evaluation, a work item may be routed to different queues, teams, or individuals for further processing.

4. **Automation**: Conditional execution can trigger automated actions or tasks within a process flow based on the satisfaction of specified conditions. For example, if a condition is met, the system may automatically send notifications, update data values, or initiate additional subprocesses.

5. **Dynamic Behavior**: Conditional execution allows processes to exhibit dynamic behavior, where the sequence of steps or actions can vary depending on the context or input data. This enables Pega applications to respond intelligently to changes in the environment or user interactions.

6. **Integration with Decision Strategies**: In more advanced scenarios, conditional execution in Pega can be integrated with decision strategies or predictive analytics to optimize decision-making based on historical data and contextual information.

Overall, conditional execution in Pega provides a powerful mechanism for implementing complex business logic, decision-making, and process automation within Pega applications. By defining conditions and rules that govern the execution of actions, organizations can create adaptive and efficient workflows that meet their specific business requirements.

## Skipping a stage or process
The typical path of events in a Case Life Cycle never skips a Stage and always begins a Process. With conditional execution, it is possible to deviate from this normal path. The system runs or skips Stages and Processes if the run-time values of the Case match the conditional logic defined on the entry.

