# Wait Step
In Pega, the "Wait" step is a component of the business process automation functionality within the Pega Platform. It allows you to pause the execution of a case or flow for a specified period of time or until a certain condition is met. The Wait step is useful for scenarios where you need to introduce a delay in the processing of a case or to synchronize with external events.

**Configuring the Wait Step** 

In the Pega Designer Studio, you can add a Wait step to a flow rule within your application. You specify the duration of the wait (in seconds, minutes, hours, etc.) or define a condition that must be met before the flow can proceed.

**Types of Waits**

1. **Duration-Based Wait**: If you choose to specify a duration for the wait, the flow will pause execution for the specified period of time before continuing to the next step in the flow.

2. **Condition-Based Wait**: Alternatively, you can configure the Wait step to wait until a certain condition evaluates to true. This condition could be based on the values of properties, the status of other cases, or any other criteria relevant to your business process. The flow will remain paused until the condition is met.

**Usage Scenarios**

The Wait step can be used in various scenarios within a business process. For example, you might use it to introduce a delay between steps in a process, to wait for external systems to complete a task, or to wait for user input or approval.

**Error Handling**

It's important to consider error handling when using the Wait step. For instance, you may need to account for scenarios where the wait duration exceeds a certain threshold or where the condition never evaluates to true. Pega provides mechanisms for handling such situations, such as setting timeouts or defining fallback actions.

**Summary**
Overall, the Wait step in Pega adds flexibility to your business processes by allowing you to introduce pauses or delays based on time or conditions, enabling you to create more robust and responsive process flows within your Pega applications.