`# Express REST API APP

## Setup Instructions

1. Open the file in an IDE (e.g., VScode)
2. Install dependencies:
   ```
   npm install
   ```
3. Start the server:
   ```
   npm start
   ```
4. API will run on `http://localhost:3000`

---

## API Endpoints

### Root
- **GET /**  
Returns "Hello, World!"

### Items CRUD
- **GET /items**  
Retrieve all items

- **GET /items/:id**  
Retrieve item by ID

- **POST /items**  
Create new item (JSON body required)

- **PUT /items/:id**  
Update item by ID

- **DELETE /items/:id**  
Delete item by ID

---

## Example Postman Requests

### 1. Get All Items
```
GET http://localhost:3000/items
```

### 2. Get Single Item
```
GET http://localhost:3000/items/1
```

### 3. Create Item
```
POST http://localhost:3000/items
Content-Type: application/json

{
  "name": "Item 3",
  "description": "Third item"
}
```

### 4. Update Item
```
PUT http://localhost:3000/items/1
Content-Type: application/json

{
  "name": "Updated Item",
  "description": "Updated description"
}
```

### 5. Delete Item
```
DELETE http://localhost:3000/items/1
```

---

## Error Responses

- **404** Item or route not found
- **400** Missing required fields
- **500** Internal server error

