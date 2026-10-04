# Implement Client Script & UI Policy (Incident)

## Project Overview

This project focuses on implementing **Client Scripts and UI Policies in ServiceNow Incident Management** to improve form behavior, enforce data validation, and maintain consistent data entry.

## Project Objectives

- Implement UI Policies on the Incident form.
- Configure UI Policy Actions.
- Create Client Scripts for dynamic form behavior.
- Validate Incident information before submission.
- Control list-based updates.
- Test the implemented configurations.
- Document the complete project workflow.

## Technologies Used

- ServiceNow
- Incident Management
- UI Policies
- UI Policy Actions
- Client Scripts
- JavaScript
- g_form API

## Team Members

| Name | Role |
|---|---|
| Varsha Devi K H | Team Lead |
| Varshida Kannivadi Balaji | Member |
| Nithishkumar N K | Member |
| Yogasairam P | Member |

## Project Workflow

The project is organized into the following phases:

### 1. Brainstorming & Ideation

Initial brainstorming and identification of the project idea and problem statement.

### 2. Requirement Analysis

Analysis of project requirements, ServiceNow requirements, and required features.

### 3. Project Design Phase

Design of the Incident form behavior, UI Policies, UI Policy Actions, and Client Scripts.

### 4. Project Planning Phase

Planning of tasks, team responsibilities, implementation activities, testing, and documentation.

### 5. Project Development Phase

Implementation of:

- UI Policy
- UI Policy Action for Urgency
- onLoad Client Script
- onChange Client Script
- onSubmit Client Script
- onCellEdit Client Script

### 6. Project Testing

Testing the implemented configuration using different Incident scenarios.

Test cases include:

- Mandatory field enforcement
- Successful Incident save
- Reverse condition testing
- List edit validation
- Form-based updates

### 7. Project Documentation

Documentation of the project implementation, configuration, testing results, and screenshots.

### 8. Project Demonstration

Final demonstration of the ServiceNow Incident configuration and implemented features.

## UI Policy Implementation

**UI Policy Name:**  
`Incident - In Progress UI Policy`

**Table:**  
`Incident [incident]`

**Condition:**  
`State is In Progress`

### UI Policy Action

| Field | Mandatory | Visible | Read Only |
|---|---|---|---|
| Urgency | True | True | False |

When the Incident state is **In Progress**, the Urgency field is configured as mandatory.

## Client Scripts

The project includes the following Client Scripts:

1. **onLoad** – Controls form behavior when the Incident form loads.
2. **onChange** – Dynamically responds when the Category field changes.
3. **onSubmit** – Validates Incident information before submission.
4. **onCellEdit** – Validates changes made from the Incident list.

## Testing

The implemented UI Policies and Client Scripts are tested under different Incident conditions to ensure that the expected behavior is achieved.

## Screenshots

Screenshots of the implementation and testing results are maintained in the `Screenshots` folder.

## Project Structure

```text
servicenow-incident-client-script-ui-policy/
│
├── 1. Brainstorming & Ideation/
├── 2. Requirement Analysis/
├── 3. Project Design Phase/
├── 4. Project Planning Phase/
├── 5. Project Development Phase/
├── 6.Project Testing/
├── 7.Project Documentation/
├── 8.Project Demonstration/
├── Screenshots/
└── README.md
```

## Expected Outcome

The project demonstrates how ServiceNow UI Policies and Client Scripts can be used to:

- Dynamically control Incident fields.
- Make fields mandatory based on conditions.
- Validate user input.
- Prevent invalid updates.
- Improve data consistency.
- Provide a better Incident management experience.

## Demo

**Project Demonstration:**  
[View Project Demonstration](https://drive.google.com/file/d/1BhmvBjVNcBjm0UWHhcywjJF-rdP0it1r/view?usp=drivesdk)

## Conclusion

This project demonstrates the implementation and testing of Client Scripts and UI Policies in ServiceNow Incident Management. The configuration improves field control, validation, and consistency during Incident creation and updating.
