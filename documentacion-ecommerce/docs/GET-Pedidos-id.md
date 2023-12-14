# Endpoint: `GET /api/pedidos/{id}`

Permite obtener información un pedido en especifico

## Parámetros de URL
- `{id}` (obligatorio): Identificador único del pedido que se desea recuperar.

## Ejemplo de Solicitud
```http
GET /api/pedidos/1
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
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
