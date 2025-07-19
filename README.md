# Simulación de Controlador de Dominio con Active Directory en Windows Server 2019

## Objetivo

Instalar y configurar **Active Directory Domain Services (AD DS)** en un entorno simulado con Windows Server 2019, promoviendo el servidor a **controlador de dominio**, creando usuarios, grupos y asignando permisos según buenas prácticas de ciberseguridad.

---

## Entorno de laboratorio

-  Sistema: Windows Server 2019 Standard Evaluation (VMware Workstation)
-  Recursos: 4 GB RAM, 2 vCPU, disco de 40 GB
-  Red: NAT o Red Interna
-  Roles:
  - AD DS (Servicios de Dominio)
  - DNS (automáticamente añadido)
  - GPMC (Group Policy Management Console)

---

## Configuración realizada

1. Renombrado del servidor a `DC-Server`
2. Instalación del rol **AD DS**
3. Promoción del servidor a **Controlador de Dominio** con el dominio: `windom.local`
4. Creación de unidad organizativa (OU): `Soporte TI`
5. Creación de usuario:
   - Nombre completo: Jose Luis JL. Guerra Gomez
   - Usuario: `j.gomez@windom.local`
6. Creación de grupo de seguridad: `Seguridad`
7. Asignación del usuario al grupo
8. Creación de carpeta compartida: `Datos Compartidos`
9. Asignación de permisos NTFS por grupo (`Seguridad`)
10. Validación del acceso en propiedades de carpeta

---

## Evidencias (capturas de pantalla)

Incluye imágenes de:

- Instalación de roles
- Promoción a controlador de dominio
- Panel ADUC (Usuarios y equipos de Active Directory)
- Creación de usuario y OU
- Permisos en carpeta compartida (`Seguridad`)

---

## Aplicaciones futuras

Esta infraestructura puede ampliarse para prácticas de:

- Aplicación de GPOs
- Configuración de políticas de contraseñas
- Restricción de uso de dispositivos (USB)
- Registro de eventos (auditoría de accesos)
- Simulación de ataques internos con usuarios comprometidos

---

## Archivos asociados

- Capturas de pantalla en formato PNG 
- Este archivo README.md

---

## Autor

- **Emiliano Martínez Vega**  
- Especialista en Ciberseguridad y Redes  
