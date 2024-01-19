# ToDo App

Este repositorio contiene una aplicación ToDo con un servidor JSON que proporciona datos a través del endpoint http://localhost:3000/todo.

La estructura de los datos en el servidor sigue el siguiente formato:

```
[
  {
    "id": "1490661791287",
    "description": "Definir los pasos para crear ToDo App",
    "done": true
  },
  {
    "id": "1105648123614",
    "description": "Crear un servidor con Node.js y JSON-Server",
    "done": true
  },
  {
    "id": "1115948301283",
    "description": "Crear la base de datos archivo DB.JSON",
    "done": true
  },
  {
    "id": "251210235489",
    "description": "Crear una aplicación con Angular",
    "done": true
  },
  {
    "id": "659936929124",
    "description": "Crear un servicio en Angular para consumir la API",
    "done": false
  }
]
```
## Instrucciones de Configuración

- Clona este repositorio en tu máquina local:
```
git clone https://github.com/tu-usuario/todo-app.git
```

- Navega al directorio del proyecto:
```
cd todo-app
```

- Instala las dependencias necesarias:
```
npm install
```

## Uso
La aplicación ToDo se encuentra en desarrollo y actualmente muestra una lista de tareas con su estado de completado. Puedes interactuar con la API JSON utilizando el endpoint mencionado anteriormente.

### Ejemplo de Uso

- Obtener todas las tareas:
```
GET http://localhost:3000/todo
```

- Obtener una tarea específica por ID:
```
GET http://localhost:3000/todo/{id}
```

- Agregar una nueva tarea:
```
POST http://localhost:3000/todo
```

- Content-Type: application/json
```
{
  "description": "Nueva tarea",
  "done": false
}
```

- Actualizar el estado de una tarea por ID:
```
PATCH http://localhost:3000/todo/{id}
Content-Type: application/json

{
  "done": true
}
```

- Eliminar una tarea por ID:
```
DELETE http://localhost:3000/todo/{id}
```

Recuerda ajustar las solicitudes HTTP según tus necesidades y explorar la aplicación para familiarizarte con su funcionalidad.

¡Disfruta utilizando la aplicación ToDo! Si tienes alguna pregunta o problema, no dudes en crear un problema (issue) en este repositorio.






