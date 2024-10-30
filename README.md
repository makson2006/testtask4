# Spy Cat Agency

## Overview

The **Spy Cat Agency** is a CRUD application designed to manage spy cats, missions, and targets. This application allows users to create and manage spy cats, assign them to missions, and track the progress of those missions as they collect data on various targets.

## Requirements

- Python 3.x
- Django
- Django REST Framework
- PostgreSQL (or your preferred database)

## Installation

### Clone the Repository

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/spy-cat-agency.git
   
API Endpoints
Spy Cats
Create a Spy Cat: POST /api/cats/

Body: { "name": "Cat Name", "years_of_experience": 5, "breed": "Siamese", "salary": 1000 }
Retrieve All Spy Cats: GET /api/cats/

Retrieve a Single Spy Cat: GET /api/cats/{id}/

Update a Spy Cat: PUT /api/cats/{id}/

Body: { "salary": 1200 }
Delete a Spy Cat: DELETE /api/cats/{id}/


Missions
Create a Mission with Targets: POST /api/missions/

Body:
json
{
  "cat": 1,
  "targets": [
    { "name": "Target 1", "country": "USA", "notes": "First target" },
    { "name": "Target 2", "country": "Canada", "notes": "Second target" },
    { "name": "Target 3", "country": "UK", "notes": "Third target" }
  ]
}
Retrieve All Missions: GET /api/missions/

Retrieve a Single Mission: GET /api/missions/{id}/

Update a Mission: PUT /api/missions/{id}/

Delete a Mission: DELETE /api/missions/{id}/


Targets
Create a Target: POST /api/targets/

Body:
json
{
  "mission": 1,
  "name": "Target 1",
  "country": "USA",
  "notes": "First target"
}
Retrieve All Targets: GET /api/targets/

Retrieve a Single Target: GET /api/targets/{id}/

Update a Target: PUT /api/targets/{id}/

Delete a Target: DELETE /api/targets/{id}/


