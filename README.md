# Requirement Analysis in Software Development Lifecycle (SDLC)

## What is Requirement Analysis?
Requirement Analysis is the process of identifying, gathering, analyzing, and documenting the functional and non-functional requirements of a software system. It serves as the foundation for software development, ensuring that the final product meets the needs and expectations of stakeholders such as clients, users, and business managers.

In simpler terms, it is about answering **"What should the software do?"** before figuring out **"How should the software be built?"**.

---

## Importance of Requirement Analysis in SDLC

Requirement Analysis is one of the most crucial phases of the Software Development Lifecycle (SDLC). Its importance lies in the following aspects:

1. **Clarity and Understanding**
   - It ensures that developers, testers, and stakeholders share a common understanding of the project goals.
   - Prevents misunderstandings and conflicting expectations.

2. **Scope Definition**
   - Clearly defines the scope of the project by distinguishing between what will be included and excluded.
   - Helps avoid scope creep (uncontrolled changes or continuous growth in a project’s scope).

3. **Improved Project Planning**
   - Accurate requirements allow project managers to estimate cost, effort, and time more effectively.
   - Serves as a basis for creating realistic schedules and resource allocation.

4. **Quality Assurance**
   - Well-defined requirements act as a benchmark for testing.
   - Ensures the final product aligns with user needs and business objectives.

5. **Cost and Risk Reduction**
   - Detecting issues or gaps in the requirement phase is significantly cheaper than fixing them during later stages like coding or testing.
   - Reduces the risk of project failure due to unclear or misunderstood requirements.

6. **Stakeholder Satisfaction**
   - Ensures that the software delivers value to end-users and aligns with business objectives.
   - Builds trust between stakeholders and the development team.

---

## Key Activities in Requirement Analysis

1. **Requirement Elicitation**
   - Gathering requirements from stakeholders using techniques such as interviews, questionnaires, brainstorming, workshops, and observation.

2. **Requirement Classification**
   - Categorizing requirements into:
     - **Functional requirements**: Define what the system should do.
     - **Non-functional requirements**: Define system qualities like performance, security, usability, and scalability.

3. **Requirement Modeling**
   - Representing requirements visually using:
     - Use Case Diagrams  
     - Data Flow Diagrams (DFD)  
     - Entity-Relationship Diagrams (ERD)  

4. **Requirement Documentation**
   - Creating a **Software Requirement Specification (SRS)** document that serves as an official reference for development and testing.

5. **Requirement Validation**
   - Ensuring the requirements are complete, consistent, feasible, testable, and aligned with stakeholder needs.

6. **Requirement Management**
   - Handling changes in requirements throughout the SDLC.
   - Maintaining traceability to ensure all requirements are implemented.

---

## Common Challenges in Requirement Analysis

- Ambiguous or incomplete requirements.
- Conflicting stakeholder interests.
- Communication gaps between technical and non-technical stakeholders.
- Changing business needs over time.
- Lack of user involvement during the requirement phase.

---

## Conclusion

Requirement Analysis is the **cornerstone of successful software development**. A project with poorly defined requirements is at high risk of delays, cost overruns, or complete failure. By investing time and effort in proper requirement analysis, teams can ensure better planning, reduced risks, higher quality software, and greater stakeholder satisfaction.

In short:
- **Good requirements = Successful project.**
- **Poor requirements = Costly failures.**

## Why is Requirement Analysis Important?

Requirement Analysis plays a vital role in the **Software Development Lifecycle (SDLC)** because it ensures the success of a project from the very beginning. Below are three key reasons why it is critical:

### 1. Clarity and Shared Understanding
Requirement Analysis provides a clear and unambiguous understanding of what the system should do.  
- It aligns stakeholders, developers, and testers around the same goals.  
- Prevents miscommunication and misunderstandings that can lead to incorrect features or missing functionality.  

### 2. Accurate Project Planning and Estimation
Well-defined requirements serve as the foundation for reliable project planning.  
- Helps in estimating **time, cost, and resources** accurately.  
- Prevents delays and budget overruns caused by vague or shifting requirements.  

### 3. Risk and Cost Reduction
Requirement Analysis reduces the chances of project failure by addressing issues early.  
- Detecting requirement gaps in the early stages is far cheaper than fixing them during coding or testing.  
- Minimizes risks such as wasted development effort, rework, and stakeholder dissatisfaction.  

---

## Key Activities in Requirement Analysis

Requirement Analysis involves several structured activities that help ensure the final software system meets user and business needs. The five key activities are:

- **Requirement Gathering**  
  - Collecting raw requirements from stakeholders such as clients, end-users, and business analysts.  
  - Involves understanding the problem domain and identifying what stakeholders expect from the system.  

- **Requirement Elicitation**  
  - Using techniques such as interviews, workshops, brainstorming, surveys, and observation to extract detailed requirements.  
  - Helps uncover hidden needs, constraints, and assumptions that might not be immediately obvious.  

- **Requirement Documentation**  
  - Recording requirements in a structured format, typically in a **Software Requirement Specification (SRS)** document.  
  - Ensures requirements are clearly written, unambiguous, and serve as an official reference for the development team.  

- **Requirement Analysis and Modeling**  
  - Analyzing gathered requirements to resolve conflicts, check feasibility, and ensure completeness.  
  - Creating visual models such as use case diagrams, data flow diagrams (DFD), or entity-relationship diagrams (ERD) to represent requirements clearly.  

- **Requirement Validation**  
  - Reviewing and verifying requirements with stakeholders to confirm accuracy, feasibility, and alignment with business goals.  
  - Ensures requirements are **clear, consistent, testable, and achievable** before moving to the design phase.
  - 
## Types of Requirements

### Functional Requirements  
Functional requirements describe **what** the system must do. They are features, behaviors, and functions the software must support.

Examples for a hotel-booking project:

- Users must be able to **search** hotels by location, check-in / check-out date, price range, number of guests.  
- The system must allow users to **book** a hotel room, including selecting room type, confirming availability, and making a reservation.  
- Integration with **payment gateway** so users can pay online.  
- Hotel managers must have a portal to **manage their hotel listings**: add/update hotel info, room availability, rates.  
- The system must send **notifications** (email or app push) to users and hotel managers when a booking is confirmed or cancelled.  

---

### Non-Functional Requirements  
Non-functional requirements describe **how** the system performs or operates. They include constraints, qualities, system performance, usability, reliability, etc.

Examples for the same hotel-booking project:

- **Performance / Scalability**: The system should support high user traffic (many concurrent search / booking requests), e.g. through load balancing, caching (e.g. using Redis), and database scaling (master-slave, replicas). :contentReference[oaicite:0]{index=0}  
- **Availability / Fault tolerance**: The impact of downtime must be minimized; the hotel booking service must be highly available. Components like multiple servers and use of replicas to ensure read/write separation help. :contentReference[oaicite:1]{index=1}  
- **Latency / Responsiveness**: Search responses should be fast. Use of caching (e.g. Redis) and optimized search (e.g. ElasticSearch) to reduce time to return results. :contentReference[oaicite:2]{index=2}  
- **Consistency & Data Integrity**: Reservation data must be accurate (no double-booking), database transactions must maintain integrity.  
- **Security**: Protect user data (payment info, personal details), secure communication (TLS/HTTPS), prevent unauthorized access to management portals.  
- **Maintainability / Extensibility**: The architecture should make it possible to add new features (e.g. reviews, offers, recommendation engine) without major rework.  

## Use Case Diagrams

### What are Use Case Diagrams?
Use Case Diagrams are a type of **Unified Modeling Language (UML)** diagram that visually represent the interactions between **actors** (users or external systems) and the **system** itself.  

They help illustrate the functional requirements of a system by showing:  
- **Actors**: The entities (people or systems) that interact with the system.  
- **Use Cases**: The actions or services the system provides to the actors.  
- **Relationships**: How actors are connected to use cases.  

### Benefits of Use Case Diagrams
- Provide a **clear, visual overview** of system functionality.  
- Help in identifying **stakeholder needs and system boundaries**.  
- Facilitate communication between **technical and non-technical stakeholders**.  
- Act as a foundation for creating **detailed requirements** and **test cases**.  

---

### Use Case Diagram for the Booking Management System

The following diagram represents the hotel booking system, inspired by apps like Airbnb or OYO.

**Actors:**
- **Guest/User**: Searches for hotels, books rooms, makes payments, manages bookings.  
- **Hotel Manager**: Manages hotel listings, availability, and pricing.  
- **Payment Gateway**: Processes payments securely.  
- **System Admin**: Monitors and maintains the system.  

**Use Cases:**
- Search for hotels  
- View hotel details  
- Book a room  
- Cancel booking  
- Make payment  
- Manage listing (add/update rooms, availability, pricing)  
- Receive booking notifications  
- System monitoring and maintenance  

---

### Diagram

![Use Case Diagram for Booking Management System](alx-booking-uc.png)

## Acceptance Criteria

### Importance of Acceptance Criteria
Acceptance Criteria are a set of predefined conditions that a software feature must meet in order to be accepted by stakeholders. They act as a bridge between requirements and testing, ensuring that **what is built matches what was intended**.  

**Key benefits of Acceptance Criteria in Requirement Analysis:**
- **Clarity of Expectations:** Clearly defines what “done” means for a feature.  
- **Testability:** Provides measurable conditions that can be verified during testing.  
- **Alignment:** Ensures developers, testers, and stakeholders share the same understanding of requirements.  
- **Scope Control:** Prevents scope creep by defining boundaries for feature behavior.  
- **Quality Assurance:** Serves as a baseline to validate that the delivered product meets business and user needs.  

---

### Example: Acceptance Criteria for Checkout Feature

**Feature:** *Checkout Process for Hotel Booking*  

**Acceptance Criteria:**
1. The system must allow a guest to view a summary of their booking (hotel details, room type, price, taxes, and total cost) before proceeding to payment.  
2. The guest must be able to select a saved payment method or enter new payment details securely.  
3. The system must integrate with the payment gateway to process the transaction.  
4. If payment is successful:  
   - The booking should be confirmed.  
   - A confirmation notification (email and/or push notification) should be sent to the guest.  
   - The hotel manager should receive a booking notification.  
5. If payment fails:  
   - The system should display an appropriate error message.  
   - The guest should be allowed to retry payment or select another method.  
6. The booking should not be created or confirmed until payment is successfully completed.  

---
