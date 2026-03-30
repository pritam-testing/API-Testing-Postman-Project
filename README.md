# API Testing Project (Postman)

## 📌 Project Description
This project demonstrates API testing using Postman. It includes CRUD operations and validation of API responses.

## 🛠️ Tools Used
- Postman
- REST API
- JSON

## 🔍 Test Scenarios Covered
- GET request validation
- POST request (Create data)
- PUT request (Update data)
- DELETE request (Remove data)
- Status code validation
- Response body validation

## ▶️ How to Run
1. Open Postman
2. Import the collection JSON file
3. Run all requests


## 🧪 Test Scripts (Postman)

## javascript

// Status Code

pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

// Response Time

pm.test("Response time is less than 500ms", function () {
    pm.expect(pm.response.responseTime).to.be.below(500);
});

// Response Body

pm.test("Response has data", function () {
    var jsonData = pm.response.json();
    pm.expect(jsonData).to.not.be.empty;
});


## 👨‍💻 Author
Pritam Tiwari
