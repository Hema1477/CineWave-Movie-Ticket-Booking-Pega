# CineWave-Movie-Ticket-Booking-Pega
Movie Ticket Booking Management application developed using Pega Platform for CineWave Entertainment. The application manages movie ticket requests, show availability, customer approval, booking execution, SLA tracking, work queue routing, and automated email confirmation.
Today 11:15 PM
HEMAPRIYA_GOVINDAN.pdf
PDF
how to make a github link and the description

Done! I created a visual one-page Project Preview using the screenshots and content from your uploaded PDF. The preview includes the project overview, Pega case lifecycle, key features, routing, SLA, and application visuals.

📄 Files
Download the Project Preview PDF
Download the Project Preview PNG

You can use the PDF for your project submission and the PNG for the SkillWallet project preview/demo section. 

CineWave_Project_Preview.pdf
PDF
CineWave_Project_Preview.png
Image
workflow and description of this  project to upload in github

Absolutely. For your CineWave Entertainment Pega project, your GitHub should look professional and clearly explain what the project does + how the workflow works.

You can copy-paste the following directly into your GitHub README.md.

🎬 CineWave Entertainment – Movie Ticket Booking Management
📌 Project Description

CineWave Entertainment – Movie Ticket Booking Management is a Pega Platform-based application designed to streamline and automate the movie ticket booking process.

The application manages the complete booking journey from the initial customer ticket request to show availability checking, customer approval, booking execution, and final confirmation. It replaces manual email and offline booking processes with a structured case-management workflow that improves visibility, reduces delays, and provides better coordination between customers and booking staff.

The application is developed using Pega Blueprint and Pega App Studio, with automated business logic, SLA monitoring, work queue routing, cost calculation, and email notification.

🎯 Project Objectives
Allow customers to submit movie ticket booking requests.
Enable staff to check movie show and seat availability.
Capture customer confirmation before final booking.
Automatically calculate the total ticket cost.
Route booking requests based on show type.
Track the booking request throughout its lifecycle.
Apply SLA monitoring to booking requests.
Notify customers after successful booking confirmation.
🔄 Project Workflow

The Movie Ticket Request case follows four main stages:

                    CUSTOMER
                       │
                       ▼
              ┌─────────────────┐
              │  Initial Stage  │
              │ Submit Request  │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │  Availability   │
              │ Check Seats &   │
              │ Show Details    │
              └────────┬────────┘
                       │
                Seats Available?
                   /         \
                 No           Yes
                 │             │
                 ▼             ▼
              Request       ┌───────────────┐
              Not Available │   Approval    │
                            │Customer       │
                            │Confirmation   │
                            └───────┬───────┘
                                    │
                              Confirm?
                              /     \
                            No       Yes
                            │         │
                            ▼         ▼
                         Reject   ┌──────────────────┐
                                  │Booking Execution │
                                  │ Finalize Booking │
                                  └────────┬─────────┘
                                           │
                                           ▼
                                    CASE RESOLVED
                                           │
                                           ▼
                                   EMAIL CONFIRMATION
🧩 Case Lifecycle
1. Initial Stage

The customer submits a Movie Ticket Request with relevant booking information such as:

Customer name
Email
Phone number
Movie
Theatre
Location
Show date
Show time
Show type
Number of tickets
Ticket price

The system uses the entered ticket information to determine the booking cost.

2. Availability Stage

Staff check whether the requested show has sufficient available seats.

The system compares:

Requested Tickets ≤ Available Seats

If sufficient seats are available, the case proceeds to the Approval stage.

3. Approval Stage

The customer must confirm the booking before the system performs the final booking.

Customer Confirmation
        │
    ┌───┴────┐
    ▼        ▼
 Confirm    Reject
    │        │
    ▼        ▼
Booking    Stop/Close
Execution   Request

This prevents tickets from being finalized without customer confirmation.

4. Booking Execution

After customer confirmation, the booking request proceeds to Booking Execution.

The booking is finalized and the case is resolved successfully.

After successful resolution, an automated confirmation email is sent to the customer.

💰 Automatic Cost Calculation

The application automatically calculates the booking cost using:

Total Cost = Ticket Price × Number of Tickets
Example
Ticket Price      = ₹300
Number of Tickets = 3

Total Cost = ₹300 × 3
           = ₹900

This reduces manual calculation errors.

🎟️ Show Type-Based Routing

Booking requests are automatically routed according to Show Type.

Show Type	Work Queue
Premium	Premium ShowQueue
Standard	Standard ShowQueue

Workflow:

                  Show Type
                     │
             ┌───────┴───────┐
             ▼               ▼
          Premium         Standard
             │               │
             ▼               ▼
    Premium ShowQueue  Standard ShowQueue

This allows staff to manage different categories of shows efficiently.

⏱️ SLA Configuration

The Movie Ticket Request case includes SLA monitoring:

SLA Parameter	Configuration
Goal	1 day
Deadline	2 days

The SLA helps monitor booking requests and identify cases that require timely action.

🗂️ Data Objects
Movie

The Movie data object stores movie-related information such as:

Movie Name
Genre
Language
Duration
Show

The Show data object stores show-related information such as:

Theatre
Location
Show Date
Show Time
Show Type
Ticket Price
Available Seats
📧 Email Confirmation

After successful booking and case resolution, the application automatically sends a confirmation email to the customer.

The confirmation contains relevant booking information such as:

Customer name
Movie
Theatre
Show date
Show time
Number of tickets
Total cost
Booking confirmation
🛠️ Technology Used
Pega Platform
Pega Blueprint
Pega App Studio
Pega Case Management
Data Objects
Business Rules
Work Queues
SLA Management
Email Correspondence
📊 Key Features

✅ Movie Ticket Request case management
✅ Four-stage booking lifecycle
✅ Movie and Show data objects
✅ Show availability checking
✅ Automatic Total Cost calculation
✅ Customer approval before booking
✅ Premium/Standard work queue routing
✅ SLA monitoring
✅ Booking status tracking
✅ Automated email confirmation

📸 Project Screenshots

Add your Pega screenshots here:

## Project Screenshots

### Case Lifecycle
![Case Lifecycle](Screenshots/case-lifecycle.png)

### Movie Data Object
![Movie Data Object](Screenshots/movie-data-object.png)

### Show Data Object
![Show Data Object](Screenshots/show-data-object.png)

### Availability
![Availability](Screenshots/availability.png)

### Customer Approval
![Approval](Screenshots/approval.png)

### Show Type Routing
![Routing](Screenshots/show-type-routing.png)

### SLA Configuration
![SLA](Screenshots/sla.png)

### Booking Confirmation
![Booking Confirmation](Screenshots/booking-confirmation.png)
👩‍💻 Project Author

Hemapriya Govindan

Project: Movie Ticket Booking Management
Platform: Pega Platform
Application: CineWave Entertainment

⭐
