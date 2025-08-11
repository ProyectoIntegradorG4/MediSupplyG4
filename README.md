# MediSupply - Proyecto Final MISW4501-202514

## Equipo de Trabajo - Grupo 4

| Integrantes	| Nombres	| Apellidos	| Correo electrónico @uniandes.edu.co |
|---|---|---|---|
| 1	| Juan Pablo	| Rodriguez Morales	| jp.rodriguezm@uniandes.edu.co| 
| 2 |	Luz Stella | 	Ochoa Marin	| ls.ochoa@uniandes.edu.co|
| 3 |	Julio César	| Forero Orjuela	| jc.foreroo1@uniandes.edu.co|
| 4 |	Wilson	| Aponte García	| w.aponte@uniandes.edu.co|

## Descripción del Proyecto

MediSupply es una empresa multinacional dedicada a la distribución de insumos médicos, medicamentos de alta complejidad y equipos biomédicos a instituciones de salud en América Latina. El proyecto consiste en desarrollar una plataforma tecnológica integral que optimice la cadena de suministros médicos.

## Estructura del Proyecto

```
MediSupplyG4/
├── DocumentacionProyecto/         # Documentación del proyecto
│   ├── 00-ANALISIS-PIDE-SOLU-PLAN-ORDEN.md
│   ├── 00-ESTADO-ACTUAL-PROYECTO.md
│   ├── 01-Planificacion/          # Documentos de planificación del proyecto
│   │   ├── 01-Acta-Constitucion.md
│   │   ├── 02-Epicas-Features.md
│   │   ├── 03-Planificacion-Sprints.md
│   │   └── 04-Historias-Usuario-Detalladas.md
│   ├── 02-Arquitectura/           # Documentos de arquitectura del sistema
│   │   ├── 01-Documento-Alcance.md
│   │   ├── 02-Hoja-Trabajo-Objetivos-Restricciones.md
│   │   ├── 03-Estrategia-Pruebas.md
│   │   ├── 04-Vision-Arquitectura.md
│   │   ├── 05-Escenarios-Calidad.md
│   │   ├── 06-Frameworks-Ambientes.md
│   │   ├── 07-Patrones-Diseno.md
│   │   ├── 08-Experimentos-Arquitectura.md
│   │   └── 09-Refinamiento-Arquitectura.md
│   ├── 03-VALIDACION-RUBRICA.md
│   ├── 04-Gestion/                # Gestión del proyecto
│   │   ├── 01-Tablero-Proyecto.md
│   │   ├── 02-Wiki-Estructura.md
│   │   └── Checklist-Actualizacion-Board-Semana3.md
│   ├── 05-RIESGOS-DECISIONES-ASR.md
│   ├── 06-PROXIMOS-PASOS.md
│   └── 07-CHECKLIST-SEMANA-ACTUAL.md
├── wiki/                          # Wiki del proyecto (submódulo Git)
│   └── MediSupplyG4.wiki/        # Contenido de la wiki
│       ├── Home.md
│       ├── Semana-1.md
│       ├── Semana-2.md
│       ├── Semana-3.md
│       ├── Semana-4.md
│       ├── Semana-5.md
│       ├── Semana-6.md
│       ├── Semana-7.md
│       ├── Semana-8.md
│       ├── 05-Entregables/
│       └── DocumentosOficiales/
├── LICENSE
└── README.md
```

## Cronograma del Proyecto

- **Semanas 1-8**: Diseño de arquitectura y pruebas de concepto
- **Semanas 9-16**: Desarrollo de la primera versión de la aplicación
- **Semana 16**: Entrega final del prototipo

## Stack Tecnológico Seleccionado

### Backend
- **Framework**: Python Flask
- **Base de Datos**: PostgreSQL/MySQL
- **Autenticación**: JWT (JSON Web Tokens)
- **APIs**: RESTful APIs con documentación Swagger

### Frontend Web
- **Framework**: React.js
- **Estado**: Redux/Context API
- **UI**: Material-UI o Ant Design
- **Internacionalización**: i18next

### Aplicación Móvil
- **Framework**: React Native
- **Plataformas**: Android e iOS
- **Navegación**: React Navigation
- **Estado**: Redux Toolkit

### Infraestructura
- **Cloud**: AWS (Amazon Web Services)
- **Contenedores**: Docker
- **CI/CD**: GitHub Actions
- **Monitoreo**: CloudWatch, Sentry

### Calidad y Testing
- **Backend**: pytest, coverage
- **Frontend**: Jest, React Testing Library
- **Móvil**: Jest, Detox
- **E2E**: Cypress, Appium

## Enlaces Importantes

- [Acta de Constitución](./DocumentacionProyecto/01-Planificacion/01-Acta-Constitucion.md)
- [Épicas y Features](./DocumentacionProyecto/01-Planificacion/02-Epicas-Features.md)
- [Planificación de Sprints](./DocumentacionProyecto/01-Planificacion/03-Planificacion-Sprints.md)
- [Documento de Alcance](./DocumentacionProyecto/02-Arquitectura/01-Documento-Alcance.md)
- [Wiki del Proyecto](./wiki/MediSupplyG4.wiki/Home.md)

## Estado del Proyecto

### ✅ Completado (Semana 1)
- [x] Acta de Constitución del Proyecto
- [x] Épicas y Features del Sistema
- [x] Planificación de Sprints
- [x] Guía para Video de Entrega

### 🔄 En Progreso (Semana 2)
- [x] Documento del Alcance (EDT) - Completado
- [x] Hoja de Trabajo con Objetivos y Restricciones - Completado
- [x] Documento de Estrategia de Pruebas - Completado
- [ ] Visión de Arquitectura - En desarrollo
- [ ] Modelos de Arquitectura (Contexto, Dominio, Componentes, Despliegue)
- [ ] Board del Proyecto actualizado
- [ ] Showcase de la Semana 2

### 📋 Pendiente
- [ ] Experimentos de Arquitectura
- [ ] Prototipos de Prueba de Concepto
- [ ] Desarrollo de la Aplicación

## Clonación del Proyecto

### Clonar todo (proyecto + submódulos):
```bash
git clone --recurse-submodules git@github.com:ProyectoIntegradorG4/MediSupplyG4.git
```

### Si ya clonado:
```bash
git submodule update --init --recursive
```

### Actualizar submódulos:
```bash
git submodule update --remote
```

## Entregables de la Semana 2

### ✅ Completados
- **Documento del alcance**: EDT en formato árbol y tabular
- **Hoja de trabajo**: Objetivos, restricciones y requisitos de calidad
- **Estrategia de pruebas**: Componentes, alcance y tipos de pruebas

### 🔄 En Desarrollo
- **Visión de arquitectura**: Modelos de contexto, dominio, componentes y despliegue
- **Board del proyecto**: Actualización del tablero Kanban
- **Showcase**: Video de presentación de la semana 2

---

**Última actualización**: Semana 2 - Proyecto MISW4501-202514

