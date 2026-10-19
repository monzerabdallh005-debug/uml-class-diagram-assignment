 UML Class Diagram Modelling Assignment - Hotel Booking Management System
​Project Overview
​This repository contains the UML Class Diagram documentation and deliverables for the Hotel Booking Management System assignment at Kigali Independent University (ULK).
​Group Information
​Member 1: [AlmonzerAbdullah Adam] (ID: [202512093 ID])
​Member 2: [Awrad Mohamed / Pending] (ID: [202512287 ID / Pending])
​Business Idea & System Scope
​Business Idea
​The Hotel Booking Management System is an information system designed to automate room reservations, customer management, and payment processing for a hotel business. It eliminates manual errors and provides real-time tracking of available rooms.
​Project Scope
​In-Scope:
​Guest profile registration and management.
​Room catalog management (room type, pricing, availability).
​Reservation creation, modification, and status tracking.
​Payment record generation and receipt creation.
​Out-of-Scope:
​Third-party payment gateway API integrations.
​Physical keycard door lock integrations.
​External travel package agency bookings.

​Repository Structur
uml-class-diagram-assignment/
├── README.md
├── documentation/
│   ├── report_1_project_description.pdf
│   └── report_2_uml_class_diagram.pdf
└── diagrams/
    ├── uml_class_diagram.drawio
└── uml_class_diagram.png

Class Overview
Class                           NameKey Responsibilities
Guest                         Stores customer information and initiates booking requests.
Room                         Maintains hotel room details, rates, and availability state.
Reservation              Tracks booking dates, total costs, and reservation status.
Payment                   Handles transaction details and processes receipts.

Key Class Relationships
1.​Guest to Reservation (1 to 0..*): A guest can place zero or multiple reservations.
2.​Reservation to Room (1..* to 1): A reservation can include one or more rooms.
3.​Reservation to Payment (1 to 1): Each completed reservation requires exactly one payment.