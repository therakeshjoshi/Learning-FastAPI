# What is an API?

APIs are mechanisms that enable two software components — such as the frontend and backend of an application — to communicate with each other using a defined set of rules, protocols, and data formats.

## How It Works

- The **Frontend** sends a **Request** to the API.
- The **API** forwards the request to the **Backend**.
- The **Backend** processes the request.
- The **Backend** sends a **Response** back through the API to the Frontend.

## Flow Representation

Frontend → Request → API → Backend  
Backend → Response → API → Frontend

# API Analogy

## Restaurant Example

An API works like a restaurant system.

- **Customer** → Sends a **Request**
- **Waiter** → Acts as the **API**
- **Kitchen** → Processes the request

## Flow

Customer → Request → Waiter → Kitchen  
Kitchen → Response → Waiter → Customer

## Explanation

- The **Customer** does not go directly to the Kitchen.
- The **Waiter (API)** takes the request to the Kitchen.
- The **Kitchen** prepares the response.
- The **Waiter** brings the response back to the Customer.


# Need for APIs

## Architecture Flow

Frontend → Backend → Database

- **Frontend** sends request to Backend.
- **Backend** processes the request.
- **Backend** interacts with the Database.
- **Database** returns data to Backend.
- **Backend** sends response to Frontend.

---

## Monolithic Architecture

In a monolithic architecture:


- Frontend and Backend exist in the same project.
- Single codebase.
- Structured into folders like:
- 
  <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/87cc67a5-cb41-44b8-b4d0-e6f77909b364" />



  # Solving Monolithic Problems Using APIs

## Architecture

Database  
   ↑  
Backend  
   ↑  
API  
   ↑  
Multiple Applications (Clients)

---

## Explanation

- The **Backend** communicates with the **Database**.
- The **API** acts as an interface between Backend and external applications.
- Multiple applications can access the same Backend using APIs.

---

## Technology Independence

Different applications can be built using different technologies:

- App 1 → Java
- App 2 → Python
- App 3 → PHP

All of them communicate with the Backend using:

- HTTP protocol
- JSON data format

---

## Advantages

- Backend logic remains centralized.
- Multiple clients can use the same backend.
- Technology flexibility on the client side.
- Better scalability compared to monolithic frontend-backend coupling.

- # API – ML Perspective

## Architecture (Monolithic)

Frontend → Backend → ML Model  
ML Model → Backend → Frontend

---

## Components

- ML Model
- Backend
- Frontend

In a monolithic architecture, all components are part of the same project.

---

## Explanation

- The Frontend sends input data.
- The Backend receives the request.
- The Backend calls the ML Model.
- The ML Model generates prediction.
- The Backend sends prediction back to Frontend.

---

## Typical Project Structure


src
├── templates
├── static
├── model.pkl
├── ml_backend.py
└── app.py


### File Description

- `model.pkl` → Trained machine learning model
- `ml_backend.py` → ML logic and prediction handling
- `app.py` → API application entry point
- `templates/` → HTML files
- `static/` → CSS, JS, and assets

---

## Key Point

In monolithic architecture:
- ML model, backend logic, and frontend exist in a single codebase.
- Everything is tightly coupled.

