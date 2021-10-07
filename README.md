## Тестовое задание для Райффайзенбанка.
Приложение написано на Spring boot.
В качестве бд использовалась PostegreSQL.
Развернуто в докер контейнере вместе с бд, которая недоступна снаружи контейнера.

API:

  Возвращает общее количество носков на складе, соответствующих переданным в параметрах критериям запроса.
  
  GET /api/socks : http://94.130.53.21:8082/api/socks
  
  Пример запроса: 
  
       http://94.130.53.21:8082/api/socks?color=red&operation=equal&cottonPart=20
       
  Регистрирует приход носков на склад.
  
  POST /api/socks/income : http://94.130.53.21:8082/api/socks/income
  
  
  Пример тела запроса: 
  
     {
        "color": "red",
        "cottonPart": 20,
        "quantity": 12
     } 
     
  Регистрирует отпуск носков со склада.
  
  POST /api/socks/outcome : http://94.130.53.21:8082/api/socks/outcome
  Пример тела запроса: 
  
     {
        "color": "red",
        "cottonPart" : 20,
        "quantity" : 12
     } 
     
  Для связи:  https://t.me/Kurtliketeenspirit
