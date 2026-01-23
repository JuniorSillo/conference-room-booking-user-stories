# Demo Script – Conference Room Booking System Onboarding

Goal: Show a new developer can clone, run, understand, and test the system in minutes.

1. Open terminal → git clone && cd repo  

2. Show README.md → Highlight Docker Quick Start section  
   ## Docker Quick Start
   ### Docker Prerequisites
   - Docker & Docker Compose installed  
   - Ports 3000 (app), 5432 (DB if exposed) free  

   ### Steps To Run
   docker-compose up --build  
   (Wait for "Server running on port 3000")

   ### Access the Application
   - Swagger UI: http://localhost:3000/api-docs (if implemented)  
   - Or Postman collection for API testing  

   ### Port Explanation
   - 3000: Backend API  
   - (DB port internal via Docker network)

3. Open browser → localhost:3000/api-docs (or paste YAML in editor.swagger.io)  
   → Expand GET /rooms → Try Execute (show list)  
   → POST /bookings → Fill sample → Execute (show 201)

4. Open Postman → Import postman-collection.json from docs/postman  
   → Select mock environment → Run collection → Show all green tests  

5. Browse docs/ folder → Open API_EXAMPLES.md → Copy-paste one curl → Run in terminal  
   → Show real response

