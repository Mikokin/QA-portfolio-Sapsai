<h1>API Testing Report — Swagger Petstore</h1>

<h2>Описание</h2>

Проект демонстрирует навыки тестирования API на примере **Swagger Petstore API**:  

https://petstore.swagger.io/v2

<h2>Проверенные эндпоинты</h2>

<table>
  <thead>
    <tr>
      <th>Endpoint</th>
      <th>Метод</th>
      <th>Описание</th>
      <th>Результат</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>/pet</td>
      <td>POST</td>
      <td>Добавление нового питомца</td>
      <td>Passed</td>
    </tr>
    <tr>
      <td>/pet/{petId}</td>
      <td>GET</td>
      <td>Получение питомца по ID</td>
      <td>Passed</td>
    </tr>
    <tr>
      <td>/pet/{petId}</td>
      <td>DELETE</td>
      <td>Удаление питомца</td>
      <td>Passed</td>
    </tr>
    <tr>
      <td>/pet/findByStatus</td>
      <td>GET</td>
      <td>Получение питомца по статусу</td>
      <td>Passed</td>
    </tr>
  </tbody>
</table>


<h2>Примеры ответов</h2>

- POST /pet → 200 OK, JSON с id, name, status 
- GET /pet/{petId} → 200 OK, JSON с тем же id
- DELETE /pet/{petId} → 200 OK, message: petId
- GET /pet/findByStatus → 200 OK, JSON со статусами питомцев

<h2>Вывод</h2>

Все ключевые эндпоинты работают корректно.  

API стабильно возвращает коды и структуру JSON в соответствии с документацией Swagger Petstore.
