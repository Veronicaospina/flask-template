# Flask App con Docker

Una aplicación Flask simple con plantillas HTML que puede ejecutarse en contenedores Docker.

## Características

- Framework Flask para Python
- Plantillas HTML con Jinja2
- Estilos CSS personalizados
- Configuración Docker completa
- Diseño responsive

## Estructura del Proyecto

```
flask-template/
├── app.py                 # Aplicación principal Flask
├── requirements.txt       # Dependencias de Python
├── Dockerfile            # Configuración de Docker
├── docker-compose.yml    # Configuración de Docker Compose
├── templates/            # Plantillas HTML
│   ├── base.html
│   ├── index.html
│   ├── about.html
│   └── contact.html
└── static/               # Archivos estáticos
    └── css/
        └── style.css
```

## Requisitos Previos

- Docker y Docker Compose instalados
- O Python 3.11+ si quieres ejecutar sin Docker

## Instalación y Ejecución

### Opción 1: Usando Docker Compose (Recomendado)

1. Construir y ejecutar el contenedor:
```bash
docker-compose up --build
```

2. La aplicación estará disponible en: http://localhost:5000

3. Para detener la aplicación:
```bash
docker-compose down
```

### Opción 2: Usando Docker directamente

1. Construir la imagen:
```bash
docker build -t flask-app .
```

2. Ejecutar el contenedor:
```bash
docker run -p 5000:5000 flask-app
```

3. La aplicación estará disponible en: http://localhost:5000


## Rutas Disponibles

- `/` - Página de inicio
- `/about` - Página acerca de
- `/contact` - Página de contacto

## Desarrollo

Para desarrollo con recarga automática, puedes usar:

El volumen está montado, por lo que los cambios en el código se reflejarán automáticamente.

## Notas

- El puerto por defecto es 5000

