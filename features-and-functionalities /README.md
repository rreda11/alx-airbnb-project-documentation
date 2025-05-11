## 🏠 Airbnb Clone – Backend Features & Functionalities

This project is a backend system for an Airbnb-like booking platform. Below is a detailed breakdown of the features and modules it supports:

---

### 1. 👤 User Management

#### 🔐 Authentication & Authorization
- Secure user registration and login
- Password hashing and JWT-based authentication
- Role-based access: `guest`, `host`, and `admin`
- Email uniqueness and validation
- Password reset/recovery functionality

#### 📝 Profile Management
- View and update profile info (name, email, phone)
- View user’s own bookings (guest) or properties (host)

---

### 2. 🏡 Property Management

#### For Hosts:
- Create new property listings with name, description, location, price per night
- Update or delete listings
- Manage listings linked to the host's account

#### For Guests:
- View property listings with search and filter options

---

### 3. 📅 Booking System

- Create bookings for specific date ranges
- Prevent double booking via date conflict checks
- Booking statuses: `pending`, `confirmed`, `canceled`
- Guests can cancel their own bookings (based on policy)
- Hosts can confirm or reject bookings
- View current and past bookings

---

### 4. 💳 Payment Integration

- Link payment records to confirmed bookings
- Track amount paid, method used, and timestamp
- Payment methods supported: `credit_card`, `paypal`, `stripe`
- Store payment metadata (for admin/audit purposes)

---

### 5. ⭐ Reviews & Ratings

- Guests can submit a review and a 1–5 star rating after a stay
- Hosts can view property feedback
- Admin can moderate or delete reviews if needed

---

### 6. 💬 Messaging System

- Guests and hosts can send messages to each other
- Messages include a timestamp (`sent_at`)
- Only accessible to sender and recipient
- Can be linked to specific bookings or properties for context

---

### 7. 🛠️ Admin Capabilities

- View, update, or remove any user, property, or booking
- Modify user roles (guest, host, admin)
- Moderate reviews and messages for abusive content
- Full access to audit logs and platform stats (future feature)

---

### 8. ⚙️ Technical Enhancements

- UUIDs used as primary keys for scalability
- Indexing on email, booking_id, property_id for performance
- Support for pagination and filtering on API responses
- Optional integration for Redis (caching) and Celery (async tasks)

---

### 9. 🧪 API Documentation & Testing

- Swagger/OpenAPI documentation available
- Postman collection for endpoint testing
- Unit & integration test coverage for all major services
- CI/CD ready (GitHub Actions or similar pipeline support)

---

![Screenshot](image.png)

