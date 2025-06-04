# How Nodes Work in n8n

In n8n, nodes are the fundamental building blocks of workflows. Each node performs a specific task, such as fetching data, processing it, or sending it to another service. Nodes can be combined to create complex automation workflows.

## Types of Nodes

n8n categorizes nodes based on their functionality:

### 1. Trigger Nodes

Trigger nodes initiate workflows in response to specific events or conditions. They listen for events from external services or internal schedules.

Examples:
- **Webhook Trigger:** Starts a workflow when an HTTP request is received.
- **Cron Trigger:** Initiates workflows based on a time schedule.

### 2. Action Nodes

Action nodes perform tasks within a workflow, such as manipulating data or interacting with external services.

Examples:
- **HTTP Request:** Sends HTTP requests to external APIs.
- **Set:** Sets static or dynamic values to be used later in the workflow.

### 3. Core Nodes

Core nodes provide essential functionalities that are not specific to any external service. They help in controlling the flow and processing of data within workflows.

Examples:
- **IF:** Implements conditional logic to determine the workflow path.
- **Merge:** Combines data from multiple branches.

### 4. Community Nodes

Community nodes are contributed by the n8n community and extend the platform's capabilities by integrating with additional services.

## Node Operations

Each node offers specific operations that define what the node can do. For instance, an HTTP Request node can perform GET, POST, PUT, DELETE operations, among others.

When adding a node:
- **Select the desired operation** from the available options.
- **Configure the necessary parameters** required for that operation.

## Adding Nodes to a Workflow

To add a node:
1. Click on the "+" icon on the workflow canvas.
2. Search for the desired node by name or functionality.
3. Click on the node to add it to the canvas.
4. Connect it to other nodes to define the workflow sequence.

## Node Parameters and Configuration

Each node has parameters that need to be configured:
- **Credentials:** Authentication details for external services.
- **Input Fields:** Data required for the node to perform its operation.
- **Options:** Additional settings that modify the node's behavior.

Proper configuration ensures that the node performs its intended function within the workflow.

## Executing and Testing Nodes

n8n allows for testing individual nodes:
- **Execute Node:** Runs the selected node to test its functionality.
- **View Output:** Examine the output data to ensure correctness.

Testing nodes individually helps in debugging and validating parts of the workflow before full execution.

---

For more detailed information, refer to the [official n8n documentation on nodes](https://docs.n8n.io/workflows/components/nodes/).
