# Endpoint: `GET /api/productos`

Permite obtener información sobre los productos


## Ejemplo de Solicitud
```http
GET /api/productos
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": [
        {
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
        {
            "id": 2,
            "attributes": {
                "Titulo": null,
                "Descripcion": null,
                "Talla": null,
                "Precio": null,
                "stock": 100,
                "Categoria": null,
                "createdAt": "2023-12-09T17:41:27.687Z",
                "updatedAt": "2023-12-09T17:41:27.687Z",
                "publishedAt": "2023-12-09T17:41:27.682Z"
            }
        },
        {
            "id": 3,
            "attributes": {
                "Titulo": "camisa",
                "Descripcion": "esto es una camisa",
                "Talla": "mediana",
                "Precio": 200,
                "stock": 100,
                "Categoria": "algodon",
                "createdAt": "2023-12-09T17:42:25.877Z",
                "updatedAt": "2023-12-09T17:42:25.877Z",
                "publishedAt": "2023-12-09T17:42:25.874Z"
            }
        }
    ],
    "meta": {
        "pagination": {
            "page": 1,
            "pageSize": 25,
            "pageCount": 1,
            "total": 3
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
