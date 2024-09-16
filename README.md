# task2-hactiv8

Create Global Variable dengan variable baseUrl to generate website  https://jsonplaceholder.typicode.com/
Create new object repository Web Service Request for GET , POST, DELETE
Input URL pada repo GET -> ${GlobalVariable.baseUrl}/todos?userId=1&completed=false (GET data todos dengan spesifikasi userId = 1 dan status completed = false)
Input URL pada repo POST -> ${GlobalVariable.baseUrl}/todos (Create data todos)
Input URL pada repo DELETE -> ${GlobalVariable.baseUrl}/todos/completed=false (DELETE data todos berstatus completed = false)
RUN masing2 repo dengan response 200,201
Create new test case GET, POST, DELETE
Gunakan function -> def slurper = new groovy.json.JsonSlurper(); def result = slurper.parseText(getResponse.getResponseBodyContent())
Add assert pada test case dan deklarkan semua komponen pada data sesuai dengan type data 
print respon 
