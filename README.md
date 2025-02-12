# CONTRIBUTING.github
StellarCode es un espacio dedicado al desarrollo de software con enfoque en inteligencia artificial, soluciones psicológicas y herramientas tecnológicas innovadoras.

## Forma de trabajo:

Código limpio, modular y escalable
Colaboración abierta y transparente
Seguridad y privacidad en cada desarrollo
Innovación constante con tecnologías emergentes

## 📌 Reglas generales
- Todo código debe ser probado antes de hacer un commit.
- Usa mensajes de commit descriptivos (ejemplo: `feat: agregar autenticación con Firebase`).
- Sigue el estilo de código de Java y las guías de Spring Boot.

## 🚀 Flujo de Trabajo en GitHub
1. **Fork** este repositorio y clona tu copia.
2. Crea una nueva rama con `git checkout -b feature/nombre-funcion`.
3. Realiza los cambios y confirma con `git commit -m "feat: descripción del cambio"`.
4. Sube los cambios a GitHub con `git push origin feature/nombre-funcion`.
5. Abre un **Pull Request** a `dev` y espera la revisión.

## ❗ Reportar Errores
Si encuentras un error, crea un **Issue** describiendo:
- **Qué pasó** y **cómo reproducirlo**.
- Logs o capturas de pantalla si es posible.

##
## Manejo de ramas segun el proyecto.

La estructura de ramas en GitHub para tu proyecto depende del flujo de trabajo:

---

### **1. Estructura Básica** (Ideal para proyectos pequeños)
- `main` (o `master`): Rama principal con el código en producción.
- `dev`: Rama donde se desarrollan nuevas características antes de fusionarlas a `main`.
- `feature/nueva-funcionalidad`: Ramas temporales para desarrollar nuevas funciones.
- `bugfix/arreglo-bug`: Ramas para corregir errores específicos.

---

### **2. Git Flow** (Ideal para proyectos medianos/grandes)
- `main`: Código estable y listo para producción.
- `develop`: Código en desarrollo, a partir del cual se crean nuevas funciones.
- `feature/*`: Ramas de nuevas características, parten de `develop` y se fusionan a `develop`.
- `release/*`: Preparación de una nueva versión antes de pasar a `main`.
- `hotfix/*`: Correcciones urgentes que parten de `main` y se fusionan en `develop` y `main`.

---

### **3. GitHub Flow** (Más simple y flexible)
- `main`: Única rama estable.
- `feature/*`: Ramas para nuevas características, que se fusionan a `main` mediante Pull Requests.
- `fix/*`: Ramas para corregir errores.

---

### **Recomendación para tu proyecto**
Dado que estás desarrollando una **API CRUD en Spring Boot con Firebase**, te sugeriría algo intermedio:

1. `main` → Código estable en producción.
2. `dev` → Desarrollo de nuevas funciones antes de fusionarlas a `main`.
3. `feature/nombre` → Para cada nueva funcionalidad (ejemplo: `feature/firebase-auth`).
4. `bugfix/nombre` → Para corregir errores específicos.

