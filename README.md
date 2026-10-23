# Proyecto: Calculadora de Área Modular y Diana ASCII — LPR 2026

**Escuela de Educación Secundaria Técnica N° 1 — Vicente López**  
**Curso:** 5° Año 3° División — Especialidad Informática / Programación  
**Materia:** Laboratorio de Programación (LPR)  
**Profesor:** Prof. York Mansilla Muñoz  
**Estudiante:** Alexander Luca Veit

## 📌 Descripción de la Actividad

Esta actividad aplica un enfoque estructurado y de diseño Top-Down (de lo general a lo particular). Se desarrolla una aplicación modular en C++ que valida el ingreso de un dato geométrico (radio), calcula la superficie de un círculo invocando una función con paso de parámetros y retorno de valor, y genera un renderizado condicional de una diana de tiro en arte ASCII según la escala del radio ingresado.

## 🗂 Estructura del Repositorio

```text
calculoarea/
├── src/                # Código fuente y binario compilado
│   ├── area.cpp        # Código fuente en C++ (modular)
│   └── area.exe        # Ejecutable generado
├── capturas/           # Capturas de pantalla del proceso
│   ├── diagrama_flujo.png
│   └── compilacion_area.png
├── docs/               # Documentación
│   └── InformeProyectoCALCULOAREA.pdf
├── .gitignore
├── LICENSE             # Licencia MIT
└── README.md
```

## 💻 Implementación

El programa se encuentra en `src/area.cpp` y está organizado con enfoque modular:

- **Prototipo de función:** Se declara `double calcularAreaCirculo(double radio);` antes de `main()` para informar al compilador.
- **Ingreso y validación:** Solicita el radio por consola y valida que sea mayor a 0, mostrando un mensaje de error y finalizando si es inválido.
- **Cálculo modular:** Invoca la función `calcularAreaCirculo()` que utiliza `const double PI = 3.1415926535` y retorna `PI * r * r`.
- **Salida:** Muestra el área calculada en cm².
- **Bonus - Diana ASCII:** Según el valor del radio, renderiza una diana distinta en consola:
  - `radio <= 5.0` → Diana mini/compacta
  - `radio <= 12.0` → Diana estándar de tiro
  - `radio > 12.0` → Diana gigante de cobertura

## 🛠️ Requisitos e Instalación

Para compilar y ejecutar este proyecto en Windows 10/11:

- **Visual Studio Code:** Con las extensiones oficiales C/C++ de Microsoft.
- **Compilador MinGW (GCC/G++):** Configurado en el `PATH` de Windows.
- **Git for Windows:** Para la gestión del repositorio y sincronización con GitHub.

## ▶️ Comandos para compilar y ejecutar (PowerShell - VS Code)

Asegurate de estar parado en la raíz de la carpeta `calculoarea` en la terminal integrada de VS Code (`Ctrl + Ñ`).

### Compilar el código fuente modular

```bash
g++ src/area.cpp -o src/area.exe
```

### Ejecutar la aplicación

```bash
./src/area.exe
```

## 🧪 Evidencias

El repositorio incluye capturas del proceso en la carpeta `capturas/`:

- `diagrama_flujo.png` - Diagrama de flujo del algoritmo
- `compilacion_area.png` - Proceso de compilación

## 👤 Autor

- **Alexander Luca Veit** — Programador / Estudiante  
  GitHub: [Xen-alt10](https://github.com/Xen-alt10)  
  Repositorio: [calculoarea](https://github.com/Xen-alt10/calculoarea)

## 📄 Licencia

Este proyecto está bajo licencia [MIT](LICENSE). Copyright (c) 2026 Xen-alt10.
