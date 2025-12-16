

# **Smart India Hackathon (SIH) – Workshop Submission **

## **Problem Title**

**SIH 1710: Enhancing Navigation for Railway Station Facilities and Locations**

## **Problem Creator’s Organization**

**Ministry of Railways, Government of India**


## **1. Idea**

Railway stations fail passengers not because information is missing, but because it is **scattered, static, and context-blind**. Boards show everything. Passengers need *only what matters to them, right now*.

The proposed solution, **RailGuide-X**, is a **context-aware station navigation and guidance system** that dynamically adapts navigation instructions based on **passenger intent, time constraints, crowd conditions, and station operations**.

Instead of asking users to “search” endlessly, RailGuide-X predicts intent:

* Catching a train
* Finding amenities
* Transferring platforms
* Exiting the station quickly

The system then delivers **priority-based navigation**, not just shortest paths. The result is reduced congestion, fewer missed connections, and smoother passenger flow.



## **2. Proposed Solution / Architecture**
<img width="1147" height="522" alt="image" src="https://github.com/user-attachments/assets/a50f5567-9180-4e91-9b8e-5652dd2035dd" />

### **Core Principle**

Navigation should adapt to **station reality**, not fixed maps.

### **System Flow**

1. **Passenger Interaction Layer**

   * Mobile application
   * Station-installed kiosks
   * Voice-only mode for accessibility

2. **Intent Detection Module**

   * Travel timing (departure/arrival window)
   * Selected service (platform, restroom, exit, food)
   * Passenger category (elderly, disabled, general)

3. **Context Engine**

   * Real-time crowd load
   * Platform changes
   * Temporary route restrictions
   * Emergency signals

4. **Dynamic Routing Engine**

   * Time-aware routing
   * Congestion-avoidance paths
   * Accessibility-compliant routes
   * Priority overrides for emergencies

5. **Information Synchronization Layer**

   * Station control systems
   * Facility management updates
   * Public announcement triggers

6. **Operations & Analytics Console**

   * Crowd movement visualization
   * Route efficiency metrics
   * Incident response control



## **3. Use Cases**

<img width="576" height="781" alt="image" src="https://github.com/user-attachments/assets/2208f2b4-6773-4df9-8bd9-2bb236aca67a" />

### **Passenger-Oriented Use Cases**

* “Fastest path to Platform 6 with minimal crowd”
* “Wheelchair-accessible route to exit”
* “Nearest restroom with low footfall”
* “Voice-guided navigation in regional language”
* “Emergency exit guidance during alerts”

### **Railway Operations Use Cases**

* Redirect passenger flow during platform changes
* Temporarily block routes digitally without physical barriers
* Identify underutilized station areas
* Reduce congestion using dynamic routing

### **Staff & Emergency Use Cases**

* Real-time evacuation routing
* Priority routing for medical emergencies
* Live passenger density alerts



## **4. Technology Stack (Alternative & Practical)**

### **Client Interfaces**

* **Flutter** (Single codebase for Android + Kiosks)
* **Progressive Web App (PWA)** for low-end devices
* **Text-to-Speech APIs** for voice guidance

### **Backend & APIs**

* **Java Spring Boot** (Scalable, railway-grade backend)
* **PostgreSQL** (Station topology & services)
* **Apache Kafka** (Real-time event streaming)

### **Intelligence Layer**

* **Python (FastAPI)** for intent prediction
* **Rule-based + ML hybrid routing**
* **Graph-based navigation engine**

### **Localization & Context Sources**

* Bluetooth beacons
* QR markers at decision points
* Wi-Fi signal strength mapping

### **Security & Access**

* OAuth 2.0
* Role-based dashboards for admins and operators

### **DevOps & Tools**

* Git
* Docker
* Grafana (monitoring)
* Figma (UX design)


## **5. Dependencies & Timeline**

| Activity                        | Duration |
| ------------------------------- | -------- |
| Station topology mapping        | 7 days   |
| Context & crowd data modeling   | 8 days   |
| Routing engine development      | 9 days   |
| UI/UX and accessibility testing | 6 days   |
| System integration              | 5 days   |
| Field simulation & validation   | 5 days   |

**Total Duration:** ~40 days


## **6. Budget Estimation**

| Component                  | Cost (INR) |
| -------------------------- | ---------- |
| Beacon & QR infrastructure | ₹14,000    |
| Cloud hosting & APIs       | ₹16,000    |
| Development & testing      | ₹15,000    |
| Risk buffer                | ₹5,000     |

**Total Estimated Budget:** **₹50,000**



## **7. Why This Solution Is Different**

* Focuses on **intent-based navigation**, not static maps
* Integrates passenger needs with **station operations**
* Reduces congestion without physical restructuring
* Works even on **low-end smartphones**
* Improves safety during peak hours and emergencies

