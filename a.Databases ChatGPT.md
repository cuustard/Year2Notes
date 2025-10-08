# Week 1 – Introduction to Data Engineering

**Module:** SCC.221 – Data Engineering  
**Lecturer:** Uraz C. Turker  
**Year:** 2025  

---

## 🎯 Learning Outcomes
By the end of this week, you should be able to:

- Define key terms:
  - **Data**
  - **Data Engineering**
  - **Database**
  - **Database Management System (DBMS)**
- Understand basics of **Entity–Relationship (ER) Diagrams**

---

## 🧩 What is Data?

- **Definition:** Anything that can be represented using *binary notation*.
- **Examples of data generation:**
  - Eating  
  - Travelling  
  - Chatting  
  - Phone conversations  
  - Gaming  
- **Purpose of data:** To retrieve **information** through **processing**.
- **Processing requirement:** Establish a  
  - **Flexible**,  
  - **Understandable**, and  
  - **Common representation** for data.

---

## 🏗️ What is Data Engineering?

> “The process of designing and building systems that allow people to collect, manage, and analyse data.”

### Key Responsibilities of Data Engineers
- **Data pipelines:** Build and maintain data flows for large datasets.  
- **Data integration:** Combine data from multiple sources.  
- **Data quality:** Ensure accuracy, reliability, and efficiency.  
- **Data analysis:** Provide insights and predictive models.  
- **Data security:** Protect data from loss or theft.  
- **Automation:** Streamline workflows for efficiency.

**Common Tools:** Hadoop, MongoDB, Kafka.

---

## 🗄️ Databases

### Definition
Structured systems for **storing, retrieving, and managing data**.

- Types: Relational (e.g., MySQL, PostgreSQL)
- Organized via **data models** defining structure & relationships.
- Must support:
  - Efficient query execution
  - Fast access
  - Secure storage
  - Scalable infrastructure (on-premise or cloud)

### Why DBMS?
Before DBMS:
- Data was stored in **file-processing systems**
- Problems:
  - Difficult to maintain
  - Low performance & reliability
  - No standardization (formatting, coding)
  
**Analogy:** DBMS is to data what an operating system is to hardware.

---

## 🧠 Database Concepts

| Concept | Description |
|----------|-------------|
| **Database** | Massive collection of persistent data organized by a logical model |
| **DBMS** | Software that provides efficient, reliable, safe, and multi-user access to data |
| **Logical Model** | Abstract representation of data; can be drawn as UML or ER diagram |

---

## 🎮 Databases in Real Life
- **EVE Online:** Uses static data exports (e.g., `agtAgents.csv`, `agtAgentTypes.csv`)  
- **Counter-Strike:** Example of game databases for player data, maps, etc.

---

## 📊 Entity–Relationship (ER) Diagrams

**Purpose:**  
Graphical representation of database *logic*, *rules*, and *structure*.

### Why Use ER Diagrams?
- Aid in documentation, debugging, updates, and maintenance.
- Represent **business rules** visually (like UML).

---

## 🧱 ER Concepts: Entity

| Term | Definition | Representation |
|------|-------------|----------------|
| **Entity** | Object with distinguishable attributes | Rectangle |
| **Attribute** | Property or characteristic of an entity | Oval |
| **Entity Set** | Collection of entities with same attributes | Table/schema |

### Example: `Car` Entity
| Model | Weight | Length | Max_Speed |
|--------|--------|--------|------------|
| BMW 3.21 | 1400 | 4.2 | 200 |
| Toyota Corolla | 1300 | 4.1 | 180 |

- **Key Attribute:** `Model` (uniquely identifies rows)
- **Primary Key:** Underlined key attribute
- **Derived Attribute:** Dashed oval (e.g., `Max_K_Energy`)
- **Multi-Valued Attribute:** Double oval (e.g., `Pre_Owners`)
- **Composite Attribute:** Grouped attributes (e.g., `Properties` from `Length`, `Weight`, etc.)

---

## 🧩 Relationships in ER Models

| Concept | Definition | Representation |
|----------|-------------|----------------|
| **Relationship** | Logical association between entities | Diamond |
| **Relationship Set** | Set of all such associations | — |
| **Degree** | Number of entity sets involved (Unary, Binary, Ternary) | — |

### Examples
- **Binary:** `Mechanic` repairs `Car`
- **Ternary:** `Customer` borrows `Loan` from `Branch`
- **Unary:** `Jedi` teaches another `Jedi` (self-relationship)

---

## 🔢 Cardinalities (Mapping Constraints)

**Definition:** Describe how many entities in one set relate to those in another.

| Type | Description | Example |
|------|--------------|----------|
| **1:1** | Each entity in A relates to one in B | Marriage |
| **1:N** | One A relates to many Bs | Person → Phone Numbers |
| **N:1** | Many As relate to one B | Students → University |
| **M:N** | Many As relate to many Bs | Students ↔ Courses |

**Business Rules determine cardinality!**

---

## 🧠 Key ER Terms Summary

| Term | Description |
|------|--------------|
| **DDL** | Data Definition Language – Create/modify tables |
| **DML** | Data Manipulation Language – Modify data |
| **Entity** | Object with attributes |
| **Entity Set** | Group of entities of same type |
| **Key Attribute** | Uniquely identifies an entity |
| **Primary Key** | Chosen unique identifier |
| **Derived Attribute** | Computed value (dashed line) |
| **Multi-valued Attribute** | Multiple values (double oval) |
| **Composite Attribute** | Grouped attributes |
| **Relationship** | Association between entities |
| **Cardinality** | Number of entities in relation |

---

## 🧰 Key Roles in Database Design

| Role | Responsibility |
|------|----------------|
| **DBMS Implementer** | Builds database system software |
| **DB Designer** | Designs schema and logical structure |
| **DB Application Developer** | Creates apps using the database |
| **DB Administrator (DBA)** | Manages, secures, and maintains database |

---

## 🧾 Summary

- **Data Engineering** bridges **raw data** and **useful information**.
- **Databases** enable structured storage and efficient data retrieval.
- **ER Diagrams** represent the **logical structure** of data.
- **Business rules** define **relationships** and **cardinalities**.
- Understanding **entities**, **attributes**, and **relationships** is foundational before SQL.

---

## 🧠 Quick Self-Check

1. What distinguishes data from information?  
2. What are key roles of a data engineer?  
3. Why do we need DBMS instead of file-based storage?  
4. What shapes represent entities and relationships in ER diagrams?  
5. What’s the difference between primary, derived, and multi-valued attributes?  
6. Define 1:1, 1:N, N:1, and M:N relationships.

---

**References:**
- Uraz C. Turker, *SCC.221 Data Engineering – Week 1 Lecture Slides* (2025)
- [EVE Online Static Data Export](https://wiki.eveuniversity.org/Static_Data_Export)
- [CS:GO Database Example](https://www.csgodatabase.com/about/)
