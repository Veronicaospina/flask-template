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

- Docker instalado

## Instalación y Ejecución

1. Construir la imagen:
```bash
docker build -t flask-app .
```

2. Ejecutar el contenedor:
```bash
docker run -p 5000:80 flask-app
```

3. La aplicación estará disponible en: http://localhost:5000


## Rutas Disponibles

- `/` - Página de inicio
- `/about` - Página acerca de
- `/contact` - Página de contacto


