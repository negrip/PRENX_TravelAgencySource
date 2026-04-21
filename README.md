# PRENX_TravelAgency

GeneXus Knowledge Base para el sistema de agencia de viajes con inteligencia artificial.

## Descripción

Este repositorio contiene los archivos fuente (texto plano) de la Knowledge Base **PRENX_TravelAgency** exportados desde GeneXus. El proyecto implementa una aplicación de agencia de viajes con dos módulos principales:

- **Backoffice**: Panel de administración para gestionar atracciones turísticas, categorías, países y datos del sistema
- **CustomerFacing**: Interfaz pública para clientes con búsqueda de atracciones y agentes conversacionales de IA

## 🚀 Características

- Sistema de gestión de atracciones turísticas
- Catálogo organizado por países, ciudades y categorías
- Agentes de IA conversacionales para asistencia al cliente
- Integración con servicios de clima (Weather)
- Diseño basado en GeneXus Unanimo Design System
- Arquitectura modular y escalable

## 📁 Estructura del Proyecto

```
PRENX_TravelAgencySource/
├── src/                          # Objetos GeneXus en formato texto
│   ├── Backoffice/              # Módulo de administración
│   │   ├── Agents/              # Agentes de IA para backoffice
│   │   ├── Data/                # Transacciones y estructuras de datos
│   │   └── DesignSystem/        # Componentes UI del backoffice
│   ├── CustomerFacing/          # Módulo público/clientes
│   │   ├── CF_Agents/           # Agentes conversacionales
│   │   ├── CF_Chat/             # Sistema de chat
│   │   └── CF_DesignSystem/     # Componentes UI del frontend
│   ├── General/                 # Módulo de utilidades generales
│   ├── Weather/                 # Integración con servicios de clima
│   ├── GeneXus/                 # Objetos base de GeneXus
│   ├── GeneXusUIControls/       # Controles de usuario GeneXus
│   └── GeneXusUnanimo/          # Componentes Unanimo
└── src.ns/                      # Namespace y estructura de módulos
```

## 🛠️ Requisitos Previos

- **GeneXus**: Versión 18 o superior con soporte para GeneXus Next
- **DBMS**: SQL Server (configurado en la KB)
- **Generador**: .NET o Java según configuración del modelo
- **Node.js**: Para user controls y componentes web

## 📥 Instalación

### Opción 1: Abrir Knowledge Base Existente

Si ya tienes la KB creada en `C:\Modelos_Next\PRENX_TravelAgency`:

```bash
# Abrir la KB con GeneXus Next MCP
gxnext open-knowledge-base --directory "C:\Modelos_Next\PRENX_TravelAgency"
```

### Opción 2: Importar desde Texto

Para importar los objetos a una KB nueva o existente:

```bash
# 1. Crear/abrir tu Knowledge Base en GeneXus
# 2. Usar la herramienta de importación de texto de GeneXus
# 3. Seleccionar el directorio src/ de este repositorio
```

### Opción 3: Usar MCP de GeneXus (Recomendado)

```bash
# Importar todos los objetos
gxnext import-text-to-kb --names "[all]" --root-directory "./src"

# Importar módulos específicos
gxnext import-text-to-kb --names "Backoffice;CustomerFacing" --root-directory "./src"
```

## 🔧 Configuración

### Variables de Entorno

El proyecto puede requerir configuración de:
- Claves API para servicios de IA
- Endpoints de servicios externos
- Configuración de base de datos

### Base de Datos

La KB utiliza SQL Server. Asegúrate de:
1. Tener SQL Server instalado y corriendo
2. Configurar la cadena de conexión en las propiedades del modelo
3. Ejecutar la reorganización después de importar

```bash
# Reorganizar la base de datos
gxnext reorganize
```

## 🏗️ Desarrollo

### Compilar el Proyecto

```bash
# Compilar todos los objetos
gxnext build-all

# Compilar un objeto específico
gxnext build-one --object-name "Home"
```

### Ejecutar la Aplicación

```bash
# Ejecutar el backoffice
gxnext run --object-name "Home"

# Ejecutar el frontend
gxnext run --object-name "TravelAgencyMaster"
```

## 📦 Módulos Principales

### Backoffice
- **Home**: Panel principal de administración
- **Agents**: Configuración de agentes de IA
- **Data**: Gestión de atracciones, categorías, países
- **DesignSystem**: Componentes reutilizables

### CustomerFacing
- **Attractions**: Catálogo de atracciones turísticas
- **CF_Agents**: Agentes conversacionales para clientes
- **CF_Chat**: Interfaz de chat en tiempo real
- **TravelAgencyMaster**: Master page del sitio público

### Weather
- Integración con APIs meteorológicas
- Información de clima para destinos turísticos

## 🤝 Contribuir

1. Fork el repositorio
2. Crea una rama para tu feature (`git checkout -b feature/nueva-funcionalidad`)
3. Realiza tus cambios en GeneXus
4. Exporta los objetos modificados a texto
5. Commit los cambios (`git commit -m 'Agregar nueva funcionalidad'`)
6. Push a la rama (`git push origin feature/nueva-funcionalidad`)
7. Abre un Pull Request

## 📄 Información de la Knowledge Base

- **Nombre:** PRENX_TravelAgency
- **Ubicación local:** `C:\Modelos_Next\PRENX_TravelAgency`
- **Repositorio fuente:** `C:\Modelos_Next\PRENX_TravelAgencySource`
- **Formato de exportación:** GeneXus Object Text Format

## 📚 Documentación Adicional

- [GeneXus Wiki](https://wiki.genexus.com)
- [GeneXus Next Documentation](https://next.genexus.com)
- [GeneXus Unanimo Design System](https://unanimo.genexus.com)

## 📝 Licencia

[Especificar licencia del proyecto]

## 👥 Autores

[Especificar autores y contacto]

---

**Nota**: Este es un proyecto GeneXus. Los archivos en `src/` están en formato texto plano de GeneXus y deben ser importados a una Knowledge Base para su edición y compilación.
