## 1. Estructura Básica (Ideal para proyectos pequeños)
main (o master): Rama principal con el código en producción.
dev: Rama donde se desarrollan nuevas características antes de fusionarlas a main.
feature/nueva-funcionalidad: Ramas temporales para desarrollar nuevas funciones.
bugfix/arreglo-bug: Ramas para corregir errores específicos.

## 2. Git Flow (Ideal para proyectos medianos/grandes)
main: Código estable y listo para producción.
develop: Código en desarrollo, a partir del cual se crean nuevas funciones.
feature/*: Ramas de nuevas características, parten de develop y se fusionan a develop.
release/*: Preparación de una nueva versión antes de pasar a main.
hotfix/*: Correcciones urgentes que parten de main y se fusionan en develop y main.

## 3. GitHub Flow (Más simple y flexible)
main: Única rama estable.
feature/*: Ramas para nuevas características, que se fusionan a main mediante Pull Requests.
fix/*: Ramas para corregir errores.
Recomendación para tu proyecto
Dado que estás desarrollando una API CRUD en Spring Boot con Firebase, te sugeriría algo intermedio:

main → Código estable en producción.
dev → Desarrollo de nuevas funciones antes de fusionarlas a main.
feature/nombre → Para cada nueva funcionalidad (ejemplo: feature/firebase-auth).
bugfix/nombre → Para corregir errores específicos.
