# Lifespan: Your Smart Plex Media Cleaner

Lifespan is an open-source application designed to help Plex users efficiently manage their media libraries. It provides powerful tools to set content expiration dates, notify users about expiring media, and automate the deletion of old or unwatched content.

-----

## Features

Lifespan is built around the following core functionalities:

  * **Plex Library Integration (Simulated):** Load and display content from your Plex libraries. (Currently simulated; future plans include direct Plex API integration).
  * **Content Expiration:** Assign custom expiration dates to individual or multiple media items.
  * **User Notification (Simulated):** Alert Plex users about content nearing its expiration date.
  * **Bulk Actions:** Efficiently select and apply actions (like setting expiration dates or marking for auto-deletion) to multiple media items.
  * **Automated Deletion (Simulated):** Automatically remove expired and marked content to free up storage space.
  * **Radarr/Sonarr-style UI:** An intuitive, data-rich table view with search, filtering, and sortable columns for streamlined media management.
  * **Quick Date Presets:** Easily set expiration dates to 30, 90, or 180 days from the current date.

-----

## Architecture

Lifespan is built with a modern, containerized architecture:

  * **Frontend:** React.js for a dynamic and responsive user interface.
  * **Backend:** Python Flask providing RESTful API endpoints for data management.
  * **Database:** SQLite for persistent storage of library and media item data.
  * **Containerization:** Docker and Docker Compose for easy deployment and environment consistency.

-----

## Getting Started

To get Lifespan up and running using Docker Compose:

1.  **Clone the repository:**

    ```bash
    git clone [YOUR_REPOSITORY_URL]
    cd lifespan
    ```

2.  **Adjust API URL (if necessary):**
    Open `frontend/src/App.js` and ensure the `API_BASE_URL` is set correctly for Docker Compose:

    ```javascript
    const API_BASE_URL = 'http://backend:5000/api';
    ```

3.  **Build and run the services:**
    Navigate to the root directory of the cloned repository (where `docker-compose.yml` is located) and run:

    ```bash
    docker-compose up --build
    ```

    This command will build the Docker images for both the backend and frontend, and then start the containers.

4.  **Access the application:**
    Once the services are running, open your web browser and navigate to: `http://localhost:3000`

-----

## Future Work

  * Real Plex API Integration: Connect to a live Plex server for actual library data and user watch history.
  * Actual Email Sending: Integrate with an email service to send genuine notifications.
  * Physical Media Deletion: Implement logic to physically remove media files from the server.
  * Scheduled Background Tasks: Set up automated tasks for periodic expiration checks and deletions.
  * User Authentication and Authorization: Implement secure user login.

-----

## License

This project is licensed under the MIT License.
