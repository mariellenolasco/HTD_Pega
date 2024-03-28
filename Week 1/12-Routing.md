# Routing in Pega
In Pega, routing assignments to users involves the process of assigning work items, tasks, or cases to specific users or groups based on predefined criteria, rules, or conditions. Assignments ensure that work is distributed effectively, efficiently, and in accordance with business requirements. Here's how routing assignments to users is typically accomplished in Pega:

1. **Assignment Shape in Processes**:
   - Within process flows, assignment shapes are used to define tasks or work items that need to be completed by users.
   - Developers configure assignment shapes within the process flow to specify the assignment type, assignment details, and routing logic.
   - Assignment shapes allow developers to define criteria for selecting the assignee, such as roles, skills, availability, workload, or predefined routing rules.

2. **Routing Logic**:
   - Routing logic determines how assignments are routed to users or groups based on predefined rules, conditions, or criteria.
   - Developers can configure routing logic using various mechanisms, such as:
     - **Assignment Policies**: Define policies or rules that specify how assignments should be routed based on criteria such as user availability, skills, workload, or priority.
     - **Routing Directives**: Define directives or instructions within the assignment shape to determine the assignee based on predefined conditions or rules.
     - **Assignment Algorithms**: Implement custom algorithms or decision logic to dynamically determine the best assignee based on real-time data, context, or business rules.

3. **Assignment Types**:
   - Pega supports different types of assignments, including:
     - **Fixed Assignment**: Assign work items to specific users or groups based on predefined assignments.
     - **Dynamic Assignment**: Dynamically route work items to users or groups based on runtime conditions, rules, or criteria.
     - **Round Robin Assignment**: Distribute work items evenly among a group of users or teams using a round-robin algorithm.
     - **Load Balancing Assignment**: Balance workload across multiple users or groups based on factors such as capacity, availability, or workload.
     - **Escalation Assignment**: Automatically reassign work items to different users or groups if certain conditions are met, such as exceeding SLA deadlines or thresholds.

4. **Assignment Worklists**:
   - Assigned work items appear in users' worklists or work queues, allowing them to view, prioritize, and act on assigned tasks.
   - Worklists provide users with a centralized view of their pending assignments, along with relevant details, deadlines, and action options.
   - Users can access their worklists from the Pega portal or through email notifications, mobile applications, or other channels.

5. **Assignment Management**:
   - Pega provides tools and interfaces for managing assignments, including reassignment, delegation, escalation, and prioritization of work items.
   - Users and managers can perform actions such as reassigning tasks, escalating issues, delegating work to other users, or prioritizing assignments based on business needs.

By effectively routing assignments to users in Pega, organizations can ensure that work is distributed efficiently, tasks are completed in a timely manner, and business processes operate smoothly and effectively.