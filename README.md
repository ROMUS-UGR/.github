# .github
Documentacion de ROMUS
# Romus – Asistente Virtual Offline (TFG)
<p align="center">
  <img src="logo_romus.png" alt="ROMUS Logo" width="300">
</p>


Este proyecto corresponde a un **Trabajo Fin de Grado (TFG)** y consiste en el desarrollo de un **asistente virtual completamente offline**, basado en modelos de lenguaje locales (LLMs), con soporte para **RAG (Retrieval-Augmented Generation)** y **análisis de imágenes**, integrando backend, frontend y despliegue mediante Docker.

---

## Características principales

- Ejecución **100% local y offline**
- Modelos de lenguaje locales mediante **Ollama**
- Chat conversacional con historial persistente
- Soporte para documentos (PDF/TXT) mediante RAG
- Soporte para imágenes (visión)
- Backend en **FastAPI**
- Frontend en **React + TypeScript**
- Persistencia con base de datos local
- Despliegue reproducible con **Docker y Docker Compose**

---

## Requisitos

- Docker
- Docker Compose

No es necesario instalar Python, Node.js ni dependencias adicionales en el sistema.

---

## Clonado del proyecto

Para descargar el proyecto completo:

```bash
git clone https://github.com/ROMUS-UGR/Romus.git

```
Y En la carpeta padre, poner:
```bash
docker compose up --build
```
El primer arranque será lento, porque te baja los modelos y todas las dependencias, sé paciente.

## Nota Importante
No he creado un .env, para que el que quisiera pudiera probar la aplicación solo haciendo git clone, pero eso conlleva a que la firma de jwt esté hardcodeada y también el correo para la recuperación de contraseña. Lo he decidido así porque es un prototipo, evidentemente esto se debería de cambiar a un .env si alguna empresa o persona me compraría la aplicación.
