# book-api
Book management REST API using Node.js and Express

# 📚 Book API

A simple RESTful API to manage a list of books using **Node.js** and **Express.js**. This project supports basic **CRUD operations** and uses in-memory storage (no database).

---

## 🚀 Features

- GET all books
- POST a new book
- PUT (update) a book by ID
- DELETE a book by ID
- Validates input and handles errors
- Includes Postman collection for easy testing

---

## 🛠 Technologies Used

- Node.js
- Express.js
- Postman (for API testing)

---

## 📦 Installation & Running Locally

### 1. Clone the repository

```bash
git clone https://github.com/PoolakuntaDakshayani03/book-api.git
cd book-api
#2. Install dependencies
npm install
#3. Start the server
node server.js

Server runs at: http://localhost:3000

#🔗 API Endpoints
#➤ GET /books
Get all books.

#Response Example:
[
  {
    "id": 1,
    "title": "The Hobbit",
    "author": "J.R.R. Tolkien"
  }
]
#➤ POST /books
Add a new book.

#Request Body:
{
  "title": "1984",
  "author": "George Orwell"
}
Response: 201 Created

{
  "id": 2,
  "title": "1984",
  "author": "George Orwell"
}

#➤ PUT /books/:id
Update an existing book by ID.

#Request Body:
{
  "title": "Updated Title",
  "author": "Updated Author"
}
#Response:

{
  "id": 2,
  "title": "Updated Title",
  "author": "Updated Author"
}
#➤ DELETE /books/:id
Delete a book by ID.

{ "message": "Book deleted successfully" }
#❗ Input Validation & Error Handling
If title or author is missing in POST/PUT requests, the API responds with:

{ "message": "Title and author are required." }
If an invalid id is provided, you get:
{ "message": "Book not found." }
#📮 Testing with Postman
Open Postman

Import the file Book-api.postman_collection.json from this repo.

Run the API calls directly from Postman.

##📁 Project Structure

book-api/
├── server.js
├── Book-api.postman_collection.json
├── package.json
├── README.md
🙋‍♀️ Author
Poolakunta Dakshayani










