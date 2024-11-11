# 📚 **BookVerse: The Library Navigator**

**BookVerse** is an interactive **Library Management System** designed to manage a collection of self-help and fiction books. This project, implemented in Python, allows users to search, borrow, and reserve books, track overdue items, and receive personalized book recommendations. The system is intended to be run in **Google Colab** for ease of access and testing.

---

## **Features**

- **Inventory Management**: Admins can add, remove, and search for books.
- **Borrowing and Returning**: Users can borrow books with due dates and receive overdue alerts.
- **User Registration and Login**: Supports multiple user roles with secure login.
- **Reservations**: Allows users to reserve books if all copies are borrowed.
- **Personalized Recommendations**: Suggests books based on recent borrowing history.
- **Statistics Dashboard**: Provides insights into popular books and active users.

---

## **Project Structure**

The project consists of the following main components:

- **Data Collections**:
  - `books`: Contains a list of dictionaries, each representing a book with details like title, author, genre, and availability.
  - `users`: A dictionary of registered users with attributes such as name, role, and borrowing history.
  - `transactions`: Records of all book borrowing and returning transactions, including due dates and overdue status.

- **Core Functions**:
  - `find_book_by_id()`: Locates a book by its ID.
  - `find_user_by_id()`: Retrieves a user by their ID.
  - `add_book()`, `remove_book()`, `search_book()`: Functions for managing the book inventory.
  - `borrow_book()`, `return_book()`: Manages borrowing and returning processes with overdue tracking.
  - `reserve_book()`: Allows users to reserve a book when no copies are available.
  - `recommend_books()`: Suggests books in the same genre as the user’s last borrowed book.
  - `most_borrowed_books()`, `most_active_users()`: Provides statistics on popular books and active users.

- **User Interaction**:
  - The `user_interaction()` function serves as the main interface, enabling users to navigate options, login, and perform actions like searching, borrowing, and managing books.

---

## **How to Use**

### **Requirements**

- Python 3.x
- Google Colab (recommended for running and testing the code)

### **Running the Program**

1. **Open Google Colab** and create a new notebook.
2. Copy and paste the code into a code cell in Colab.
3. Run the code cell to initialize the library management system.
4. Follow the on-screen prompts to interact with the system.

### **Testing and Example Use Cases**

The program supports the following user actions:

#### **1. Registering and Logging In**
- Users can register with unique IDs and passwords and log in to access the system.

#### **2. Searching for a Book**
   - Enter the title of the book to view its details, including availability and genre.

#### **3. Borrowing a Book**
   - Users can borrow books if available, and due dates are set automatically.

#### **4. Returning a Book**
   - Return borrowed books and check if they are overdue.

#### **5. Reserving a Book**
   - Reserve a book if no copies are available, and receive notification when it becomes available.

#### **6. Book Recommendations**
   - Get book recommendations in the same genre as your last borrowed book.

#### **7. View Statistics (Admin Only)**
   - Admins can view statistics on the most borrowed books and the most active users.

---

## **Future Improvements**

- **Database Integration**: Migrate data to a database like SQLite or PostgreSQL for persistent storage.
- **Real-Time Notifications**: Implement email notifications for overdue and reserved books.
- **Enhanced UI**: Convert this console-based system to a web app using Flask for a better user experience.

---

## **Acknowledgments**

This project was developed with assistance from ChatGPT for code structure, suggestions, and debugging. All logic and implementation have been adapted and customized for this project.
