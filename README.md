# FS_RohitSingh  
# Student Commute Optimizer  
A full-stack carpooling app that anonymously matches students with similar commuting routes using real-time maps and chat. Helps reduce solo rides, save costs, and build smarter student commutes.

---

## Frontend

- **React**  
  Fast, reusable UI components with virtual DOM for efficient updates and interactive features.

- **Mapbox GL JS / Google Maps API**  
  Provides smooth, customizable maps with route drawing and proximity features.

- **Debouncing Input**  
  Limits API calls while typing locations, reducing server load and improving responsiveness.

- **Lazy Loading**  
  Loads heavy components (maps, chat) only when needed, speeding up initial page load.

- **WebSockets**  
  Enables real-time, low-latency chat without page refreshes for instant messaging experience.

- **Redux (State Management)**  
  Efficiently manages app data and reduces unnecessary re-renders for better performance.

---

### Frontend Diagram

```plaintext
+------------------------------------+
|         Student Interface           |
|      (React / React Native App)    |
+------------------------------------+
               |
       +-------+--------+
       |                |
       v                v
+--------------+  +-----------------+   +------------------+
| Location     |  | Map Display     |   | Chat Interface   |
| Input        |  | (Route + Nearby)|   | (Real-time chat) |
| (Home +      |  +-----------------+   +------------------+
| Destination) |          
+--------------+
       |                |               |
       +----------------+---------------+
                        |
                        v
              +--------------------+
              | State Management    |
              | (React Context /    |
              | Redux)             |
              +--------------------+
                        |
                        v
              +--------------------+
              | Backend API Calls   |
              | (Routes, Users,     |
              | Matches, Chat)      |
              +--------------------+
Backend

Node.js with Express
Handles multiple concurrent requests efficiently with non-blocking I/O for fast backend operations.

PostgreSQL / MongoDB
Efficiently stores and queries route coordinates to quickly find overlapping or nearby routes.

PostGIS
PostgreSQL extension adding support for geographic objects and spatial queries.

Routing APIs
Google Directions and OpenRouteService provide accurate route calculations for matching student routes precisely.

WebSocket Server
Supports real-time communication between users for instant chat functionality.

Unique Username Generation Logic
Ensures anonymous, non-duplicable usernames for privacy and identity management.

Authentication & Authorization (Firebase Auth / OAuth)
Securely manages user sessions and protects data access while maintaining anonymity.


