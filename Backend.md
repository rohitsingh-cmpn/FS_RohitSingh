# FS_RohitSingh
# Student Commute Optimizer-
A full-stack carpooling app that anonymously matches students with similar commuting routes using real-time maps and chat. Helps reduce solo rides, save costs, and build smarter student commutes.
---

## Backend

- **Node.js with Express**  
  Handles multiple concurrent requests efficiently with non-blocking I/O for fast backend operations.

- **PostgreSQL / MongoDB**  
  Efficiently stores and queries route coordinates to quickly find overlapping or nearby routes.

- **PostGIS**  
  PostgreSQL extension adding support for geographic objects and spatial queries.

- **Routing APIs**  
  Google Directions and OpenRouteService provide accurate route calculations for matching student routes precisely.

- **WebSocket Server**  
  Supports real-time communication between users for instant chat functionality.

- **Unique Username Generation Logic**  
  Ensures anonymous, non-duplicable usernames for privacy and identity management.

- **Authentication & Authorization (Firebase Auth / OAuth)**  
  Securely manages user sessions and protects data access while maintaining anonymity.

---

### Backend Diagram

```plaintext
+---------------------------------------------------+
|                   Backend Server                   |
|                (Node.js / Express)                 |
+---------------------------------------------------+
            |                  |                  |
            |                  |                  |
            v                  v                  v
+----------------+   +-------------------+  +------------------+
| Route Matching |   | User Management   |  | Chat Service      |
| (PostGIS +     |   | (Unique usernames,|  | (Socket.IO /      |
| Routing APIs)  |   | Authentication)   |  | Real-time chat)   |
+----------------+   +-------------------+  +------------------+
            |                  
            v                  
+----------------+  
|   Database     |  
| (PostgreSQL +  |  
| PostGIS /      |  
| MongoDB)       |  
+----------------+
