# 📚 Book Management System – Java Web Application

This is a simple, responsive **Book Management System** built using **Java (JSP & Servlets), JDBC, and MySQL**. It allows users to manage book records efficiently through a web interface.

---

## 🌟 Features

- ✅ Add a new book with ID, Name, Author, Description, and Price
- 📖 View all books in a stylish table layout
- 📝 Update book details
- ❌ Delete books by ID
- 🎨 Aesthetic, responsive UI using internal CSS and background images
- 🔒 Clean separation of concerns using Servlets, DAO, and JSPs

---

## 🛠️ Tech Stack

| Layer         | Technology       |
|--------------|------------------|
| Frontend     | HTML, CSS, JSP    |
| Backend      | Java (Servlets)   |
| Database     | MySQL             |
| Connection   | JDBC              |
| Server       | Apache Tomcat     |

---

## 📂 Project Structure

book-management-system/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/
│       │       └── bookapp/
│       │           ├── controller/
│       │           │   └── BookController.java        # Handles web requests
│       │           ├── service/
│       │           │   ├── BookService.java           # Interface
│       │           │   └── BookServiceImpl.java       # Business logic implementation
│       │           ├── repository/
│       │           │   └── BookRepository.java        # Extends JpaRepository
│       │           ├── entity/
│       │           │   └── Book.java                  # Entity mapped to DB
│       │           └── BookManagementApplication.java # Main Spring Boot class
│       └── resources/
│           ├── templates/
│           │   ├── home.html                          # Home Page (Thymeleaf)
│           │   ├── addBook.html                       # Form to add book
│           │   ├── viewBooks.html                     # Displays all books
│           │   └── success.html                       # Confirmation page
│           ├── static/
│           │   ├── css/
│           │   │   └── style.css
│           │   └── images/
│           └── application.properties                 # DB config, port, etc.
├── README.md
├── LICENSE
└── pom.xml                                             # Maven dependencies


---

## ⚙️ How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/purvaa-12/book-management-system.git

Import into IDE:

Open Eclipse or NetBeans.

Import the project as a dynamic web project.

Set up MySQL:

Create a booksdb database.

Create a books table with appropriate columns.

Update DB credentials in BookDAO.java.

Deploy to Tomcat:

Run the project on Apache Tomcat.

Visit: http://localhost:8080/book-management-system/home.jsp

