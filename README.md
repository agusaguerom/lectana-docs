# LECTANA

Lectana es una plataforma digital integral que facilite el acceso gratuito, equitativo y personalizado a cuentos y libros, fomentando el hábito de la lectura y fortaleciendo la interacción entre estudiantes y docentes. El sistema integra una aplicación móvil y un panel web que garantiza una gestión centralizada y una experiencia de uso fluida

## 🌐 Web
- [Ver aplicación](https://lectana.vercel.app)

## 📦 Repositorios

- [Frontend](https://github.com/tomiiroma/lectana-frontend-web.git)
- [Backend](https://github.com/tomiiroma/lectana-backend.git)
- [App Movil](https://github.com/Kerooo0/lectana-app-mobile.git)


## 🛠️ Tecnologías utilizadas

### Frontend Web
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![React Router](https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white)
![Axios](https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white)

### Backend
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![Zod](https://img.shields.io/badge/Zod-3E67B1?style=for-the-badge&logo=zod&logoColor=white)

### App Móvil
![Android](https://img.shields.io/badge/Android_Studio-3DDC84?style=for-the-badge&logo=androidstudio&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)

## ✨ Funcionalidades principales

### 📱 App Móvil
**Estudiantes**
- 📚 Acceso a catálogo de cuentos y libros con lectura en línea
- 🔊 Reproducción en modo audiolibro
- 🎮 Actividades interactivas y retos gamificados
- 📊 Seguimiento de progreso personal

**Docentes**
- 🏫 Gestión de aulas virtuales y asignación de lecturas
- ✏️ Creación y corrección de actividades
- 💬 Comunicación con estudiantes via mensajes y comentarios

### 🖥️ Panel Web (Administración)
- 📖 Gestión del catálogo de libros y cuentos
- 👥 Administración de usuarios y aulas
- 🔍 Supervisión general del sistema

## 🏗️ Arquitectura

La plataforma sigue una arquitectura **cliente-servidor** con tres clientes conectados a una API REST central.
```
[App Móvil - Android]  ─┐
                         ├──► [API REST - Node.js/Express] ──► [Supabase DB]
[Web - React]          ─┘              │
                                       └──► [ElevenLabs API]
                                            (Audiolibros)
```

### Backend
Organizado en capas: `routes → controllers → services → database`
Con `middleware` para autenticación JWT y validación con Zod.

### Frontend Web
Arquitectura de componentes React con separación en `components`, `layouts`, `hooks` y `services`.

### App Móvil
Patrón **Repository** con capas `models → repository → services → adapters`.
## Documentacion

- [SRS](./docs/SRS.pdf)
- [DER](./docs/DER.jpeg)
- [Casos de prueba](./docs/casos-de-prueba.pdf)


