📌 README.md
md
Copy
Edit
# 🏗️ Spring Boot Thread-Safe TTL Cache API

This repository provides a **Spring Boot starter project** for implementing a **Thread-Safe In-Memory Cache with TTL (Time-To-Live) Eviction**.

---

## **🛠️ Installation & Setup**
### **1️⃣ Prerequisites**
Ensure you have the following installed:
- **Java 17+** → [Download JDK](https://adoptium.net/)
- **Maven** → [Install Maven](https://maven.apache.org/install.html)
- **Git** → [Install Git](https://git-scm.com/)
- An API testing tool like **Postman** or **cURL**

### **2️⃣ Clone the Repository**
```sh
git clone https://github.com/BUNara/JavaTTLCache.git
cd JavaTTLCache
### **3️⃣ Build the Project**
sh
Copy
Edit
mvn clean install
### **4️⃣ Run the Spring Boot Application**
sh
Copy
Edit
mvn spring-boot:run
By default, the API will be available at:

arduino
Copy
Edit
http://localhost:8080
## **📌 Task Overview**
Your task is to implement a thread-safe in-memory cache that supports:
1️⃣ Storing key-value pairs
2️⃣ Retrieving values from the cache
3️⃣ Automatically expiring cache entries after a specified TTL (Time-To-Live)
4️⃣ Exposing REST API endpoints to interact with the cache

## **📌 Requirements**
The cache should be thread-safe and handle concurrent access.
Entries should expire automatically after 60 seconds.
The cache should be accessible via a REST API with the following endpoints:
API Endpoints
Method	Endpoint	Description
PUT	/cache/{key}	Stores a value in the cache
GET	/cache/{key}	Retrieves a value (returns 404 if expired)
DELETE	/cache/{key}	Removes a value from the cache
📂 Project Structure
bash
Copy
Edit
JavaTTLCache/
│── src/main/java/com/example/ttlcache/
│   ├── CacheService.java      # Implement your caching logic here
│   ├── CacheController.java   # Implement API endpoints here
│── src/main/resources/
│   ├── application.properties # Configuration settings (optional)
│── pom.xml                    # Maven dependencies
│── README.md                   # Instructions for candidates
📩 Submitting Your Solution
Fork this repository.
Implement your solution in CacheService.java and CacheController.java.
Push your changes and share the GitHub repo link.
## **📌 Notes**
You can use any approach to ensure thread safety and TTL expiration.
Follow REST API best practices.
The correctness, performance, and maintainability of your solution will be evaluated.
## **🚀 Good luck! Looking forward to your implementation!**
