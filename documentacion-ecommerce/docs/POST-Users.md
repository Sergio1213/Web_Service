# Endpoint: `POST /api/users`

Permite registrar un nuevo usuario

## Parámetros de URL
- `{username}` (obligatorio)
- `{email}` (obligatorio)
- `{password}` (obligatorio)
- `{role}` (obligatorio)


## Ejemplo de Solicitud
```http
POST /api/users
{
        "username":"pruebaaaaaaa",
        "email":"email@gmail.commmm",
        "password":"hola123",
        "role":"public"
}
   
```

## Respuesta Exitosa (Código 200 OK)
```json
{
    "data": {
        "id": 3,
        "attributes": {
            "username": "pruebaaaaaaa",
            "email": "email@gmail.commmm",
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

  }
  ``` 
