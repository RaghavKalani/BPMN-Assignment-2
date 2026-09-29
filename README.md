# BPMN Process Modeling — Lab Practice

## Overview

This repository contains BPMN process models created using **Camunda 8** as part of the BPMN Process Modeling Lab Practice.

The models demonstrate the use of:

* Start Events
* Tasks
* Exclusive Gateways
* Sequence Flows
* Alternative Process Paths
* End Events

---

## Scenario 1: Hotel Room Reservation

### Process Description

The process begins when a guest submits a room booking request with check-in and check-out dates.

The reservation system checks room availability.

* If no room is available, the guest is notified and the process ends.
* If a room is available, an advance payment is requested and processed.
* If the payment fails, the guest is notified and the process ends.
* If the payment is successful, the booking is confirmed and a booking reference is generated.
* A booking confirmation email containing the reservation details is then sent to the guest.
* The process ends after the confirmation email is sent.

### BPMN Model

[View Hotel Room Reservation BPMN Model](models/scenario-1-hotel-room-reservation.bpmn)

---

## Scenario 2: Loan Application Processing

### Process Description

The process begins when a customer submits a personal loan application.

The bank system verifies the submitted documents and credit score.

* If the documents are incomplete or invalid, the application is rejected and the customer is notified.
* If the documents are valid, the applicant's eligibility is checked based on credit score and income.
* If the applicant is not eligible, a rejection notification is sent.
* If the applicant is eligible, the application is forwarded to a loan officer for final approval.
* If the loan officer rejects the application, the customer receives a rejection notification.
* If approved, the loan amount is disbursed and an approval notification is sent.
* The process ends after the appropriate notification.

### BPMN Model

[View Loan Application Processing BPMN Model](models/scenario-2-loan-application-processing.bpmn)

---

## Scenario 3: Job Applicant Recruitment Process

### Process Description

The process begins when a candidate submits a job application online.

The HR system screens the application against the minimum eligibility criteria.

* If the candidate is not eligible, a rejection notification is sent and the process ends.
* If eligible, a technical interview is scheduled.
* The technical panel evaluates the candidate.
* If the candidate fails the technical interview, a rejection notification is sent.
* If the candidate passes, an HR/managerial round is scheduled.
* The candidate is evaluated in the HR/managerial round.
* If rejected, a rejection notification is sent.
* If selected, the system generates an offer letter and sends it to the candidate.
* The process ends after the offer letter is sent.

### BPMN Model

[View Job Applicant Recruitment BPMN Model](models/scenario-3-job-applicant-recruitment.bpmn)

---

## Repository Structure

```text
BPMN-Process-Models/
│
├── README.md
│
└── models/
    ├── scenario-1-hotel-room-reservation.bpmn
    ├── scenario-2-loan-application-processing.bpmn
    └── scenario-3-job-applicant-recruitment.bpmn
```

---

## Tools Used

* **Camunda 8 Web Modeler** — BPMN process modeling
* **BPMN 2.0** — Process modeling notation
* **GitHub** — Version control and submission

---

## Submission

The repository contains the completed BPMN models for all three scenarios along with their corresponding process descriptions.

All BPMN models have been created and organized according to the requirements of the lab practice assignment.
