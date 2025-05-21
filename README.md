# Proyecto CI/CD con Flask

Este repositorio contiene una aplicación web simple desarrollada con Flask, junto con integración continua y despliegue automático utilizando GitHub Actions y Render.

## Estructura del proyecto

```
.
├── app.py
├── src/
│   └── app.py
├── test_app.py
├── requirements.txt
├── runtime.txt
├── Procfile
├── sonar-project.properties
├── .github/
│   └── workflows/
│       └── pythonapp.yml
└── .gitignore
```

## Descripción

- [`src/app.py`](src/app.py): Código principal de la aplicación Flask.
- [`test_app.py`](test_app.py): Prueba unitaria para la función `index`.
- [`requirements.txt`](requirements.txt): Dependencias del proyecto.
- [`Procfile`](Procfile): Configuración para despliegue en plataformas como Heroku o Render.
- [`runtime.txt`](runtime.txt): Versión de Python utilizada.
- [`sonar-project.properties`](sonar-project.properties): Configuración para análisis de calidad con SonarCloud.
- [`.github/workflows/pythonapp.yml`](.github/workflows/pythonapp.yml): Workflow de GitHub Actions para CI/CD.

## Instalación

1. Clona el repositorio:
   ```sh
   git clone https://github.com/tu-usuario/tu-repo.git
   cd tu-repo
   ```

2. Crea un entorno virtual e instala las dependencias:
   ```sh
   python -m venv venv
   source venv/bin/activate  # En Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

## Ejecución local

```sh
python src/app.py
```

La aplicación estará disponible en [http://localhost:5000](http://localhost:5000).

## Pruebas

Ejecuta las pruebas con pytest:

```sh
pytest
```

## CI/CD

- El workflow de GitHub Actions realiza linting, pruebas y despliegue automático.
- El análisis de calidad se realiza con SonarCloud.
- El despliegue se realiza automáticamente a Render tras pasar las pruebas.

## Licencia

Este proyecto está bajo la licencia MIT.
