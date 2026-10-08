# Alexandria - Library Management System (Spring MVC + Hibernate + JSP + MySQL)

A modern, production-grade web platform for digital library operations. Members can explore curated catalogs, borrow books with real-time stock management, renew active loans online, and return books with automated late fee calculation. Librarians and administrators have access to an administrative circulation desk and inventory management dashboard.

---

## 🚀 Tech Stack

- **Framework**: Spring Boot 3.3.4 / Spring MVC (Jakarta EE)
- **ORM / Persistence**: Hibernate 6.x / Spring Data JPA
- **View Layer**: JSP & Jakarta JSTL (with Embedded Tomcat Jasper)
- **Database**: MySQL 8.0+ / 9.0+
- **Security & Password Hashing**: Spring Security Crypto (BCrypt)
- **Styling & UI**: Modern Vanilla CSS Design System (Glassmorphism, Dark/Light theme toggle, responsive mobile grid)

---

## 🗄️ Database Configuration

- **Host**: `localhost:3306`
- **Database**: `library_management_db` (Automatically created if not present)
- **Username**: `root`
- **Password**: `Rushi@123`

---

## 🔑 Pre-Seeded Demo Accounts

The application automatically seeds categories, books, and user accounts on initial startup:

| Role | Email | Password | Access Privileges |
| :--- | :--- | :--- | :--- |
| **Administrator / Librarian** | `admin@library.com` | `admin123` | Full Admin Console, Catalog Inventory, Circulation Desk, Member Directory |
| **Patron / Member** | `member@library.com` | `member123` | Book Catalog, 1-Click Borrowing, 14-Day Renewals, Return Processing, History |
| **Patron / Member** | `sarah@library.com` | `member123` | Standard Member Dashboard |

---

## 📖 Key Features

1. **Book Catalog & Smart Search**:
   - Search by title, author, or ISBN.
   - Filter by discipline category (Computer Science, Fiction, Science, Philosophy, Business, History).
   - Filter by "In Stock" availability.
   - Detailed book view with publication metadata and shelf location.

2. **Borrowing Operations (Core)**:
   - 1-Click borrow with instant copy decrement and 14-day loan assignment.
   - Max 5 active borrowed items per member.
   - Duplicate active loan prevention.

3. **Online Renewals**:
   - Renew active loans (+14 days extension from current due date).
   - Maximum 2 online renewals per loan.
   - Automatic lock on overdue loans.

4. **Return & Overdue Fine Engine**:
   - Return books online with instant copy re-stocking.
   - Automatic overdue penalty calculation ($0.50/day late).
   - Fine payment / waiver processing.

5. **Admin Console & Circulation Desk**:
   - Real-time statistics: Total titles, copies, active circulations, overdue alerts, member counts.
   - Catalog Manager: Add new books, edit metadata, +/- adjust physical stock.
   - Circulation Desk: View all active/returned loans, search by borrower or book, process returns, waive fines.
   - Member Directory: View member borrowing status and suspend/activate privileges.

---

## 🛠️ How to Build and Run

### Run using the helper script:
```bash
cd LibraryManagementSystem
./run.sh
```

### Or run directly with Maven:
```bash
mvn spring-boot:run
```

Once started, open your browser and navigate to:
**`http://localhost:8080`**
# Library-Management-System
