# Further Reading - About the Sample Maintenance Backend

The Joule agent you built connects to a sample CAP-based OData v4 service — `MaintenanceOrderService` — via the `sample-maintenance-service` destination. This page explains the data behind it, introduces the persona who would use it, and gives you some prompts to explore further.

---

## Who Uses This Agent?

**Persona: Maintenance Planner**

A maintenance planner is responsible for scheduling and coordinating maintenance work orders across a plant or facility. Before dispatching a work team, they need to confirm that all required materials and spare parts are available in sufficient quantities. Traditionally, this involves manually cross-referencing the work order, its operations, the required components, and current stock levels across warehouses — a time-consuming process prone to errors.

With the Joule agent, a maintenance planner can simply ask in natural language:

> *"Can Maintenance Order 1 be fulfilled based on current stock?"*

The agent walks the full data chain — order → operations → components → stock levels — and responds with a clear fulfillment assessment and recommendations, saving the planner significant time and reducing the risk of dispatching a team for a job that cannot be completed due to missing parts.

---

## Data Model

The service exposes five related entities:

![data model](../images/data_model.png)

| Entity | What it represents |
|--------|--------------------|
| **MaintenanceOrder** | A work order to maintain equipment - has a status, scheduled dates, and a work center |
| **Operation** | A step within a maintenance order - describes what work needs to be done and how long it takes |
| **Component** | A material item required to carry out an operation, with a required quantity |
| **Material** | A spare part or consumable — identified by a material code and description |
| **StockLevel** | The available quantity of a material in a specific warehouse and plant center |

**How they connect:** An order contains operations → each operation needs components (materials) → each material has stock levels across warehouses. The agent walks this chain to check if everything needed is available before the order starts.

---

## Full Dataset

To explore the complete data and verify the agent's responses, download the Excel file below. It contains one sheet per entity with all records from the backend service.

📥 [Download maintenance_backend_data.xlsx](maintenance_backend_data.xlsx)

The file contains:
- **50 Maintenance Orders** (statuses: OPEN, IN PROGRESS, COMPLETE)
- **87 Operations** across all orders
- **110 Components** linking operations to materials
- **60 Materials** (spare parts and consumables)
- **100 Stock Level** records across warehouses M001 and M002

---

## Sample Prompts

Once your agent is set up, try these in the test chat to explore the data:

**Basic fulfillment check:**
> Can Maintenance Order 1 be fulfilled based on current stock?

**Order details with operations:**
> What operations are planned for order 1, and do we have all the required materials in stock?

**Stock shortage focus:**
> Which materials for order 1 are below the required quantity? What should we do about it?

**Multi-order comparison:**
> Compare orders 1 and 2 — which one is more likely to proceed without delays?

**What-if scenario:**
> If warehouse WH-01 is unavailable, can order 1 still be fulfilled from other locations?

**Proactive planning:**
> List all components for order 1 and their current stock levels across all warehouses.

---

**Back to - [Home Page](../README.md)**
