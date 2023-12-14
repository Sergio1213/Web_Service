# Endpoint: `GET /api/productos/{id}`

Permite obtener información sobre un producto en especifico
## Parámetros de URL
- `{id}` (obligatorio): Identificador único del producto que se requiere identificar.

## Ejemplo de Solicitud
```http
GET /api/productos/1
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 1,
        "attributes": {
            "Titulo": "Camisa street",
            "Descripcion": "Camisas de 100% de algodon",
            "Talla": "Mediana",
            "Precio": 400,
            "stock": 200,
            "Categoria": "algodon",
            "createdAt": "2023-12-09T02:27:36.999Z",
            "updatedAt": "2023-12-09T02:27:37.993Z",
            "publishedAt": "2023-12-09T02:27:37.987Z"
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
