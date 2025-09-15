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

---
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

---

