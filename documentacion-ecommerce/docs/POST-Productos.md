# Endpoint: `POST /api/productos`

Permite ingresar un nuevo prodcuto

## Parámetros de URL
- {Titulo} (obligatorio)
- - {Descripcion} (obligatorio)
- - {Talla} (obligatorio)
- - {Precio} (obligatorio)
- - {stock} (obligatorio)
- - {Categoria} (obligatorio)
## Ejemplo de Solicitud
```http
POST /api/productos
{
    "data":{
        "Titulo":"camisa",
        "Descripcion":"esto es una camisa",
        "Talla":"mediana",
        "Precio":"200",
        "stock":"100",
        "Categoria":"algodon"
    }

}
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 5,
        "attributes": {
            "Titulo": "camisa",
            "Descripcion": "esto es una camisa",
            "Talla": "mediana",
            "Precio": 200,
            "stock": 100,
            "Categoria": "algodon",
            "createdAt": "2023-12-14T09:25:51.736Z",
            "updatedAt": "2023-12-14T09:25:51.736Z",
            "publishedAt": "2023-12-14T09:25:51.735Z"
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
