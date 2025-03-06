---
description: >-
  Use cases and scenarios describe how a person or system interacts with the
  solution being modelled to achieve a goal.
---

# Use Cases and Scenarios

Use cases and scenarios are essential tools for understanding how users (actors) interact with a system or solution to achieve specific goals. They help define the functional requirements of a system and ensure that the solution aligns with user needs. Below is a detailed breakdown of the **purpose, description, elements, and usage considerations** for use cases and scenarios.

## Tasks to do when creating use cases

* [ ] Identify Actors
* [ ] Identify goal user wants to archive
* [ ] Create use case diagram&#x20;
* [ ] Write use case description
* [ ] Create different scenarios (variations) of use case
* [ ] Validate with stockholders&#x20;





***

#### **Purpose**

Use cases and scenarios are used to:

* Describe how a person or system interacts with a solution to achieve a goal.
* Capture the functional behavior of a system from the user’s perspective.
* Provide a clear understanding of the system’s scope and functionality.

***

#### **Description**

A **use case** describes the interactions between:

* **Primary Actor**: The main user or system initiating the interaction.
* **Solution**: The system or process being modeled.
* **Secondary Actors**: Other users or systems involved in the process.

A use case outlines:

* **Primary Flow**: The most direct path to achieve the goal.
* **Alternative Flows**: Other successful paths to achieve the goal.
* **Exception Flows**: Scenarios where the goal cannot be achieved.

A **scenario** is a specific instance of a use case, describing one way an actor can achieve a goal.

#### **3. Elements of Use Cases**

**3.1 Use Case Diagram**

* A visual representation of the relationships between actors and use cases.
* Uses **Unified Modeling Language (UML)** notation.
* Key components:
  * **Actors**: Represented as stick figures.
  * **Use Cases**: Represented as ovals.
  * **Relationships**: Shown as lines connecting actors to use cases.

**Common Relationships**:

* **Extend**: Adds additional behavior to a use case (e.g., an alternate flow).
* **Include**: Reuses functionality from another use case (e.g., shared logic).

**3.2 Use Case Description**

* **Name**: A unique, descriptive title (e.g., “Place Order”).
* **Goal**: A brief description of the successful outcome (e.g., “Customer places an order successfully”).
* **Actors**:
  * **Primary Actor**: Initiates the use case (e.g., “Customer”).
  * **Secondary Actors**: Support the process (e.g., “Payment Gateway”).
* **Preconditions**: Conditions that must be true before the use case begins (e.g., “Customer is logged in”).
* **Trigger**: The event that initiates the use case (e.g., “Customer clicks ‘Place Order’”).
* **Flow of Events**:
  * **Primary Flow**: The main sequence of steps to achieve the goal.
  * **Alternative Flows**: Other successful paths.
  * **Exception Flows**: Scenarios where the goal fails.
* **Post-conditions**: Conditions that must be true after the use case completes (e.g., “Order is confirmed, and payment is processed”).

***

#### **4. Usage Considerations**

**4.1 Strengths**

* **Clarifies Scope**: Use case diagrams provide a high-level view of the system’s functionality.
* **Easy to Understand**: Narrative-style descriptions are accessible to stakeholders.
* **Focus on Value**: Clearly articulates the business value of each use case.
* **Functional Behavior**: Describes how the system should behave from the user’s perspective.

**4.2 Limitations**

* **Flexibility Can Lead to Overcomplication**: Use cases may include unnecessary details or mix functional and non-functional requirements.
* **Not Suitable for All Requirements**: Decisions, business rules, and UI interactions are better captured using other techniques.
* **No Direct Link to Design**: Use cases do not map to software architecture, requiring additional effort during development.

#### **5. Steps to Create Use Cases and Scenarios**

**Step 1: Identify Actors**

* Determine who or what interacts with the system (e.g., customers, admins, payment gateways).

**Step 2: Define Use Cases**

* For each actor, identify the goals they want to achieve (e.g., “Place Order,” “Cancel Subscription”).

**Step 3: Create Use Case Diagrams**

* Visualize the relationships between actors and use cases.

**Step 4: Write Use Case Descriptions**

* Document the name, goal, actors, preconditions, triggers, flows, and post-conditions for each use case.

**Step 5: Develop Scenarios**

* Create specific instances of use cases to describe different paths (e.g., “Successful Order Placement,” “Order Placement with Payment Failure”).

**Step 6: Validate with Stakeholders**

* Review use cases and scenarios with stakeholders to ensure accuracy and completeness.

**Step 7: Link to Other Artifacts**

* Connect use cases to business rules, UI designs, and non-functional requirements as needed.

***

#### **6. Example: Use Case for an E-Commerce System**

**Use Case Name: Place Order**

* **Goal**: Customer places an order successfully.
* **Primary Actor**: Customer
* **Secondary Actor**: Payment Gateway
* **Preconditions**: Customer is logged in and has items in the cart.
* **Trigger**: Customer clicks “Place Order.”
* **Primary Flow**:
  1. Customer selects “Place Order.”
  2. System displays order summary.
  3. Customer confirms order.
  4. System processes payment via Payment Gateway.
  5. System confirms order and generates an order ID.
* **Alternative Flow**: Payment fails.
  1. System notifies customer of payment failure.
  2. Customer retries payment.
* **Exception Flow**: Insufficient stock.
  1. System notifies customer of out-of-stock items.
  2. Customer removes items or cancels order.
* **Post-conditions**: Order is confirmed, and payment is processed.

***

#### **7. Best Practices**

* **Keep It Simple**: Focus on the user’s perspective and avoid technical jargon.
* **Collaborate with Stakeholders**: Ensure use cases reflect real-world needs.
* **Use Diagrams Sparingly**: Use case diagrams are helpful but not always necessary.
* **Maintain Traceability**: Link use cases to higher-level requirements and test cases.



