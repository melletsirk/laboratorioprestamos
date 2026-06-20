# 💰 Sistema de Gestión de Préstamos

Aplicación web para la administración y gestión de solicitudes de préstamos, desarrollada bajo una arquitectura cliente-servidor. El sistema permite registrar usuarios, gestionar solicitudes, evaluar préstamos y realizar el seguimiento de estados mediante una interfaz intuitiva y segura.

## 🚀 Características

* Registro e inicio de sesión de usuarios.
* Gestión de clientes.
* Solicitud de préstamos.
* Evaluación y aprobación de préstamos.
* Consulta de historial de préstamos.
* Gestión de cuotas y pagos.
* Control de estados (Pendiente, Aprobado, Rechazado, Cancelado).
* Interfaz web responsiva.
* API REST para comunicación entre frontend y backend.

## 🛠️ Tecnologías Utilizadas

### Backend

* Python
* FastAPI / Flask (según corresponda)
* SQLAlchemy
* PostgreSQL / MySQL
* JWT Authentication

### Frontend

* HTML5
* CSS3
* JavaScript
* Bootstrap / React (según corresponda)

### Base de Datos

* PostgreSQL / MySQL

## 📂 Estructura del Proyecto

```text
laboratorioprestamos/
│
├── backend/
│   ├── app/
│   ├── models/
│   ├── routes/
│   ├── services/
│   └── database/
│
├── frontend/
│   ├── src/
│   ├── assets/
│   ├── components/
│   └── pages/
│
├── docs/
├── screenshots/
└── README.md
```

## ⚙️ Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/melletsirk/laboratorioprestamos.git
cd laboratorioprestamos
```

### 2. Configurar el Backend

```bash
cd backend

python -m venv .venv

# Linux/Mac
source .venv/bin/activate

# Windows
.venv\Scripts\activate

pip install -r requirements.txt
```

Configurar variables de entorno:

```env
DB_HOST=localhost
DB_PORT=5432
DB_NAME=prestamos
DB_USER=usuario
DB_PASSWORD=password
SECRET_KEY=tu_clave_secreta
```

Ejecutar el servidor:

```bash
uvicorn main:app --reload
```

### 3. Configurar el Frontend

```bash
cd frontend

npm install
npm run dev
```

## 🔐 Roles del Sistema

### Administrador

* Gestionar usuarios.
* Aprobar o rechazar préstamos.
* Consultar reportes.
* Administrar clientes.

### Usuario

* Solicitar préstamos.
* Consultar estado de solicitudes.
* Revisar historial de préstamos.

## 📸 Capturas

Agregar aquí imágenes del sistema.

```markdown
![Login](screenshots/login.png)
![Dashboard](screenshots/dashboard.png)
![Solicitudes](screenshots/solicitudes.png)
```

## 📖 API

### Autenticación

```http
POST /api/auth/login
```

### Solicitar préstamo

```http
POST /api/prestamos
```

### Obtener préstamos

```http
GET /api/prestamos
```

## 👨‍💻 Autor

**Melissa Chambi Flores**

GitHub: https://github.com/melletsirk

## 📄 Licencia

Este proyecto fue desarrollado con fines académicos y educativos.
