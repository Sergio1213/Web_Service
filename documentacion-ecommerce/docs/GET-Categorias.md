# Endpoint: `GET /api/categorias`

Permite obtener información sobre todas las categorias



## Ejemplo de Solicitud
```http
GET /api/categorias
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": [
        {
            "id": 1,
            "attributes": {
                "Nombre": "Algodon",
                "Descripcion": "Camisas de 100% de algodon",
                "createdAt": "2023-12-09T02:26:41.065Z",
                "updatedAt": "2023-12-09T02:26:43.947Z",
                "publishedAt": "2023-12-09T02:26:43.943Z"
            }
        },
        {
            "id": 2,
            "attributes": {
                "Nombre": "camisa",
                "Descripcion": "esto es una camisa",
                "createdAt": "2023-12-09T17:44:57.480Z",
                "updatedAt": "2023-12-09T17:44:57.480Z",
                "publishedAt": "2023-12-09T17:44:57.479Z"
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
    "error_description": "Ocurrió un problema para procesar la solicitud"
  }
  ``` 

