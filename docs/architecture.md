# architecture.md

# Proyecto Principal — Plataforma Geoespacial y Observatorio Urbano

## Objetivo General

Desarrollar una plataforma web moderna orientada a visualización y análisis de datos urbanos y geoespaciales, utilizando tecnologías frontend y backend actuales, con arquitectura escalable y despliegue real en VPS.

El proyecto debe funcionar como:

* Producto técnicamente serio
* Pieza principal de portfolio
* Demostración de arquitectura fullstack
* Experiencia práctica real
* Base extensible para futuras funcionalidades o monetización

---

# Concepto Inicial

## Nombre provisional

* Observatorio Urbano CABA
* Urban Data Hub
* GeoCABA
* Urban Layers
* Atlas Urbano

(El nombre definitivo puede definirse más adelante.)

---

# Idea Principal

La plataforma permitirá visualizar y explorar información urbana mediante mapas interactivos, dashboards y capas temáticas.

El foco inicial estará puesto en:

* visualización geoespacial
* datos públicos
* filtros y análisis
* experiencia de usuario
* arquitectura backend
* despliegue real

---

# Objetivos Técnicos

## Backend

Construir una API moderna y mantenible utilizando:

* NestJS
* TypeScript
* PostgreSQL
* PostGIS
* JWT Authentication
* Roles y permisos
* Validaciones
* Arquitectura modular
* DTOs
* Guards
* Configuración segura mediante variables de entorno

---

## Frontend

Desarrollar una SPA moderna utilizando:

* Angular
* RxJS
* Angular Signals (si resulta conveniente)
* Angular Material o Tailwind
* Leaflet o MapLibre GL JS
* Lazy loading
* Guards
* Manejo de estado
* Formularios reactivos

---

## Infraestructura

Implementar despliegue real utilizando:

* VPS Ubuntu
* Nginx
* HTTPS
* Docker (principalmente para PostgreSQL)
* Variables de entorno
* PM2 o sistema equivalente
* Dominio propio

---

# MVP Inicial

## Primera Meta Funcional

Contar con una plataforma online capaz de:

### Backend

* autenticación básica
* registro/login
* roles
* CRUD de datasets
* CRUD de capas geográficas
* endpoints protegidos
* carga de datos simples

### Frontend

* mapa interactivo
* visualización de capas
* panel lateral
* filtros básicos
* login
* panel administrador inicial

---

# Tipos de Datos Iniciales

El sistema podrá mostrar inicialmente:

* barrios
* hospitales
* universidades
* espacios verdes
* estaciones de transporte
* datos censales
* alquileres
* zonas inundables
* calor urbano

Los datos podrán provenir de:

* APIs públicas
* archivos GeoJSON
* datasets abiertos
* WMS/WFS
* carga manual

---

# Roles Iniciales

## Usuario Público

* explorar mapas
* activar/desactivar capas
* aplicar filtros

## Usuario Registrado

* guardar favoritos
* personalizar visualización
* guardar capas preferidas

## Administrador

* cargar datasets
* administrar capas
* moderar contenido
* gestionar usuarios

---

# Arquitectura General

## Frontend

Angular SPA

↓

## API

NestJS REST API

↓

## Base de Datos

PostgreSQL + PostGIS

---

# Prioridades Iniciales

## Fase 1 — Base Técnica

### Objetivo

Tener backend funcional y deployado.

### Tareas

* inicializar NestJS
* configurar PostgreSQL
* configurar Docker
* auth JWT
* roles
* estructura modular
* configuración de entorno
* primeras entidades
* deploy inicial VPS

---

## Fase 2 — Frontend Base

### Objetivo

Consumir la API y visualizar datos básicos.

### Tareas

* iniciar Angular
* login
* guards
* layout principal
* mapa interactivo
* consumo de endpoints
* panel lateral

---

## Fase 3 — Datos Reales

### Objetivo

Integrar datasets reales.

### Tareas

* GeoJSON
* APIs públicas
* filtros
* clustering
* capas dinámicas

---

## Fase 4 — UX y Producto

### Objetivo

Hacer que la plataforma se vea profesional.

### Tareas

* dashboards
* estadísticas
* bookmarks
* visualización avanzada
* responsive
* performance

---

# Objetivos Profesionales del Proyecto

El proyecto debe permitir demostrar:

* arquitectura fullstack
* diseño backend
* APIs REST
* autenticación y permisos
* visualización geoespacial
* manejo de datos
* frontend avanzado
* despliegue real
* infraestructura básica
* experiencia cercana a un producto real

---

# Restricciones Importantes

* evitar sobreingeniería temprana
* evitar microservicios inicialmente
* evitar intentar competir con plataformas enormes
* priorizar MVP funcional
* priorizar consistencia arquitectónica
* priorizar deploy temprano

---

# Objetivo Final

Construir una plataforma técnicamente sólida, visualmente profesional y con identidad propia, capaz de funcionar como:

* portfolio principal
* demostración de experiencia práctica
* producto extensible
* posible base comercial futura
* puente hacia experiencia profesional real
