# Endpoint: `POST /api/pedidos`

Permite crear un pedido

## Parámetros de URL
- `user_Id` (obligatorio): Identificador único .
- `"Fecha_pedido` (obligatorio): Fecha en la que se hizo el pedido .
- `Estado` (obligatorio): Estado actual del pedido.


## Ejemplo de Solicitud
```http
POST /api/pedidos

{
    "data":{
        "user_Id":"1",
        "Fecha_pedido":"2023-12-09T15:30:00",
        "Estado":"enviado"
    }

}
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 3,
        "attributes": {
            "user_Id": 1,
            "Fecha_pedido": "2023-12-09T21:30:00.000Z",
            "Estado": "enviado",
            "createdAt": "2023-12-14T09:15:27.138Z",
            "updatedAt": "2023-12-14T09:15:27.138Z",
            "publishedAt": "2023-12-14T09:15:27.136Z"
        }
    },
    "meta": {}
}
```

## Respuestas de Errores Posibles
- Código 404 Not Found:

  ```json
  {
    "errno": 404,
    "error": "not_found",
    
  }
  ```

- Código 500 Internal Server Error:
  ```json
  {
    "errno": 500,
    "error": "internal_error",
   
  }
  ``` 
