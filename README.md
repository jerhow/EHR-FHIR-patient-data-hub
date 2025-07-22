# Patient Data Hub & Visualizer (EHR/FHIR)

## Overview

This will be a full-stack .NET application designed to demonstrate the integration of modern healthcare interoperability standards (FHIR) with cloud services. It will feature a secure API backend that interacts with a managed Azure FHIR Service and a Razor Pages frontend, providing user-friendly data visualizations of synthetic patient health records.

---

## Roadmap

* **FHIR Data Integration:** Ingest and retrieve standardized healthcare data using the FHIR R4 specification.
* **Secure RESTful API:** A secure backend API built with ASP.NET Core.
* **Patient Data Visualization:** A web interface to display patient demographics, medications, and chart key observations over time.
* **Cloud-Native Architecture:** Utilizing Azure PaaS services for data, hosting, and security.
* **Automated Deployments:** A CI/CD pipeline built with GitHub Actions automates building, testing, and deploying the application to Azure.
* **Unit Testing:** Verify key backend components with unit tests using xUnit and Moq.

---

## Technology Stack

* **Backend:** C# / .NET 8, ASP.NET Core Web API
* **Frontend:** ASP.NET Core Razor Pages, Chart.js for visualizations
* **Healthcare Standard:** FHIR R4
* **Azure Services:**
    * Azure Health Data Services (FHIR Service)
    * Azure App Service
* **DevOps:** GitHub Actions for CI/CD
* **Unit Testing:** xUnit, Moq
* **Data:** Synthea for synthetic patient data generation

---

## Architecture

The plan is to use a decoupled architecture consisting of a frontend Web App and a backend API. The API will serve as a secure gateway to the Azure FHIR Service, which will act as the persistence layer for all electronic health record data.

---

## Getting Started

### Prerequisites (as currently known)

* .NET 8 SDK
* Git
* Synthea (for data generation)
* Azure subscription (for resource deployment)

### Configuration

*Instructions for setting up User Secrets for both the API and Web App projects will be detailed here.*

### Running Locally

*Instructions for running both the API and Web App projects locally will be provided here.*

---

## Deployment

Continuous integration and deployment to be handled by a GitHub Actions workflow. Pushes to the `main` branch will trigger a workflow that builds, tests, and deploys both the API and Web App to their respective Azure App Services.

---

## Future Enhancements (extended roadmap)

* Integration of additional FHIR resources (e.g., `AllergyIntolerance`, `Condition`).
* Implementation of user accounts and authentication.
* More advanced data filtering and reporting capabilities.
