# Phase 1 Waterfall Complete Report

## Requirement_Engineer

## Use Cases

### UC1: Student Registration and Profile Setup

* As a student, I want to register for the LMS and set up my profile, so I can access personalized learning paths and AI tutor support.
* Precondition: Student has a valid email address and password.
* Postcondition: Student profile is created, and AI tutor is initialized.

### UC2: AI Tutor Chatbot

* As a student, I want to engage with the AI tutor chatbot to get help with course-related questions, so I can clarify concepts and get feedback.
* Precondition: Student is logged in and has access to the AI tutor.
* Postcondition: AI tutor provides relevant answers, explanations, and suggestions for next steps.

### UC3: Instructor Course Creation and Management

* As an instructor, I want to create and manage courses, including setting up learning objectives, assessments, and project plans, so I can effectively teach and track student progress.
* Precondition: Instructor is logged in and has the necessary permissions.
* Postcondition: Course materials are created, and AI agents are initialized for project planning support.

### UC4: Student Progress Tracking and Insights

* As a student, I want to track my progress, see areas for improvement, and receive recommendations for next steps, so I can stay motivated and focused.
* Precondition: Student is logged in and has access to their progress dashboard.
* Postcondition: Student sees their learning path progress, completed modules, scores, and identified weak areas with AI-generated insights and recommendations.

### UC5: Instructor Progress Tracking and Analytics

* As an instructor, I want to track student progress, see class-level analytics, and receive insights and recommendations, so I can identify areas for improvement and adjust my teaching approach.
* Precondition: Instructor is logged in and has the necessary permissions.
* Postcondition: Instructor sees class-level analytics, engagement, completion rates, average performance by topic, and individual student insights including risk of falling behind

## System_Engineer

## System Architecture

The system architecture for the Learning Management System (LMS) consists of the following layers:

* **Presentation Layer**: Web-based interface for students and instructors to interact with the system.
* **Application Layer**: Handles user requests, authenticates users, and provides access to AI tutor and course management features.
* **Business Logic Layer**: Contains the core logic for AI tutor chatbot, course creation, and management.
* **Data Access Layer**: Provides access to the database for storing student profiles, course data, and AI tutor conversations.
* **Data Storage Layer**: Manages the database for storing and retrieving data.

## Component Diagram

The component diagram shows the relationships between the components:

* **Student Registration and Profile Setup**:
	+ Component: Student Registration and Profile Setup
	+ Dependencies: AI Tutor, Course Management
* **AI Tutor Chatbot**:
	+ Component: AI Tutor Chatbot
	+ Dependencies: Student Profile, Course Data
* **Instructor Course Creation and Management**:
	+ Component: Instructor Course Creation and Management
	+ Dependencies: Course Data, Student Profile

## Sequence Diagram

The sequence diagram shows the interactions between the components:

* **Student Registration and Profile Setup**:
	1. Student requests registration
	2. System authenticates student
	3. System creates student profile
	4. AI tutor is initialized
* **AI Tutor Chatbot**:
	1. Student initiates chatbot conversation
	2. AI tutor processes conversation
	3. AI tutor provides answers and explanations
* **Instructor Course Creation and Management**:
	1. Instructor requests course creation
	2. System creates course
	3. Instructor sets learning objectives, assessments, and project plans

## ER Diagram

The ER diagram shows the relationships between the entities:

* **Student**:
	+ Attributes: student_id, email, password, profile_setup
* **Course**:
	+ Attributes: course_id,

## Software_Engineer

## Implementation Task List

### Presentation Layer

* Implement web-based interface for students and instructors
* Handle user requests and authentication
* Integrate with Application Layer

### Application Layer

* Handle user requests and authentication
* Provide access to AI tutor and course management features
* Integrate with Business Logic Layer

### Business Logic Layer

* Implement AI tutor chatbot
* Implement course creation and management
* Integrate with Data Access Layer

### Data Access Layer

* Provide access to database for storing student profiles, course data, and AI tutor conversations
* Integrate with Data Storage Layer

### Data Storage Layer

* Manage database for storing and retrieving data
* Integrate with Data Access Layer

## Dependencies

* Presentation Layer: Application Layer, Business Logic Layer
* Application Layer: Business Logic Layer, Data Access Layer
* Business Logic Layer: Data Access Layer
* Data Access Layer: Data Storage Layer

## Development Phases

### Phase 1: Presentation Layer

* Implement web-based interface for students and instructors
* Handle user requests and authentication

### Phase 2: Application Layer

* Handle user requests and authentication
* Provide access to AI tutor and course management features

### Phase 3: Business Logic Layer

* Implement AI tutor chatbot
* Implement course creation and management

### Phase 4: Data Access Layer

* Provide access to database for storing student profiles, course data, and AI tutor conversations

### Phase 5: Data Storage Layer

* Manage database for storing and retrieving data

## 4. Effort Calculation

SLOC = 15000  
Productivity = 50 SLOC/day  

Effort = 15000 / 50 = 300 days

## Test_Engineer

**Test Plan**
================

### Test Strategy

* Black box testing: Verify functionality and behavior without knowledge of internal implementation
* White box testing: Verify internal implementation and logic
* Gray box testing: Verify functionality and behavior with knowledge of internal implementation

### Functional Tests

* **Presentation Layer**
	+ Test user authentication and authorization
	+ Test AI tutor chatbot functionality
	+ Test course creation and management
* **Application Layer**
	+ Test user request handling and authentication
	+ Test AI tutor and course management integration
* **Business Logic Layer**
	+ Test AI tutor chatbot logic and conversation flow
	+ Test course creation and management logic
* **Data Access Layer**
	+ Test database access and data retrieval
* **Data Storage Layer**
	+ Test database storage and retrieval

### Non-Functional Tests

* **Performance**
	+ Test system response time and throughput
* **Security**
	+ Test user authentication and authorization
	+ Test data encryption and access control
* **Usability**
	+ Test user interface and user experience

### Schedule

* Week 1-2: Test planning and preparation
* Week 3-4: Functional testing (Presentation, Application, Business Logic)
* Week 5-6: Non-functional testing (Performance, Security, Usability)
* Week 7: Test reporting and documentation

### Effort Calculation

* Estimated test cases: 20
* Test cases per day: 2
* Total test days: 10
* Total effort: 20 test cases/day \* 10 days = 200 test cases
* Estimated effort: 200 test cases \* 1 day/test case = 200 days

## Documentation_Engineer

**Documentation Plan**
=====================

### User Documentation Outline

* **Overview**
	+ Introduction to the AI tutor chatbot and course creation platform
	+ Features and benefits
* **Getting Started**
	+ User registration and login
	+ AI tutor chatbot usage and conversation flow
* **Course Creation and Management**
	+ Creating and managing courses
	+ Adding and managing course content
* **FAQs and Troubleshooting**
	+ Frequently asked questions
	+ Troubleshooting common issues

### Developer Documentation Outline

* **Architecture**
	+ Overview of the system architecture
	+ Component diagrams and descriptions
* **API Documentation**
	+ API endpoints and request/response formats
	+ API usage guidelines and best practices
* **Code Snippets and Examples**
	+ Code examples for key features and functionality
	+ Code snippets for troubleshooting and debugging
* **Release Notes and Changelogs**
	+ Release notes and changelogs for each version

### Documentation Schedule

* Week 1: Complete user documentation outline and start writing
* Week 2: Complete developer documentation outline and start writing
* Week 3: Finish writing and reviewing user and developer documentation
* Week 4: Finalize and publish documentation

**Effort Calculation**
=====================

* Estimated documentation pages: 30
* Pages per day: 3
* Total days: 10
* Total effort: 30 pages / 3 pages per day = 10 days

Estimated effort: 10 days

