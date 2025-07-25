# Lifespan

Lifespan is an open-source application designed to help Plex users efficiently manage their media libraries. It provides powerful tools to set content expiration dates, notify users about expiring media, and automate the deletion of old or unwatched content.

Key Features:

Radarr/Sonarr-style UI: Intuitive table view with search, filtering, and sortable columns for easy media management.

Content Expiration: Assign custom expiration dates or use quick presets (30, 90, 180 days) for media items.

User Notifications: (Simulated) Alert Plex users about content nearing its expiration.

Bulk Actions: Efficiently mark multiple media items for expiration or auto-deletion.

Automated Deletion: (Simulated) Automatically remove expired and marked content to free up storage.

Persistent Storage: Utilizes a Python Flask backend with a SQLite database for reliable data persistence.

Dockerized Deployment: Easy setup and consistent environment with Docker Compose.

Lifespan aims to streamline your media cleanup workflow, ensuring your Plex library remains lean and relevant.
