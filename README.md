# 🏢 Sistema de Gestión de Empleados - FullStack

Aplicación web full-stack para la gestión centralizada de empleados. Permite a los departamentos de RRHH crear, visualizar, actualizar y eliminar la información de los empleados de manera sencilla y segura.

## 📸 Capturas de Pantalla

| Vista de Lista de Empleados | Agregar Empleado | Formulario de Edición |
| :---: | :---: | :---: |
| ![Vista Lista](https://github.com/RocioGuimet/RecursosHumanos_FullStack/blob/main/Screenshots/Screenshot%20(1).png?raw=true) | ![Vista Agregar](https://github.com/RocioGuimet/RecursosHumanos_FullStack/blob/main/Screenshots/Screenshot%20(2).png?raw=true) | ![Vista Formulario](https://github.com/RocioGuimet/RecursosHumanos_FullStack/blob/main/Screenshots/Screenshot%20(3).png?raw=true) |

## 🚀 Tecnologías Utilizadas

### **Backend**
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

### **Frontend**
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
![Axios](https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white)

## 🛠️ Características

- **CRUD Completo**: Crear, Leer, Actualizar y Eliminar registros de empleados.
- **API RESTful**: Backend construido con Spring Boot siguiendo principios REST.
- **Interfaz Reactiva**: Frontend en React que se actualiza instantáneamente.
- **Diseño Responsive**: Se adapta a móviles, tablets y ordenadores.
- **Persistencia de Datos**: Base de datos MySQL gestionada con Spring Data JPA.

## 📦 Instalación y Ejecución Local

Sigue estos pasos para ejecutar el proyecto.

### **Prerrequisitos**
- [Java 17 o superior](https://adoptium.net/)
- [Node.js y npm](https://nodejs.org/)
- [MySQL](https://dev.mysql.com/downloads/) instalado y ejecutándose.

### **1. Clonar el Repositorio**
```bash
git clone https://github.com/TU_USUARIO/RecursosHumanos_FullStack.git
cd RecursosHumanos_FullStack
```

### **2. Configurar la Base de Datos (Backend)**
1. Entra en la carpeta del backend:
```bash
cd RecursosHumanosSpring
```

```bash
# Copia el archivo de ejemplo
cp src/main/resources/application.properties.example src/main/resources/application.properties

# Edita el nuevo archivo con tus credenciales de MySQL
# Cambia: TU_USUARIO_AQUI → tu usuario (ej: 'root')
# Cambia: TU_CONTRASEÑA_AQUI → tu contraseña
```
```bash
# En lugar de editar el archivo, puedes hacer:
export DB_USERNAME=tu_usuario
export DB_PASSWORD=tu_contraseña
```
### **3. Ejecutar el Backend (Spring Boot)**
Desde la carpeta `RecursosHumanosSpring`, ejecuta:

```bash
# En Windows
mvnw.cmd spring-boot:run

# En Linux/Mac
./mvnw spring-boot:run
```
El servidor empezará en http://localhost:8080. Deberías ver mensajes de Spring en la consola.

### **4. Configurar y Ejecutar el Frontend (React)**
1. Abre una NUEVA terminal y vuelve a la carpeta principal:

```bash
cd ..
```
Entra en la carpeta del frontend:

```bash
cd RecursosHumanosReact
```
Instala las dependencias:

```bash
npm install
```
Inicia la aplicación:

```bash
npm start
```
Abre tu navegador en http://localhost:3000.

## 📁 Estructura del Proyecto
```
RecursosHumanos_FullStack/
├── RecursosHumanosSpring/          # Backend (Spring Boot)
│   ├── src/main/java/com/example/
│   │   ├── controller/    # Controladores REST
│   │   ├── service/       # Lógica de negocio
│   │   ├── repository/    # Acceso a datos
│   │   └── model/         # Entidades (Empleado.java)
│   └── pom.xml            # Dependencias de Maven
├── RecursosHumanosReact/      # Frontend (React)
│   ├── src/
│   │   ├── components/    # Componentes React
│   │   └── App.js         # Componente principal
│   └── package.json       # Dependencias de Node
└── Screenshots/           # Capturas de pantalla
