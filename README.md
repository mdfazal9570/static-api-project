# Static Data APIs (Node.js + Express)

This project implements all 15 requested GET API behaviors using static arrays and separate route files.

## Requirements
- Node.js (LTS recommended)
- npm

## Run the project
Open a terminal in this project folder and run:

```bash
npm install
npm start
```

The server starts at `http://localhost:3000`.

## Test these endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/orders` | All orders |
| GET | `/orders/101` | Order by ID |
| GET | `/users` | All users |
| GET | `/users/Raman` | User(s) by name |
| GET | `/products` | All products |
| GET | `/products/11` | Product by ID |
| GET | `/students` | All students |
| GET | `/students/Ajay` | Student(s) by name |
| GET | `/employees` | All employees |
| GET | `/employees/1` | Employee by ID |
| GET | `/books` | All books |
| GET | `/movies` | All movies |
| GET | `/courses` | All courses |
| GET | `/cities` | All cities |
| GET | `/weather` | All weather reports |

Unknown IDs/names return HTTP `404` with a JSON message. Name searches are case-insensitive. User/student name endpoints return arrays because names may not be unique.

## Folder structure

```text
static-api-project/
├── server.js
├── package.json
├── README.md
└── routes/
    ├── orders.js
    ├── users.js
    ├── products.js
    ├── students.js
    ├── employees.js
    ├── books.js
    ├── movies.js
    ├── courses.js
    ├── cities.js
    └── weather.js
```

You can test the URLs in a browser or Postman after starting the server.
