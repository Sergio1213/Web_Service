# Endpoint: `POST /api/categorias`

Permite crear una nueva Categoria

## Parámetros de URL
- `Nombre` (obligatorio): Identificador Para ingresar el nombre de la categoria.
- `Descripcion` (obligatorio): Identificador para ingresar su descripcion.
## Ejemplo de Solicitud
```http
{
    "data":{
        "Nombre":"camisa",
        "Descripcion":"esto es una camisa"
    }

}
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 3,
        "attributes": {
            "Nombre": "camisa",
            "Descripcion": "esto es una camisa",
            "createdAt": "2023-12-14T09:04:53.168Z",
            "updatedAt": "2023-12-14T09:04:53.168Z",
            "publishedAt": "2023-12-14T09:04:53.163Z"
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
