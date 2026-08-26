# Further Reading - About the Sample Maintenance Backend

The Joule agent you built connects to a sample CAP-based OData v4 service — `MaintenanceOrderService` — via the `sample-maintenance-service` destination. This page explains the data behind it and gives you some prompts to explore further.

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
