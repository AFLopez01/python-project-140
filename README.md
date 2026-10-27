# Juegos mentales

[![hexlet-check](https://github.com/AFLopez01/python-project-140/actions/workflows/hexlet-check.yml/badge.svg)](https://github.com/AFLopez01/python-project-140/actions)

Aprende a configurar el entorno de Python, usar gestores de dependencias y linters, y trabajar con git/GitHub. Adquiere experiencia en arquitectura de aplicaciones y código limpio.

Proyecto de aprendizaje de Códica: https://app.codica.la/programs/python

## Stack

- Python 3.10+
- uv (gestor de paquetes)
- ruff (linter)
- make

## Instalación

Requisitos: Python 3.10 o superior, [uv](https://docs.astral.sh/uv/) y make.

bash
git clone https://github.com/AFLopez01/python-project-140.git
cd python-project-140
make install
make build
make package-install


## Uso

Pantalla de bienvenida y saludo personalizado:

bash
brain-games


Juegos disponibles:

bash
brain-even


## Juegos

### Brain Even (¿Par o impar?)

Se muestra un número aleatorio. Responde yes si es par o no si es impar. Si respondes correctamente tres veces seguidas, ganas; cualquier respuesta incorrecta termina el juego.

[![asciicast](https://asciinema.org/a/Ke9uhaPCj4wrUHgn )

## Estructura del proyecto


brain_games/
├── cli.py          # welcome() y welcome_user()
├── engine.py       # flujo común de cualquier juego
├── games/
│   └── even.py     # lógica propia de cada juego
└── scripts/
    ├── brain_games.py
    └── brain_even.py


## Desarrollo

bash
make lint    # revisar el código con ruff
make clean   # borrar archivos generados


---

<details>
<summary>Pruebas automáticas de Códica</summary>

Las pruebas se ejecutan en cada commit. El archivo .github/workflows/hexlet-check.yml es el responsable de ejecutarlas: no lo elimine ni lo renombre, y no cambie el nombre del repositorio.

</details>

## Acerca de Códica

[Códica](https://app.codica.la/) es una escuela de programación: programas de aprendizaje propios con práctica, apoyo de mentores y proyectos reales que quedan en su currículum. Este repositorio es uno de esos proyectos.