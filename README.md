# Configuraciones de Kubernetes

Este repositorio contiene toda la configuración necesaria para desplegar y gestionar la infraestructura de nuestros servicios en un entorno Kubernetes. Aquí encontrarás la definición y orquestación de servicios, bases de datos, servicios externos y otros componentes que conforman nuestra arquitectura.

## Contenido del Repositorio

- **Servicios**: Configuraciones y despliegues de nuestros microservicios y aplicaciones.
- **Bases de Datos**: Definiciones para la creación y administración de bases de datos utilizadas por la aplicación.
- **Servicios Externos**: Configuraciones para la integración con APIs y servicios de terceros.
- **Recursos Adicionales**: Configuraciones para volúmenes persistentes, secretos, configuraciones de red y otros componentes necesarios.

## Requisitos Previos

Antes de desplegar las configuraciones, asegúrate de tener:

- **Kubernetes** instalado y configurado.
- **kubectl** configurado y apuntando al cluster correspondiente.
- Acceso a los repositorios de imágenes de contenedores necesarios.

## Despliegue

Para aplicar las configuraciones, utiliza el comando `kubectl apply` en cada directorio o en el archivo correspondiente:

```bash
# Desplegar todos los recursos de una carpeta
kubectl apply -f services/

# Desplegar una configuración específica
kubectl apply -f databases/mysql.yaml