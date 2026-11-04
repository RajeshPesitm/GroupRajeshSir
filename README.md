# GroupRajeshSir
# Agriculture Online Market 🌾🚜

**Agriculture Online Market** is a full-stack e-commerce web application designed to bridge the gap between local farmers and consumers/wholesalers. The platform allows farmers to showcase and sell their fresh produce directly to customers, enabling fair pricing, reducing middleman intervention, and giving buyers access to high-quality agricultural goods.

---

## 📝 Abstract

Modern agricultural supply chains often suffer from fragmentation, leaving farmers dependent on local middlemen who take a significant cut of the profits. **Agriculture Online Market** eliminates these intermediaries by offering a direct-to-consumer digital marketplace. 

Farmers can register, manage digital inventories of their seasonal produce, and control their pricing based on real-time market demands. Buyers (individual households or commercial wholesalers) can seamlessly browse local fresh produce, filter items by category or location, and securely place orders. By streamlining communication and logistics data, this application enhances profit margins for rural producers while lowering costs and improving freshness for urban consumers.

---

## 🛠️ Tech Stack

| Layer | Technology | Description |
| :--- | :--- | :--- |
| **Frontend** | Vanilla HTML5, CSS3, JavaScript (ES6+) | Clean, lightweight UI built without heavy frameworks to ensure fast loading speeds and high accessibility. Uses Fetch API for asynchronous backend communication. |
| **Backend** | Spring Boot 3.x, Spring Data JPA, Spring Security | Enterprise-grade Java framework managing the business logic, RESTful API routing, and system security. |
| **Database** | Oracle SQL / Oracle Database | Relational database handling complex transactional data, integrity constraints, and scalable storage for users, products, and invoices. |
| **Build Tool** | Maven | Dependency management and automated application build lifecycle. |

---

## 📋 System Requirements

### ⚙️ Functional Requirements
Functional requirements define the core actions and operations the application must perform for its users.

#### 1. User Management & Authentication
* **Registration & Login:** Users must be able to register and log in securely as either a **Farmer** or a **Buyer**.
* **Profile Management:** Users can update their contact details, delivery addresses, and farm/business descriptions.

#### 2. Farmer Inventory & Produce Management
* **Product Listing:** Farmers must be able to add, update, or remove crops, fruits, and vegetables with details (name, category, price per kg/quintal, available stock quantity, and product images).
* **Stock Management:** The system must automatically deduct product stock quantities upon successful order generation.

#### 3. Buyer Marketplace & Checkout
* **Browse & Search:** Buyers can view all live agricultural listings and filter produce by category, price, or location.
* **Shopping Cart:** Buyers must be able to add multiple items from different farmers to a persistent shopping cart, edit quantities, and view a price breakdown.
* **Order Placement:** A checkout system that processes orders, calculates totals, and logs delivery information.

#### 4. Order Tracking & History
* **Farmer Dashboard:** Farmers can view incoming orders, update order status (e.g., *Pending, Dispatched, Delivered*), and track total earnings.
* **Buyer Dashboard:** Buyers can view past order history and monitor the active status of their pending shipments.

---

### 🛡️ Non-Functional Requirements
Non-functional requirements specify the quality attributes, operational limits, and performance metrics of the system.

* **Performance & Latency:** API endpoints must process requests quickly, ensuring that the marketplace catalog loads within less than 2 seconds under normal network conditions.
* **Data Consistency & Integrity:** Using Oracle SQL's ACID transactions, the database must prevent race conditions (e.g., two buyers purchasing the exact same stock allocation simultaneously).
* **Scalability:** The Spring Boot backend architecture must remain stateless to easily support horizontal scaling as the user base grows.
* **Security:** Data passwords must be securely hashed before storage in the Oracle DB, and session tokens/cookies must protect unauthorized access to dashboard routes.
* **Usability & Accessibility:** The Vanilla HTML/CSS frontend must be fully responsive, offering a seamless user experience across mobile phones, tablets, and desktop monitors.

