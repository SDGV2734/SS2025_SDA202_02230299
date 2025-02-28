# Assignment Submission and Grading System

## 1. Introduction

The Assignment Submission and Grading System is designed to facilitate the ease the submission, evaluation, and grading of student assignments within an academic setting. The report provides an in-depth analysis of the system's Interaction Overview Diagram (IOD), Use Case Diagram (UCD), and Functional Overview to illustrate the core processes and actors involved.

## 2. Interaction Overview Diagram (IOD)

![Alt text](<IoD Class Practical.png>)

### 2.1 Purpose

The Interaction Overview Diagram (IOD) presents a structured flow of interactions between different system components, detailing how assignments move through submission, evaluation, and grading.

### 2.2 Process Flow

1. Submission Decision: The system determines whether a student submits an assignment.

    * If no submission, the process terminates.

    * If submission occurs, the process continues to code submission.

2. Code Submission: The student submits their assignment via the Learning Management System (LMS).

3. Plagiarism Check: The system forwards the submission to Turnitin for plagiarism verification.

4. Code Execution & Review:

    * If code submission passes plagiarism checks, it is sent for execution.

    * The Auto Grading System (AGS) evaluates the code’s correctness.


5. Grading Process:

    * The Auto Grading System assigns an initial grade.

    * Professors review and finalize grades.

6. Results Compilation: The LMS compiles the grades and feedback for student access.

### 2.3 Key Components

* Actors: Student, LMS, Professor, Auto Grading System, Turnitin

* Decisions: Submission validation, plagiarism check, grading method selection

* Final Output: Graded assignments with feedback stored in LMS

## 3. Use Case Diagram (UCD)

![Alt text](<Use Case Practical 1 (1).png>)

### 3.1 Purpose
The Use Case Diagram (UCD) provides a high-level overview of the interactions between actors and functional components.

### 3.2 Use Cases & Actors

1. Student:

    * Submit assignment

    * View submitted code

    * View feedback

2. Professor:

    * Review work

    * Set grading criteria


3. LMS:

    * Store and manage submissions

    * Check plagiarism

    * Process grading

    * Auto Grading System:

    * Run and grade code

    * Store and record grades

    * Plagiarism Checking Service (Turnitin):

    * Verify originality of submissions

### 3.3 System Flow

* Submission → Plagiarism Check → Grading (Auto/Manual) → Feedback Compilation → Result Storage

## 4. Functional Overview

![Alt text](<Functional Overview Practical 1 (1).png>)

### 4.1 Overview

The functional overview combines insights from the IOD and UCD to present a structured breakdown of how the system operates.

### 4.2 Core Functionalities

1. Assignment Submission

    * Students upload assignments to LMS.

    * Late submissions may be penalized or rejected.

2. Code Execution & Review

    * Auto Grading System executes code.

    * Professors review manually if required.

3. Plagiarism Check

    * Turnitin scans assignments for similarities.

    * Results determine further processing.


4. Grading Process

    * Automated Grading assigns initial scores.

    * Professors finalize and approve grades.

5. Store & Result Compilation

    * Grades are stored in LMS.

   * Students can review their performance.

6. View Grade Process

    * A regulatory body audits grading fairness.

    * Professors can modify grading criteria if needed.

### 4.3 System Flow Summary

* Input: Assignment submission (by students)

* Processing: Plagiarism check → Code execution → Auto/manual grading

* Output: Graded assignments and feedback (accessible via LMS)

## 5. Conclusion

The Assignment Submission and Grading System streamlines the submission and evaluation process, integrating automated and manual grading while ensuring academic integrity through plagiarism checks. The IOD and UCD highlight the interaction between actors, while the Functional Overview explains the system’s core functionalities, ensuring efficiency and fairness in academic assessments.