# Kim Minsun - Project Portfolio Page

## Project: ModTrack

ModTrack is a CLI (Command Line Interface) application designed for students to manage modules, track completion status, and organize prerequisite and graduation requirements. It is optimized for efficiency and clarity, leveraging a command-based architecture implemented in Java.

---

## Summary of Contributions

### 1. Core System Architecture (Parser, Storage, Execution Pipeline)

I was responsible for implementing the core execution backbone of the system, including the Parser, Storage system, and command execution pipeline. These components form the foundation upon which all features operate.

#### Parser System Design & Implementation

- Designed and implemented the full Parser responsible for interpreting user input  
- Converts raw input strings into structured `Command` objects  
- Differentiates between command types and extracts arguments  
- Enforces strict input validation rules  

**Impact:**
- Enabled scalable addition of commands without modifying core logic  
- Prevented malformed inputs from propagating into execution flow  
- Established a consistent command-handling pattern across the application  

---

#### Command Execution Pipeline Integration

- Integrated Parser output into the main application loop  

**Pipeline:**
User Input → Parser → Command → Model → UI  

**Impact:**
- Enforced a command-driven architecture  
- Standardized execution flow across all features  
- Reduced coupling between system components  

---

#### Persistent Storage System

- Implemented file-based storage (load/save)  

**Technical Details:**
- Handles serialization and deserialization of module data  
- Ensures consistency between runtime state and stored state  
- Safeguards against missing or malformed data  

**Impact:**
- Enables persistence across sessions  
- Prevents data loss  
- Supports real-world usability of the application  

---

#### Data Integrity: Duplicate Module Prevention

- Implemented validation to prevent duplicate module entries  

**Impact:**
- Maintains a consistent and reliable data model  
- Prevents downstream logical errors  

---

#### System Integration & Conflict Resolution

- Led integration of independently developed components into a stable system  

**Key Contributions:**
- Resolved merge conflicts across Parser, Command, UI, and Storage layers  
- Refactored code to ensure compatibility between implementations  
- Adapted logic to align with evolving system design  

**Impact:**
- Delivered a fully functional and stable Version 1.0  
- Ensured end-to-end system reliability  

---

### 2. Feature Development (Version 2.0 Enhancements)

Implemented multiple commands that extend ModTrack into a structured academic planning tool:

- AddPrereqCommand  
- ExemptCommand  
- FindCommand  
- ShowPrereqCommand  
- TransferCommand  

*(SetProgressCommand was implemented during development but omitted from the final deliverable.)*

---

#### Prerequisite Management System (AddPrereq & ShowPrereq)

- Introduced module dependency relationships  
- Supports assigning multiple prerequisites to a module  
- Enables retrieval and display of dependency information  

**Impact:**
- Transforms ModTrack from a flat list into a structured academic planner  
- Allows users to visualize module dependencies  

---

#### TransferCommand

- Enables modules to be moved across categories or states  

**Impact:**
- Requires safe state transitions and consistency checks  

---

#### ExemptCommand

- Allows modules to be marked as exempted  

**Impact:**
- Reflects real-world academic scenarios such as credit transfers  

---

#### FindCommand

- Implements keyword-based search  

**Impact:**
- Improves usability for large datasets  

---

### 3. Developer Guide Contributions

#### Command Documentation (Primary Author)

Authored Developer Guide sections for:

- AddPrereqCommand (Christina)  
- ShowPrereqCommand (Christina)  
- TransferCommand (Christina)  

Included:
- Parsing logic  
- Execution flow  
- Design rationale  
- Limitations  

---

#### Parser Architecture Documentation

- Documented how the Parser processes input, dispatches commands, and handles invalid cases  

**Impact:**
- Improves maintainability and extensibility  

---

#### UML & Sequence Diagrams

- Contributed diagrams for:
  - Command execution flow  
  - Parser-command interaction  
  - Features such as `mark`, `unmark`, `showgradreq`, and prerequisite commands  

- Improved:
  - UML correctness (inheritance, dependencies)  
  - Diagram clarity and layout  

---

#### Edge Cases & Limitations

- Added “Current Limitations” sections  
- Documented:
  - Invalid input handling  
  - Edge-case behaviors  
  - System constraints  

---

### 4. User Guide Contributions

- Authored and refined sections for:
  - `mark`, `unmark`  
  - `showgradreq`  
  - prerequisite-related features  

**Key Contributions:**
- Clear command formatting  
- Realistic usage examples  
- Explanation of edge cases  

---

### 5. Software Quality & Testing Support

- Contributed to command-level testing design  
- Verified functionality through realistic input scenarios  

---

### 6. Team Contribution & Engineering Ownership

- Took responsibility for delivering a stable Version 1.0 system  
- Ensured integration across Parser, Commands, Storage, and UI  

**Role:**
- Bridging individual contributions into a cohesive product  
- Maintaining consistency across system components  

---

## Code Contributed

- [RepoSense Dashboard](https://nus-cs2113-ay2526-s2.github.io/tp-dashboard/?search=violetsunshades&breakdown=true&sort=groupTitle%20dsc&sortWithin=title&since=2026-02-20T00%3A00%3A00&timeframe=commit&mergegroup=&groupSelect=groupByRepos&checkedFileTypes=docs~functional-code~test-code~other&filteredFileName=)

---

## Overall Contribution

My contributions focused on both system-level architecture and feature-level development. I implemented the core infrastructure (Parser, Storage, execution pipeline), ensured successful system integration for Version 1.0, and expanded functionality through multiple Version 2.0 features.

In addition, I contributed extensively to the Developer Guide and User Guide, strengthening the clarity, maintainability, and technical rigor of the project. Through these efforts, I helped transform ModTrack into a cohesive, well-documented, and extensible software system.
