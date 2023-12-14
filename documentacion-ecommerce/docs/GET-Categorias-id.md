# Endpoint: `GET /api/categorias/{id}`

Permite obtener información sobre una categoria en especifico

## Parámetros de URL
- `{id}` (obligatorio): Identificador único de la categoria que se desea recuperar.

## Ejemplo de Solicitud
```http
GET /api/categorias/1
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 1,
        "attributes": {
            "Nombre": "Algodon",
            "Descripcion": "Camisas de 100% de algodon",
            "createdAt": "2023-12-09T02:26:41.065Z",
            "updatedAt": "2023-12-09T02:26:43.947Z",
            "publishedAt": "2023-12-09T02:26:43.943Z"
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
    "error_description": "Ocurrió un problema para procesar la solicitud"
  }
  ``` 
