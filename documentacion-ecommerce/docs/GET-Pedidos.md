# Endpoint: `GET /api/pedidos`

Permite obtener información sobre los pedidos



## Ejemplo de Solicitud
```http
GET /api/pedidos
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": [
        {
            "id": 1,
            "attributes": {
                "user_Id": 1,
                "Fecha_pedido": "2023-12-09T06:00:00.000Z",
                "Estado": "enviado",
                "createdAt": "2023-12-09T02:28:29.009Z",
                "updatedAt": "2023-12-09T17:46:42.690Z",
                "publishedAt": "2023-12-09T17:46:42.687Z"
            }
        },
        {
            "id": 2,
            "attributes": {
                "user_Id": 1,
                "Fecha_pedido": "2023-12-09T21:30:00.000Z",
                "Estado": "enviado",
                "createdAt": "2023-12-09T17:49:24.203Z",
                "updatedAt": "2023-12-09T17:49:24.203Z",
                "publishedAt": "2023-12-09T17:49:24.202Z"
            }
        }
    ],
    "meta": {
        "pagination": {
            "page": 1,
            "pageSize": 25,
            "pageCount": 1,
            "total": 2
        }
    }
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

## Notas Adicionales

- Asegurate de incluir un ID válido en la solicitud para obtener la información
  sobre los libros de un tema en específico.
