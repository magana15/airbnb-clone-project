## Airbnb clone project ##
### project description ###
The project is a real world application designed to simulate the development of a robust booking like Airbnb which involves a deep dive into full-stack development. It focuses on backend systems database design API development and app security thus enabling the understanding of complex architectures workflows and collaborative team dynamics using technologies like **Django**, **docker** among others.

## Team Roles ##
### Business Analyst (BA) ###
Understands the customer’s business processes, elicits and translates business needs into requirements, bridges between stakeholders and the development team.
### Product Owner (PO) ###
Owns the product vision and evolution, balances business needs and market demands, ensures the product meets customer requirements, manages the product backlog.

### Project Manager ###
Ensures that the project is delivered on time and within budget, plans and organizes tasks, motivates the team, and maintains communication and status transparency.
### UI/UX Designer ###
Designs the user interface and overall user experience, creates user journeys, wireframes, prototypes, ensures functionality is intuitive and visually appealing.
### Software Architect ###
Designs the high-level system architecture, selects tools and technologies, defines code quality standards, oversees architecture decisions and integration approaches.
### Software Developer ###
Implements features and functionality (front-end, back-end, or full stack), writes and maintains code, solves technical problems during development.
### Quality Assurance  Engineer ###
Verifies that the application meets both functional and non-functional requirements, identifies defects, runs tests, ensures quality across features.
### Test Automation Engineer ###
Builds and maintains automated test scripts and frameworks, selects areas suitable for automation, ensures automated tests provide reliable feedback.
### DevOps Engineer ###
Facilitates collaboration between development and operations, builds CI/CD pipelines, automates deployment and operations to accelerate delivery while maintaining stability.


## Technology stack ##
### Django ###
A web framework for building RESTful APIs and managing backend logic such as authentication, bookings, and property listings.

### PostgreSQL ###
A relational database used to store structured data like users, listings, reviews, and transactions securely and efficiently.

### GraphQL ###
A query language for APIs that lets clients request exactly the data they need, improving performance and flexibility.

### Celery ###
A task queue system for running background jobs like sending confirmation emails or processing payments asynchronously.

### Redis ###
An in-memory data store used for caching, managing sessions, and acting as a message broker for Celery tasks.

### Docker ###
A containerization tool that packages the app and its dependencies to ensure consistent deployment across environments.

### CI/CD Pipelines ###
Automated workflows for continuously testing, building, and deploying new updates safely and efficiently.

## **database design** ##
users - id,name,email,role, created-on
properties- id, host-id,title,location,price
bookings - id, guest-id, check-in,check-out,status
payments - id, booking-id, amount,payment method,status
reviews - id, payment-id,guest-id,rating,comment

 ### **relationships** ###
- a host can have many properties
- a property can host many guests
- a user can review many properties
- a user can rate many properties
- a property can have many reviews
- a user can book many properties
