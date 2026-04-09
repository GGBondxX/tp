### **leegoang - Project Portfolio Page**

## **Overview**

I am a Year 2 Computer Engineering student at NUS, and this portfolio highlights my technical contributions to **ModTrack**, a CLI-based module management application. My primary focus was designing and implementing the **UI layer**, ensuring code quality through testing, and maintaining clear documentation for both developers and users.

---

## **Summary of Contributions**

### **1. Issue Tracker & Project Coordination**
* **What it is:** I managed the issue tracker, ensuring all tasks were clearly defined, tracked, and assigned.
* **Technical Detail:** I created structured user stories, applied appropriate labels, and ensured proper linkage between issues and pull requests. I verified that PRs referenced the correct issues and milestones, and enforced consistent workflows across the team.
* **Impact:** This improved traceability between features and code changes, reduced ambiguity in task ownership, and ensured smoother integration of team contributions.

---

### **2. UI Development & Refactoring**
* **What it is:** I designed and implemented the **`Ui` class**, which handles all user-facing output for the CLI application.
* **Technical Detail:**  
  - Refactored the UI into **modular, single-responsibility methods** (e.g., `showAddModule`, `showDeletedModule`, `showPrerequisites`, `showComparedList`).  
  - Standardized all output using `System.out.println` to ensure **consistent formatting and predictable output behavior**.  
  - Introduced reusable helper methods such as `showDivider()` to eliminate duplicated code.  
  - Improved UI consistency by standardizing message formats and structuring outputs (headers, sections, and separators).  
  - Ensured proper **separation of concerns** by avoiding modification of model state inside UI methods.  
* **Impact:** This resulted in a clean, maintainable UI layer that is easier to extend, reduces duplication, and minimizes the risk of inconsistent or incorrect output.

---

### **3. UI Testing (JUnit)**
* **What it is:** I developed comprehensive **JUnit tests** for the UI layer.
* **Technical Detail:**  
  - Implemented tests using `ByteArrayOutputStream` to **capture and verify console output**.  
  - Designed test cases covering multiple UI methods, including:
    - Output formatting (e.g., `showAddModule`, `showDeletedModule`)  
    - Edge cases (e.g., empty module list, no prerequisites)  
    - Error messages and user feedback  
  - Updated tests to reflect refactored method signatures and behavior changes (e.g., transition from string-based inputs to `Mod` objects).  
* **Impact:** These tests ensured UI correctness after refactoring, improved reliability of user-facing features, and helped catch regressions early during development.

---

### **4. Code Maintenance & Bug Fixing**
* **What it is:** I actively maintained code quality and resolved integration issues within the team.
* **Technical Detail:**  
  - Fixed inconsistencies in imports and package structures across team contributions.  
  - Identified and resolved UI-related bugs, including formatting issues and incorrect output behavior.  
  - Ensured adherence to coding standards (e.g., checkstyle compliance and consistent method naming).  
* **Impact:** This reduced runtime errors, improved overall codebase stability, and ensured smoother collaboration among team members.

---

## **Contributions to Documentation**

* **Developer Guide:**  
  - Drafted the initial DG structure and table of contents.  
  - Documented the **UI component design**, including responsibilities and interaction with other components.  
  - Provided setup instructions and execution steps for developers.  

* **User Guide:**  
  - Documented features such as `exit` and `show grad req`.  
  - Enhanced the guide by adding **error handling explanations and resolutions** for each command, improving usability.  
  - Ensured command formats and examples were clear and consistent.  

* **Project Scope & Requirements:**  
  - Wrote the Product Scope and Non-Functional Requirements sections, defining system constraints and user expectations.  

* **Impact:**  
  My documentation improved clarity for both developers and users, reduced onboarding time, and ensured the system’s functionality and limitations were well understood.

---

## **Overall Contribution**

My contributions focused on strengthening the **UI architecture, testing reliability, and documentation quality** of ModTrack. By refactoring the UI into a clean, modular structure and supporting it with targeted tests, I helped ensure that the application delivers consistent and reliable user interactions while remaining maintainable for future development.
